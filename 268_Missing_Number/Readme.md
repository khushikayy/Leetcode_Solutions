# Missing Number (Java)

A simple and efficient Java solution for the **Missing Number** problem using the mathematical sum formula.

## 📌 Problem Statement

Given an array `nums` containing `n` distinct numbers in the range **[0, n]**, return the only number in the range that is missing.

### Link 
https://leetcode.com/problems/missing-number/description/?envType=problem-list-v2&envId=array
---

### Example 1

**Input**
```text
nums = [3,0,1]
```

**Output**
```text
2
```

### Example 2

**Input**
```text
nums = [0,1]
```

**Output**
```text
2
```

### Example 3

**Input**
```text
nums = [9,6,4,2,3,5,7,0,1]
```

**Output**
```text
8
```

---

## 💡 Approach

The solution uses the **Mathematical Sum Formula**.

1. Calculate the expected sum of numbers from **0 to n** using:

   ```
   n × (n + 1) / 2
   ```

2. Calculate the actual sum of all elements in the array.

3. The missing number is:

   ```
   Missing Number = Expected Sum − Actual Sum
   ```

This approach avoids sorting and extra memory, making it highly efficient.

---

## 🧮 Algorithm

1. Let `n` be the length of the array.
2. Compute the expected sum:
   ```
   expected = n * (n + 1) / 2
   ```
3. Traverse the array and compute the actual sum.
4. Return:
   ```
   expected - actual
   ```

---

## ⏱️ Complexity Analysis

| Complexity | Value |
|------------|-------|
| Time Complexity | **O(n)** |
| Space Complexity | **O(1)** |

---

## 💻 Java Solution

```java
class Solution {
    public int missingNumber(int[] nums) {
        int n = nums.length;
        int expected = n * (n + 1) / 2;
        int actual = 0;

        for (int num : nums) {
            actual += num;
        }

        return expected - actual;
    }
}
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/MissingNumber.git
```

2. Navigate to the project directory:

```bash
cd MissingNumber
```

3. Compile the Java file:

```bash
javac Main.java
```

4. Run the program:

```bash
java Main
```

---

## 📂 Project Structure

```
MissingNumber/
│── Main.java
│── README.md
```

---

## 🚀 Features

- Efficient mathematical approach
- Linear time complexity **O(n)**
- Constant space complexity **O(1)**
- Beginner-friendly implementation
- Clean and well-documented code

---

## 🏷️ Topics

- Java
- Arrays
- Mathematics
- Algorithms
- Data Structures
- LeetCode
- Interview Preparation

---

## 👨‍💻 Author

**Your Name**

GitHub: https://github.com/your-username

---

## ⭐ Support

If you found this project helpful, consider giving it a **⭐ Star** on GitHub.