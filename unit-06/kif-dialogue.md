```ruby
;; Types and attributes
(∀ (?x) (=> (Television ?x) (and (Product ?x) (hasAttr ?x sizeInches) (hasAttr ?x hdmiSlots))))
(= (sizeInches ?t) 50)            ;; numeric attribute (inches)
(= (hdmiSlots  ?t) n)             ;; integer number of HDMI ports
(= (inStockQty ?t) q)             ;; integer quantity on hand
(= (model ?t) "STRING")           ;; model identifier

;; Derived/query functions
(totalAvailable ?pred)            ;; sums (inStockQty ?t) over all ?t where ?pred holds
(sum ?x ?pred ?expr)              ;; generic summation form
(reserveBatch ?pred n)            ;; action: create a reservation of n units matching ?pred
(reservationId "…")               ;; reservation identifier when successful

```