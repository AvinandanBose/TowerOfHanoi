Repository
👉 [https://github.com/AvinandanBose/TowerOfHanoi](https://github.com/AvinandanBose/TowerOfHanoi)

---

# 🗼 Tower of Hanoi

![GitHub repo size](https://img.shields.io/github/repo-size/AvinandanBose/TowerOfHanoi)
![GitHub stars](https://img.shields.io/github/stars/AvinandanBose/TowerOfHanoi?style=social)
![GitHub forks](https://img.shields.io/github/forks/AvinandanBose/TowerOfHanoi?style=social)
![GitHub issues](https://img.shields.io/github/issues/AvinandanBose/TowerOfHanoi)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📖 Overview

This repository provides a structured explanation and implementation of the **Tower of Hanoi** problem using recursion.

It is designed as a **learning-focused project** that explains:

* Recursive problem solving
* Recurrence relations
* Time & space complexity
* Step-by-step execution

---

## 📂 Repository Contents

Based on the uploaded materials, this repository includes:

* 📄 Concept notes explaining the Tower of Hanoi
* 📑 Step-by-step recursive breakdown
* 💻 Source code implementation (C/C++ style)
* 📊 Complexity analysis and recurrence relations
* 🧾 Supporting documentation / PDFs

---

## ⚙️ Problem Statement

You are given:

* Three rods: **Source (A), Auxiliary (B), Destination (C)**
* `n` disks of different sizes arranged in decreasing order

### 🎯 Objective

Move all disks from **Source → Destination**

---

## 📜 Rules

1. Only one disk can be moved at a time
2. Only the top disk can be moved
3. A larger disk cannot be placed on a smaller disk

---

## 🧠 Recursive Insight

The problem follows a **divide-and-conquer strategy**:

```
Step 1: Move (n-1) disks from A → B
Step 2: Move nth disk from A → C
Step 3: Move (n-1) disks from B → C
```

---

## 💻 Sample Implementation (C++)

```cpp
#include <iostream>
using namespace std;

void towerOfHanoi(int n, char source, char auxiliary, char destination)
{
    if (n == 1)
    {
        cout << "Move disk 1 from " << source << " to " << destination << endl;
        return;
    }

    towerOfHanoi(n - 1, source, destination, auxiliary);
    cout << "Move disk " << n << " from " << source << " to " << destination << endl;
    towerOfHanoi(n - 1, auxiliary, source, destination);
}

int main()
{
    int n = 3;
    towerOfHanoi(n, 'A', 'B', 'C');
    return 0;
}
```

---

## 📊 Recurrence Relation

```
T(n) = 2T(n - 1) + 1
T(1) = 1
```

### ✔️ Solution:

```
T(n) = 2^n - 1
```

---

## ⏱️ Complexity Analysis

| Type             | Complexity |
| ---------------- | ---------- |
| Time Complexity  | O(2ⁿ)      |
| Space Complexity | O(n)       |
| Total Moves      | 2ⁿ − 1     |

---

## 🔍 Explanation of Growth

* The number of recursive calls doubles at each level
* This results in **exponential growth**
* Even small increases in `n` significantly increase computation

---

## 🚀 How to Run

### 🧾 Requirements

* C++ Compiler (g++, clang, etc.)

### ▶️ Steps

```bash
g++ tower_of_hanoi.cpp -o hanoi
./hanoi
```

---

## 🎯 Learning Outcomes

After exploring this repository, you will understand:

* ✔️ Recursion and recursive trees
* ✔️ Stack depth and function calls
* ✔️ Recurrence relation solving
* ✔️ Exponential time complexity
* ✔️ Algorithmic thinking

---

## 📁 Suggested File Structure

```
TowerOfHanoi/
│── README.md
│── tower_of_hanoi.cpp
│── docs/
│   ├── introduction.pdf
│   ├── recursion_steps.pdf
│   ├── complexity_analysis.pdf
```


---

## ⭐ Support

If you find this repository helpful:

👉 Star the repo
👉 Share with others learning recursion

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

**Avinandan Bose**
- GitHub: [@AvinandanBose](https://github.com/AvinandanBose)

---
<br>
<br>
<br>
<h3><a href="https://github.com/AvinandanBose/CPLUSPLUS_DataStructure/blob/main/toh.cpp">𝑻𝒐𝒘𝒆𝒓 𝑶𝒇 𝑯𝒂𝒏𝒐𝒊 𝑷𝒓𝒐𝒈𝒓𝒂𝒎 𝒊𝒏 𝑪++ </a>  𝒊𝒏 <a href="https://github.com/AvinandanBose/CPLUSPLUS_DataStructure/">𝑪++ 𝑫𝒂𝒕𝒂 𝑺𝒕𝒓𝒖𝒄𝒕𝒖𝒓𝒆 𝑹𝒆𝒑𝒐</a></h3>
