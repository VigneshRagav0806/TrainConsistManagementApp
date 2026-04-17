## UC18: Linear Search for Bogie ID (Array-Based Searching)

### Overview

This use case introduces Linear Search to locate a specific bogie ID in an unsorted list.

### Objective

To search for a bogie ID by traversing the array sequentially.

### Drawback of Previous Approach

In UC17, data was sorted, but there was no way to locate a specific bogie quickly.

### Solution

Use Linear Search to check each element until a match is found.

### Flow of Execution

1. User provides bogie ID to search
2. System traverses array sequentially
3. Each element is compared using equals()
4. If match found → search stops
5. Result is displayed

### Key Concepts Used

* **Linear Search**

  * Sequential search technique

* **Sequential Traversal**

  * Checks elements one by one

* **equals() Method**

  * Safe string comparison

* **Early Termination**

  * Stops when match is found

* **Unsorted Data Handling**

  * Works without sorting

### Code Summary

* Array of bogie IDs created
* User input taken
* Loop iterates through array
* Match checked using equals()
* Result displayed

### Key Benefits

* Simple and easy to implement
* Works on unsorted data
* Builds search fundamentals
* Prepares for optimized search algorithms

### Output

```text id="uc18output03"
Bogie found at position: 2
```

### Conclusion

This use case introduces fundamental searching logic, enabling the system to locate specific bogies efficiently.
