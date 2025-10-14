# Constituency-Based Parse Trees

This document provides Penn Treebank–style constituency parses (with bracketed notation and ASCII trees) for three sentences. Where the sentence is structurally ambiguous, multiple parses are shown.

---

## 1) The government raised interest rates.

**Bracketed notation (PTB style):**  
```
(S
  (NP (DT The) (NN government))
  (VP (VBD raised)
      (NP (NN interest) (NNS rates)))
  (. .))
```

**ASCII tree:**  
```
S
├── NP
│   ├── DT The
│   └── NN government
├── VP
│   ├── VBD raised
│   └── NP
│       ├── NN interest
│       └── NNS rates
└── . .
```

---

## 2) The internet gives everyone a voice.

**Bracketed notation (PTB style):**  
```
(S
  (NP (DT The) (NN internet))
  (VP (VBZ gives)
      (NP (NN everyone))
      (NP (DT a) (NN voice)))
  (. .))
```

**ASCII tree:**  
```
S
├── NP
│   ├── DT The
│   └── NN internet
├── VP
│   ├── VBZ gives
│   ├── NP
│   │   └── NN everyone
│   └── NP
│       ├── DT a
│       └── NN voice
└── . .
```

---

## 3) The man saw the dog with the telescope.

This sentence is ambiguous (PP-attachment). Below are the two common parses.

### A) Instrument attachment to **VP** (“saw … with the telescope”)

**Bracketed notation:**  
```
(S
  (NP (DT The) (NN man))
  (VP (VBD saw)
      (NP (DT the) (NN dog))
      (PP (IN with) (NP (DT the) (NN telescope))))
  (. .))
```

**ASCII tree:**  
```
S
├── NP
│   ├── DT The
│   └── NN man
├── VP
│   ├── VBD saw
│   ├── NP
│   │   ├── DT the
│   │   └── NN dog
│   └── PP
│       ├── IN with
│       └── NP
│           ├── DT the
│           └── NN telescope
└── . .
```

### B) Modifier attachment to **NP** (“the dog with the telescope”)

**Bracketed notation:**  
```
(S
  (NP (DT The) (NN man))
  (VP (VBD saw)
      (NP
        (NP (DT the) (NN dog))
        (PP (IN with) (NP (DT the) (NN telescope)))))
  (. .))
```

**ASCII tree:**  
```
S
├── NP
│   ├── DT The
│   └── NN man
├── VP
│   ├── VBD saw
│   └── NP
│       ├── NP
│       │   ├── DT the
│       │   └── NN dog
│       └── PP
│           ├── IN with
│           └── NP
│               ├── DT the
│               └── NN telescope
└── . .
```

---

