

## 🌡️ Sensor Data Range Filter using Binary Search Tree (BST)

This project implements a simple **Binary Search Tree (BST)** structure in Python to store sensor readings indexed by timestamp. It provides a recursive method to retrieve all sensor readings that fall within a specified time range.

---

### ✅ Key Features

* **Binary Tree Node Structure**: Each node contains a timestamp and its corresponding sensor reading.
* **Recursive Range Search**: Efficiently traverses the BST to retrieve readings whose timestamps lie within a user-defined inclusive range.
* **Sorted Output**: Ensures readings are returned in ascending order of their timestamps.
* **Tree-Based Filtering**: Demonstrates the use of tree traversal (in-order logic) to filter time-based data.

---

### 🧠 How It Works

1. A binary search tree is constructed with nodes containing both a timestamp and a sensor reading label.
2. The function `get_readings_in_range()` is called with a start and end time.
3. It recursively:

   * Traverses the left subtree for timestamps less than the current node.
   * Traverses the right subtree for timestamps greater than the current node.
   * Appends readings within the `[start_time, end_time]` range to a result list.
4. The matched timestamps are mapped back to their original readings using a dictionary.

---

### 📦 Sample Output

For the given BST structure and time range `[10, 15]`, the program outputs:

```python
Readings within range: ['Reading-10', 'Reading-12', 'Reading-15']
```

---

### 🌳 Sample Tree Structure

```
         10
       /    \
      5      15
            /  \
          12    20
```

---

### 🛠️ Tech Stack

* **Language**: Python 3
* **Data Structures**: Custom binary search tree
* **Concepts**: Tree traversal, range query, recursion, data filtering

---
