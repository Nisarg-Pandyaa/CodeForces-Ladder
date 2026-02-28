# ⚔️ A. Oath of the Night's Watch

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Codeforces-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Greedy-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Arrays%20%26%20Sorting-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Time%20Limit-2s-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Space%20Limit-256MB-purple?style=for-the-badge"/>
</p>

---

## 📌 [Problem Statement](https://codeforces.com/problemset/problem/768/A)

Jon Snow has been assigned to support `n` stewards.  
Each steward has a certain **strength**.

Jon will support a steward **only if**:

- There exists **at least one steward with strength strictly less** than him, and  
- There exists **at least one steward with strength strictly greater** than him.

Your task is to determine how many stewards Jon will support.

---

## 📥 Input

- First line:  
  `n` (1 ≤ n ≤ 10^5) — number of stewards  

- Second line:  
  `a₁ a₂ ... aₙ`  
  (0 ≤ aᵢ ≤ 10^9) — strengths of the stewards  

---

## 📤 Output

Print a single integer —  
the number of stewards Jon will support.

---

## 🧾 Examples

### Example 1

**Input**

2
1 5


**Output**

0


**Explanation**

- Steward with strength `1` has no strictly smaller steward.
- Steward with strength `5` has no strictly greater steward.

So Jon supports none.

---

### Example 2

**Input**

3
1 2 5


**Output**

1


**Explanation**

- Steward with strength `2` has:
  - `1` (strictly smaller)
  - `5` (strictly greater)

So Jon supports exactly one steward.

---
