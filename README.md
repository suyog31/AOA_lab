# Analysis of Algorithms (AOA) Lab

This repository contains lab assignments and implementations for the Analysis of Algorithms (AOA) course.

## Contents

- **Lab 1**: Implementation of Iterative and Numeric Algorithms
  - Contains detailed implementations in Python using Jupyter Notebook (`1.ipynb`).
  - Algorithms covered:
    1. GCD (Euclid's Algorithm)
    2. Fibonacci Series
    3. Sequential Search
    4. Bubble Sort
    5. Insertion Sort
    6. Selection Sort
    7. Chinese Remainder Theorem (CRT)
    8. Fermat's Primality Test
    9. Miller-Rabin Test

---

## 📊 Flowcharts

*(Note: GitHub's built-in Jupyter viewer does not render Mermaid flowcharts inside `.ipynb` files. They are provided here for easy viewing).*

### GCD (Euclidean Algorithm) Flowchart
```mermaid
graph TD
    Start([Start]) --> Input[/"Input a, b"/]
    Input --> Cond{"b == 0?"}
    Cond -- Yes --> Out[/"Output a"/]
    Cond -- No --> Calc["temp = a % b<br/>a = b<br/>b = temp"]
    Calc --> Cond
    Out --> Stop([Stop])
```

### Bubble Sort Flowchart (Conceptual)
```mermaid
graph TD
    Start([Start]) --> Input[/"Input Array A of size N"/]
    Input --> LoopI["For i from 0 to N-1"]
    LoopI --> LoopJ["For j from 0 to N-i-1"]
    LoopJ --> Cond{"A[j] > A[j+1]?"}
    Cond -- Yes --> Swap["Swap A[j] and A[j+1]"]
    Cond -- No --> NextJ["Next j"]
    Swap --> NextJ
    NextJ --> LoopJ
    LoopJ -. "Loop J Ends" .-> NextI["Next i"]
    NextI --> LoopI
    LoopI -. "Loop I Ends" .-> Out[/"Output Sorted A"/]
    Out --> Stop([Stop])
```

---

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/suyog31/AOA_Lab.git
   cd AOA_Lab
   ```

2. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook lab1/1.ipynb
   ```
