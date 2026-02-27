# 🧠 D. Unnatural Language Processing

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Codeforces-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Greedy-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Strings%20%26%20Parsing-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Time%20Limit-1s-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Space%20Limit-256MB-purple?style=for-the-badge"/>
</p>

---

## 📌 [Problem Statement](https://codeforces.com/problemset/problem/1915/D)

Lura created a simple artificial language using only five letters:
a, b, c, d, e


### 🔤 Letter Types

- **Vowels (V)** → `a`, `e`
- **Consonants (C)** → `b`, `c`, `d`

---

## 🗣️ Syllable Rules

There are two valid syllable types:

1. **CV** → consonant followed by vowel  
2. **CVC** → consonant, vowel, consonant  

Examples of valid syllables:

ba
ced
bab


Invalid examples:

aa
eda
baba


---

## 🎯 Task

A word in this language is a sequence of valid syllables.

You are given a valid word but without syllable boundaries.

Your task is to split the word into valid syllables by inserting:


.


between every pair of adjacent syllables.

If multiple splittings are possible, output **any** valid one.

It is guaranteed that:
- Every word is valid
- At least one valid splitting exists

---

## 📥 Input

- First line:

t (1 ≤ t ≤ 100)

— number of test cases

For each test case:

- Integer:

n (1 ≤ n ≤ 2 × 10^5)

— length of the word

- String of length `n` consisting only of:

a, b, c, d, e


Constraint:
- Sum of `n` over all test cases ≤ `2 × 10^5`

---

## 📤 Output

For each test case, print the word with `.` inserted between syllables.

---

## 🧾 Example

### 🔹 Input

6 </br>
8 </br>
bacedbab </br>
4 </br>
baba </br>
13 </br>
daddecabeddad </br>
3 </br>
dac </br>
6 </br>
dacdac </br>
22 </br>
dababbabababbabbababba </br>


### 🔹 Output

ba.ced.bab </br>
ba.ba </br>
dad.de.ca.bed.dad </br>
dac </br>
dac.dac </br>
da.bab.ba.ba.bab.bab.ba.bab.ba </br>


---

## 🏷️ Tags

- Greedy
- Strings
- Pattern Recognition
- Implementation
- Parsing

---

## 🎯 Category & Difficulty

- **Type:** Greedy + String Parsing  
- **Difficulty Level:** ~1400–1600 (Div2 D)

---

> 💡 Key idea:  
> Every syllable starts with a consonant.  
> Decide whether to form `CV` or `CVC` greedily while scanning the string.
