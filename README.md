## UC16: Sort Passenger Bogies by Capacity (Bubble Sort – Algorithm Intro)

### Overview

This use case introduces manual sorting using the Bubble Sort algorithm to help understand how sorting works internally.

### Objective

To sort passenger bogie capacities using a basic comparison-based algorithm without using built-in methods.

### Drawback of Previous Approach

Earlier use cases relied on library functions like Comparator and Streams, which hide the internal working of sorting algorithms.

### Solution

Implement Bubble Sort manually using nested loops and swapping logic.

### Flow of Execution

1. User provides bogie capacities
2. System iterates through the array
3. Adjacent elements are compared
4. If out of order, elements are swapped
5. Multiple passes ensure sorting
6. Sorted result is displayed

### Key Concepts Used

* **Bubble Sort Algorithm**

  * Repeatedly compares and swaps adjacent elements

* **Array Manipulation**

  * Direct index-based access

* **Nested Loops**

  * Outer loop for passes, inner loop for comparisons

* **Swapping Logic**

  * Uses temporary variable

* **Time Complexity**

  * O(n²) for worst and average cases

### Code Summary

* Array of capacities initialized
* Nested loops applied
* Adjacent elements compared and swapped
* Final sorted array printed

### Key Benefits

* Builds algorithmic understanding
* Strengthens logic building skills
* Prepares for advanced sorting techniques
* Bridges theory and implementation

### Output

```text id="uc16output02"
Sorted Capacities (Ascending): 24 56 60 70 72
```

### Conclusion

This use case demonstrates how sorting works internally, providing a strong foundation before using optimized library methods.
