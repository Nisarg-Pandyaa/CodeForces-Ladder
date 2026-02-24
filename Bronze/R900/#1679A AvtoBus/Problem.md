# 🚌 A. AvtoBus

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Codeforces-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Rank-900-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Math-purple?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Greedy-orange?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

Spring has come, and the management of the **AvtoBus** fleet has ordered to replace winter tires with summer tires on all buses.

You own a small bus service business and have received an order to replace `n` tires.

The fleet owns two types of buses:

- 🟢 **Two-axle buses** → 4 wheels  
- 🔵 **Three-axle buses** → 6 wheels  

You do **not** know how many buses of each type exist.

Your task is to determine:

- The **minimum number of buses**
- The **maximum number of buses**

such that the total number of wheels equals `n`.

---

## 🎯 Objective

For each test case:

- Print two integers `x` and `y`  
  where:
  x = minimum possible number of buses
  y = maximum possible number of buses

- If no valid configuration exists, print:

-1
---

## 📥 Input

- First line contains integer:

t (1 ≤ t ≤ 1000)

— number of test cases.

- Each test case contains one integer:

n (1 ≤ n ≤ 10^18)
— total number of wheels.

---

## 📤 Output

For each test case:

- Print `x y` if possible  
- Otherwise print `-1`

---

## 🧾 Example

### 🔹 Input

4 </br>
4 </br>
7 </br>
24 </br>
998244353998244352 </br>


### 🔹 Output

1 1 </br>
-1  </br>
4 6 </br> 
166374058999707392 249561088499561088


---

## 🧠 Explanation

### 🟢 Test Case 1

`n = 4`

Only possible configuration:
- 1 two-axle bus (4 wheels)

Output:

1 1


---

### 🟢 Test Case 2

`n = 7`

No combination of 4s and 6s can produce 7.

Output:

-1


---

### 🟢 Test Case 3

`n = 24`

Possible configurations:

- 4 buses with 6 wheels → 4 buses  
- 3 buses (4 wheels) + 2 buses (6 wheels) → 5 buses  
- 6 buses with 4 wheels → 6 buses  

Minimum buses = 4  
Maximum buses = 6  

Output:

4 6

---

## 📎 Constraints

- `1 ≤ t ≤ 1000`
- `1 ≤ n ≤ 10^18`
- Each bus contributes either 4 or 6 wheels.

---

## 🏷️ Tags

- Mathematics
- Greedy
- Number Theory
- Implementation
- Competitive Programming

---

> 💡 This is a mathematical reasoning problem involving combinations of fixed wheel counts.
