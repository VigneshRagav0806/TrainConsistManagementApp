## UC3: Track Unique Bogie IDs (Set – HashSet)

### Overview

This use case introduces the concept of uniqueness in the Train Consist Management System by using a Set data structure to prevent duplicate bogie IDs.

### Objective

To ensure that no duplicate bogie IDs are stored in the system.

### Drawback of Previous Approach

In UC2, bogies were stored using a List, which allows duplicate entries. This could lead to multiple bogies having the same ID, causing inconsistencies in train management.

### Solution

Use a HashSet to automatically enforce uniqueness.

### Flow of Execution

1. User runs the program
2. Bogie IDs are added to the system
3. Duplicate IDs are intentionally inserted
4. HashSet automatically removes duplicates
5. Unique bogie IDs are displayed

### Key Concepts Used

* **Set Interface**

  * A collection that does not allow duplicate elements

* **HashSet**

  * Implementation of Set using hashing for fast access

* **add() Method**

  * Adds elements to the set
  * Ignores duplicates automatically

* **Automatic Deduplication**

  * No manual checking required for duplicates

* **Unordered Storage**

  * Elements are not stored in insertion order

### Code Summary

* A HashSet is created to store bogie IDs
* Duplicate IDs are added intentionally
* HashSet filters out duplicates automatically
* Final set contains only unique values

### Key Benefits

* Enforces real-world business rules (unique IDs)
* Prevents data duplication and corruption
* Improves data integrity
* Demonstrates when to use Set instead of List

### Output

```text id="uc3output02"
=== Train Consist Management App ===

Bogie IDs in the Train (Unique Only):
[BG101, BG102, BG103]

Total unique bogies: 3
```

### Conclusion

This use case strengthens the system by ensuring data uniqueness, a critical requirement in real-world applications like railway management systems.
