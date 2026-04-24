# 3-Coloring Interactive Visualizer

Interactive educational web tool for understanding **Graph 3-Coloring**, **Greedy Coloring**, **Exact Backtracking 3-Coloring**, and the **NP-Completeness proof via reduction from 3-SAT** step-by-step.

Developed for **BCS 309 – Algorithms I** as a web-based teaching and visualization project.

---

## Project Purpose

This tool helps students:

- understand the Graph 3-Coloring problem
- visualize graph coloring step-by-step
- compare heuristic and exact algorithm approaches
- understand NP-completeness
- understand reduction from 3-SAT
- explore algorithm complexity and performance

The visualization transforms abstract algorithm concepts into a clear and intuitive learning experience.

---

## Algorithms Included

### 1. Greedy Coloring

Assigns the smallest available color to each vertex based on a selected ordering.

Formula:

Choose the smallest available color not used by adjacent vertices.

Time Complexity:

O(V + E)

Characteristics:

- fast and simple
- depends on vertex ordering
- may use more than 3 colors
- not guaranteed to find the optimal coloring

---

### 2. Exact Backtracking 3-Coloring

Recursively tries colors and backtracks when conflicts occur.

Formula:

Try colors {1, 2, 3} recursively and backtrack when invalid.

Time Complexity:

O(3^V) worst case

Characteristics:

- exact algorithm
- determines whether a valid 3-coloring exists
- guarantees correct result
- expensive for large graphs

---

## NP-Completeness / Reduction

This tool demonstrates why **Graph 3-Coloring** is NP-complete.

### 1. 3-Coloring is in NP

A proposed coloring acts as a **certificate**.

A **verifier** checks every edge to ensure adjacent vertices have different colors.

Verification takes polynomial time:

O(E)

---

### 2. Reduction from 3-SAT

The tool demonstrates a polynomial-time reduction from **3-SAT** to **3-Coloring**.

It includes visual explanations of the following gadgets:

- **Truth Gadget**  
  Forces three distinct colors: True, False, and Base.

- **Variable Gadget**  
  Ensures a variable and its negation receive opposite truth colors.

- **Clause Gadget**  
  Simulates the OR condition so at least one literal must be True.

The constructed graph is **3-colorable if and only if** the original Boolean formula is satisfiable.

---

## Features

- step-by-step graph coloring visualization
- interactive graph building
- preset graph examples
- custom graph input
- random graph generation
- side-by-side comparison mode
- pseudocode with line highlighting
- step explanation box
- live statistics panel
- complexity estimate panel
- reduction animation
- gadget explanation section
- performance comparison charts
- playback controls:
  - Build Steps
  - Step
  - Play
  - Pause
  - Reset
- responsive dark-theme UI

---

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6)
- SVG for graph rendering and animations

No external libraries or frameworks were used.

---

## How to Run

Open locally:

open the file  
index.html

Or use the GitHub Pages version:

https://boutchitmn.github.io/3-Coloring-Visualizer/

No installation required.

---

## Educational Focus

This project demonstrates:

- Greedy paradigm
- Backtracking paradigm
- NP-completeness
- polynomial-time reduction
- algorithm complexity analysis
- effect of vertex ordering
- heuristic vs exact comparison

---

## Course Information

Course: BCS 309 – Algorithms I  
Instructor: Dr. Arash Kermani Kolankeh  
University: Canadian University Dubai  

Semester: Spring 2026  

Student: Bouchina, Othmane  
Student ID: 20220001467  

---

## Notes

This project is intended for educational purposes to help students better understand graph coloring and NP-complete problems through visualization.
