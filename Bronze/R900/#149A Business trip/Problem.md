# 🏢 A. Business Trip

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Codeforces-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Rank-900-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Greedy-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Sorting-purple?style=for-the-badge"/>
</p>

---

## 📌 [Problem Statement (on CodeForces)](https://codeforces.com/problemset/problem/149/A)

What joy! Petya's parents went on a business trip for the whole year and the playful kid is left all by himself.

Petya discovered that his parents left him with an important responsibility:

He must water their favorite flower **every month**.  

He knows that:

- If he fulfills the task in the `i-th` month (1 ≤ i ≤ 12),  
  the flower will grow by `aᵢ` centimeters.
- If he does not water the flower in that month,  
  the flower will not grow at all during that month.

However, Petya also knows that:

His parents will only believe him if the flower grows **at least `k` centimeters** in total.

---

## 🎯 Objective

Help Petya determine the **minimum number of months** he must water the flower so that the total growth is:
≥ k centimeters


If it is impossible to reach `k` centimeters within the year, print:


-1


---

## 📥 Input

- The first line contains an integer:

k (0 ≤ k ≤ 100)
- The second line contains 12 space-separated integers:

a₁ a₂ a₃ ... a₁₂

where:

0 ≤ aᵢ ≤ 100
---

## 📤 Output

Print a single integer:

- The **minimum number of months** required to achieve total growth ≥ `k`.
- Print `-1` if it is impossible.

---

## 🧾 Examples

---

### 🟢 Example 1

**Input**

5
1 1 1 1 2 2 3 2 2 1 1 1
**Output**

2


**Explanation**

Watering during the 7th and 9th months gives:


3 + 2 = 5


This satisfies the requirement.

---

### 🟢 Example 2

**Input**

0
0 0 0 0 0 0 0 1 1 2 3 0
**Output**

0


**Explanation**

Since `k = 0`, the flower does not need to grow at all.  
Petya does not need to water the flower.

---

### 🟢 Example 3

**Input**

11
1 1 4 1 1 5 1 1 4 1 1 1


**Output**
3

---

## 📎 Constraints

- Exactly 12 months
- `0 ≤ k ≤ 100`
- `0 ≤ aᵢ ≤ 100`

---

## 🏷️ Tags

- Greedy
- Sorting
- Implementation
- Simulation

---

> 💡 This is a classic greedy problem where selecting the largest growth months first minimizes the number of selections.
