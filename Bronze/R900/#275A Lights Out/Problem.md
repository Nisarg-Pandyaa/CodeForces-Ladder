# 💡 A. Lights Out

<p align="center">
  <img src="https://img.shields.io/badge/Time%20Limit-2s-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Memory%20Limit-256MB-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Simulation/Implementation-purple?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Simulation%20%26%20Matrix-orange?style=for-the-badge"/>
</p>

---

## 📌 [Problem Statement (on CodeForces)](https://codeforces.com/problemset/problem/275/A)

Lenny is playing a game on a **3 × 3 grid of lights**.

At the beginning:
- All lights are **switched on**.

Pressing any light will:
- Toggle the selected light
- Toggle all **side-adjacent lights** (up, down, left, right)

### 🔄 Toggle Rule

- If a light is **ON (1)** → it becomes **OFF (0)**
- If a light is **OFF (0)** → it becomes **ON (1)**

Lenny has pressed each light a certain number of times.

Your task is to determine the **final state of the grid**.

---

## 📥 Input

- The input consists of **3 rows**
- Each row contains **3 integers** (0 to 100 inclusive)
- The `j-th` number in the `i-th` row represents how many times that light was pressed

---

## 📤 Output

Print **3 lines**, each containing **3 characters**:

- Print `"1"` if the light is ON
- Print `"0"` if the light is OFF

---

## 🧾 Example 1

### 🔹 Input
1 0 0 </br>
0 0 0 </br>
0 0 1 </br>


### 🔹 Output

001 </br>
010 </br>
100 </br>


---

## 🧾 Example 2

### 🔹 Input

1 0 1 </br>
8 8 8 </br>
2 0 3 </br>


### 🔹 Output

010 </br>
011 </br>
100 </br>

---

## 📎 Constraints

- Grid size is fixed: `3 × 3`
- Each press count: `0 ≤ value ≤ 100`

---

## 🏷️ Tags

- Implementation
- Simulation
- Matrix
- Brute Force
- Parity Logic

---

> 💡 Key Insight:  
> Since toggling twice cancels out, only whether the number of presses is **odd or even** matters.
