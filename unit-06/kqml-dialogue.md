```ruby
1) (ask-if
      :sender    Alice
      :receiver  Bob
      :ontology  retail-warehouse-ont
      :language  KIF
      :reply-with  A1
      :content
        (exists (?t ?q)
          (and (Television ?t)
               (= (sizeInches ?t) 50)
               (inStock ?t ?q)
               (> ?q 0)))))

2) (tell
      :sender    Bob
      :receiver  Alice
      :in-reply-to A1
      :ontology  retail-warehouse-ont
      :language  KIF
      :content
        (exists (?t)
          (and (Television ?t)
               (= (sizeInches ?t) 50)
               (> (inStockQty ?t) 0)))))

3) (ask-one
      :sender    Alice
      :receiver  Bob
      :ontology  retail-warehouse-ont
      :language  KIF
      :reply-with  A2
      :content
        (totalAvailable
          (lambda (?t)
            (and (Television ?t)
                 (= (sizeInches ?t) 50)))) )

4) (tell
      :sender    Bob
      :receiver  Alice
      :in-reply-to A2
      :ontology  retail-warehouse-ont
      :language  KIF
      :content
        (= (totalAvailable
             (lambda (?t)
               (and (Television ?t)
                    (= (sizeInches ?t) 50))))
           24))

5) (ask-all
      :sender    Alice
      :receiver  Bob
      :ontology  retail-warehouse-ont
      :language  KIF
      :reply-with  A3
      :content
        (and (Television ?t)
             (= (sizeInches ?t) 50)
             (= ?m (model ?t))
             (= ?s (hdmiSlots ?t))))

6) (tell
      :sender    Bob
      :receiver  Alice
      :in-reply-to A3
      :ontology  retail-warehouse-ont
      :language  KIF
      :content
        (set
          (tuple (model "ACME-50UHD-2025") (hdmiSlots 3) (inStockQty 12))
          (tuple (model "ZenView-50QLED")  (hdmiSlots 4) (inStockQty 8))
          (tuple (model "Nova-50HDR")      (hdmiSlots 2) (inStockQty 4))))

7) (ask-if
      :sender    Alice
      :receiver  Bob
      :ontology  retail-warehouse-ont
      :language  KIF
      :reply-with  A4
      :content
        (>= (sum ?t
                 (and (Television ?t)
                      (= (sizeInches ?t) 50))
                 (inStockQty ?t))
            20))

8) (tell
      :sender    Bob
      :receiver  Alice
      :in-reply-to A4
      :ontology  retail-warehouse-ont
      :language  KIF
      :content
        (true))

9) (request
      :sender    Alice
      :receiver  Bob
      :ontology  retail-warehouse-ont
      :language  KIF
      :reply-with  A5
      :content
        (reserveBatch
           (and (Television ?t)
                (= (sizeInches ?t) 50))
           20))

10) (agree
       :sender    Bob
       :receiver  Alice
       :in-reply-to A5
       :ontology  retail-warehouse-ont
       :language  KIF
       :content
         (willDo (reserveBatch
                   (and (Television ?t)
                        (= (sizeInches ?t) 50))
                   20)))

11) (inform
       :sender    Bob
       :receiver  Alice
       :ontology  retail-warehouse-ont
       :language  KIF
       :content
         (and
           (= (reservationId "R-5087-2025-10-13"))
           (= (reservedQty 20))
           (= (mix
               (list
                 (tuple "ACME-50UHD-2025" 12 3)
                 (tuple "ZenView-50QLED"  8 4))))))

;; Notes:
;; - tuple fields in (mix) are (model, reservedUnits, hdmiSlots).
```