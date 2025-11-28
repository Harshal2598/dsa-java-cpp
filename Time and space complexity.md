# Resource for Learning Time and Space Complexity

▶ **Video Link:** https://www.youtube.com/watch?v=FPu9Uld7W-E  
This video explains Time Complexity and Space Complexity in the context of **coding interviews** and **problem-solving**.

Below is a clean summary of the key concepts.

---

# 📌 Summary of Key Points

## 1️⃣ What is Time Complexity?
- It is **not actual runtime in seconds**, because execution time depends on the machine.
- Instead, it measures **how fast the runtime grows as input size increases**.  
  *(Timestamp: 3:46)*

---

## 2️⃣ Why is Time Complexity Important?
- Interviewers **cannot run your code**; instead, they evaluate its **efficiency theoretically**.  
  *(Timestamp: 1:16)*

---

## 3️⃣ Big O Notation
Time complexity is expressed using **Big O notation**, such as:

- **O(1)**  
- **O(n)**  
- **O(n²)**  
- **O(log n)**  

Big O gives a machine-independent performance comparison.  
*(Timestamp: 6:11)*

---

## 4️⃣ Rules for Computing Big O

### ✔ Always consider the **worst-case**  
E.g., searching in an unsorted array.  
*(10:40)*

### ✔ Ignore constants  
`O(2n)` → **O(n)**  
*(14:05)*

### ✔ Ignore lower-order terms  
`O(n² + n)` → **O(n²)**  
*(16:23)*

---

## 5️⃣ Space Complexity
Space Complexity refers to the **memory** an algorithm uses.  
*(Timestamp: 26:00)*

It includes:

- **Input space** → memory to store input  
- **Auxiliary space** → extra memory used inside the algorithm  
*(26:50)*

---

## 6️⃣ Important Rule for Space Complexity
- **Do NOT modify input arrays/strings unless the interviewer allows it.**  
It’s considered a bad practice in software engineering.  
*(Timestamp: 30:26)*

---

## 7️⃣ Competitive Programming Insight
Most competitive programming servers can execute:

### **≈ 10⁸ (100 million) operations per second**  
*(Timestamp: 32:39)*

This helps determine if your code will pass within time limits.

Example:
- **O(n²)** might fail for n = 10⁵  
- **O(n log n)** will pass for large n  
- **O(n)** and **O(1)** always safe

---

# ⭐ Final Notes
This video provides a strong foundation on:

- Time Complexity  
- Space Complexity  
- Big O rules  
- Recursion complexity  
- Competitive programming constraints  

Highly recommended for anyone preparing for **coding interviews**, **DSA**, or **competitive programming**.


# Time and Space Complexity

Time and Space Complexity are two important concepts in Data Structures and Algorithms (DSA).  
They help measure **how efficient** an algorithm is in terms of **execution time** and **memory usage**.

---

# 1️⃣ Time Complexity

Time Complexity tells **how much time an algorithm takes to run** based on the input size **n**.

It does NOT calculate actual time (seconds).  
Instead, it measures how the number of operations grows as the input grows.

---

## ✔ Big-O Notation (Most Common)

Big-O describes the **upper bound** of the algorithm.

| Complexity | Name | Meaning |
|------------|------|----------|
| O(1) | Constant | Fastest, independent of input size |
| O(log n) | Logarithmic | Grows very slowly |
| O(n) | Linear | Grows proportionally with input |
| O(n log n) | Linearithmic | Efficient sorting |
| O(n²) | Quadratic | Slow for large inputs |
| O(2ⁿ) | Exponential | Very slow |
| O(n!) | Factorial | Extremely slow |

---

## ✔ Examples of Time Complexity

### 🔹 O(1) – Constant Time
```cpp
int getFirst(int arr[]) {
    return arr[0];
}
```

### 🔹 O(n) – Linear Time
```cpp
for (int i = 0; i < n; i++) {
    cout << arr[i];
}
```

### 🔹 O(n²) – Quadratic Time
```cpp
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
        cout << i << j;
    }
}
```

---

# 2️⃣ Space Complexity

Space Complexity tells **how much extra memory** an algorithm needs.

It includes:
- Input space  
- Auxiliary space (extra variables, arrays, recursion stack)

---

## ✔ Examples of Space Complexity

### 🔹 O(1) – Constant Space
```cpp
int sum = 0; // only one variable
```

### 🔹 O(n) – Linear Space
```cpp
int arr[n]; // array of size n
```

### 🔹 Space used by Recursion (Call Stack)
```cpp
int fact(int n) {
    if (n == 1) return 1;
    return n * fact(n-1); // recursion depth = n
}
```
This uses **O(n)** space.

---

# ⭐ Difference Between Time and Space Complexity

| Feature | Time Complexity | Space Complexity |
|---------|------------------|------------------|
| Measures | Execution time | Memory usage |
| Affected by | Loops, recursion | Variables, arrays, recursion stack |
| Goal | Reduce time | Reduce memory |
| Example | O(n²) | O(n) |

---

# ⭐ Why Time & Space Complexity Matters?

- Helps choose the **best algorithm**
- Shows how code performs on **large inputs**
- Crucial for **DSA, competitive coding, interviews**
- Avoids slow and memory-heavy programs

---

# 🎯 Conclusion

Time and Space Complexity help evaluate how efficient an algorithm is.  
Good algorithms should use:
- **Minimum time**  
- **Minimum memory**  

Understanding complexities is essential for writing **optimized and scalable** programs.

