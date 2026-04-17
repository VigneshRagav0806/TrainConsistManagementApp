## UC17: Sort Bogie Names Using Arrays.sort()

### Overview

This use case introduces Java's built-in sorting mechanism using Arrays.sort() to efficiently sort bogie names.

### Objective

To sort bogie type names alphabetically using Java’s optimized library function.

### Drawback of Previous Approach

In UC16, sorting was implemented manually using Bubble Sort, which is inefficient (O(n²)) and not suitable for real-world applications.

### Solution

Use Arrays.sort() for fast and reliable sorting.

### Flow of Execution

1. User provides bogie names
2. System calls Arrays.sort()
3. Java sorts the array internally
4. Sorted result is displayed

### Key Concepts Used

* **Arrays.sort()**

  * Built-in method for sorting arrays

* **Natural Ordering**

  * Strings sorted alphabetically

* **Time Complexity**

  * O(n log n)

* **Library Optimization**

  * Uses efficient internal algorithms

* **Readable Code**

  * Minimal and clean implementation

### Code Summary

* String array initialized
* Arrays.sort() applied
* Output displayed using Arrays.toString()

### Key Benefits

* Faster than manual sorting
* Cleaner and shorter code
* Reliable and optimized
* Suitable for real-world applications

### Output

```text id="uc17output02"
[AC Chair, First Class, General, Luxury, Sleeper]
```

### Conclusion

This use case demonstrates the transition from manual algorithm implementation to efficient use of built-in Java utilities for production-ready code.
