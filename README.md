# Quantum-Native Python

### Quantum Thinking in Classical Code

> **"The wall between Classical and Quantum computing is artificial. It exists only because we usually restrict our software to integers."**

This repository demonstrates that "Quantum" principles—Superposition, Wave Collapse, and Entanglement—are not magical properties of exotic hardware. They are fundamental mathematical concepts (Linear Algebra & Probability) that can be implemented and understood in standard Python.

We do not need a cryogenically cooled chandelier to think in Quantum. We just need to stop thinking in `0` and `1` and start thinking in **Vectors**.

---

## 📂 The Project: `Quantum-Native-Python.ipynb`

This repository contains a single, self-contained Jupyter Notebook that breaks down the barrier between classical logic and quantum logic through two specific experiments using **NumPy**.

### 1. Differentiable Gates: Logic is Geometry
**The Concept:**
In standard computer science, logic is Boolean: `True` is `1`, `False` is `0`.
In this project, we define a bit not as a number, but as a **vector on a circle**:
*   **State 0 (False):** 0° Rotation.
*   **State 1 (True):** 90° Rotation.
*   **Superposition:** Any angle in between.

**The Experiment:**
We do not hard-code logic gates (like `NOT` or `AND`). Instead, we use **Differentiable Programming** (Gradient Descent). We give the code a target (e.g., "Output a 50% probability of 1") and let the gate *learn* the correct rotation to achieve it.

**The Result:**
The code successfully learns to create a "Hadamard Gate" (Superposition) purely by minimizing error, proving that quantum states are just specific angles of geometry.

### 2. Entanglement: High-Dimensional Correlation
**The Concept:**
Entanglement is often described as "spooky action at a distance." This experiment demystifies it by showing that entanglement is simply **High-Dimensional Correlation**.
*   We treat two bits not as two separate objects, but as **a single point in 4-dimensional space**.
*   By manipulating this 4D vector, we mathematically delete the possibility of the bits disagreeing (e.g., removing the `01` and `10` states).

**The Result:**
When we measure the system, the bits behave randomly, yet identically:
```text
Sample 1: Measured 00 | Correlation: PERFECT MATCH
Sample 2: Measured 11 | Correlation: PERFECT MATCH
Sample 3: Measured 00 | Correlation: PERFECT MATCH
...
```
Even though both bits are random, they are random *together*. There is no "signal" sent between them—just shared geometry.

---

## 🧠 Philosophy

Standard computing limits us to the **corners of the hypercube** (0 and 1). Quantum computing explores the **volume inside**.

By switching our mathematical view from integers to vectors, we realize that "Classical" and "Quantum" are not different universes. Classical computing is simply a subset of Quantum computing where we are restricted to 90-degree turns.

This project allows you to explore that volume using nothing but Python and Math, proving that **Quantum Logic is a software architecture, not just a hardware state.**

---

## 🚀 How to Run

1. Open `Quantum-Native-Python.ipynb` in [Google Colab](https://colab.research.google.com/) or Jupyter.
2. Run the cells to watch the **Gradient Descent** learn a quantum gate in real-time.
3. Run the **Entanglement** simulation to observe the correlation statistics.
4. **Dependencies:** `numpy` (That's it. No quantum simulators required).
