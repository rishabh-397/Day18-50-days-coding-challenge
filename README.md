# Day18-50-days-coding-challenge
## 🔹 Problem 1: Implement Queue using Stacks

### Problem Statement:
Implement a **FIFO Queue** using two stacks. Support the following operations:
- `push(int x)` – Add element to the back.
- `pop()` – Remove and return front element.
- `peek()` – Get the front element.
- `empty()` – Check if the queue is empty.

### ✅ Constraints:
- Use only standard stack operations (push to top, pop from top, etc.).
- Up to 100 operations allowed.
- All calls to `pop` and `peek` are valid.

### 💡 Approach:
Use two stacks:
- `in_stack` for enqueue (`push`)
- `out_stack` for dequeue (`pop` and `peek`)
Transfer elements only when needed for efficient amortized O(1) performance.

---

## 🔹 Problem 2: Contains Duplicate

### Problem Statement:
Given an array `nums`, return `true` if any value appears **at least twice**; otherwise, return `false`.

### ✅ Examples:
```plaintext
Input: nums = [1,2,3,1]    → Output: true
Input: nums = [1,2,3,4]    → Output: false
Input: nums = [1,1,1,3,3]  → Output: true
💡 Approach:
Use a set to store seen elements while traversing.

If an element is already in the set, return true.

Else, continue and return false at the end.
