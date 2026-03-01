# Chapter 3: Algorithms 

> "An algorithm is a finite sequence of precise instructions for performing a computation or solving a problem." — **Kenneth H. Rosen**

##  Overview
This directory serves as the computational implementation of **Chapter 3** from our study of Discrete Mathematics. Here, we transition from static mathematical structures (Sets and Functions) to dynamic processes. The goal is to implement, analyze, and verify the efficiency of various algorithmic strategies.

---

## Implemented Modules

### 1. Searching Algorithms (`searching.py`)
Searching is the process of locating an element $x$ in a list of distinct elements. 
* **Linear Search:** A brute-force approach that examines each element sequentially. 
    * **Complexity:** $O(n)$
* **Binary Search:** A "Divide and Conquer" strategy that requires a **pre-sorted list**. It repeatedly ignores half of the search interval.
    * **Complexity:** $O(\log n)$



### 2. Sorting Algorithms (`sorting.py`)
Sorting is a fundamental prerequisite for many optimized algorithms. We implement two classic **quadratic** sorting methods to practice in-place array manipulation.
* **Bubble Sort:** Compares adjacent elements and swaps them if they are in the wrong order. The largest values "bubble" to their correct position at the end of the list.
* **Insertion Sort:** Iteratively builds a sorted portion of the array by taking the next element and "inserting" it into its correct relative position.



### 3. Greedy Algorithms (`greedy.py`)
A **Greedy Algorithm** makes the simplest, most "locally optimal" choice at each step with the intent of reaching a global optimum.
* **The Change-Making Problem:** Minimizing the total number of coins used to provide a specific value $V$.
* **Note:** While effective for standard currency (quarters, dimes, etc.), greedy algorithms do not always yield the optimal solution for arbitrary denominations.



### 4. Complexity & Big-O Analysis (`complexity.py`)
This module provides a benchmarking suite to visualize the growth rate of our algorithms.
* **Big-O Notation ($O$):** Used to provide an upper bound on the growth of an algorithm's execution time or space requirements as the input size $n$ increases.



---

## Programming Objectives
1.  **Mathematical Accuracy:** Ensure the code strictly follows the logical definitions provided in the text.
2.  **Efficiency Awareness:** Use Python's `time` module to empirically observe the performance gap between $O(n^2)$ and $O(n \log n)$ implementations.
3.  **In-place Logic:** Practice memory efficiency by modifying lists directly when implementing sorting algorithms.
4.  **Verification:** Every algorithm is tested against Python’s native functions (e.g., `sorted()` or `in` operator) to confirm zero logic-regression.