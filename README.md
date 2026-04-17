## UC7: Sort Bogies by Capacity (Comparator)

### Overview

This use case introduces sorting of bogies based on seating capacity using the Comparator interface, enabling better planning and analysis.

### Objective

To arrange passenger bogies in ascending order of capacity using custom comparison logic.

### Drawback of Previous Approach

In UC6, bogies were mapped to capacities but lacked ordering. This made it difficult to compare and prioritize bogies for operational planning.

### Solution

Use Comparator to define custom sorting logic based on bogie capacity.

### Flow of Execution

1. User runs the program
2. Bogie objects are created
3. Bogies are stored in a List
4. Comparator is applied to sort based on capacity
5. Sorted bogies are displayed

### Key Concepts Used

* **Comparator Interface**

  * Defines custom sorting logic

* **Custom Objects**

  * Bogies represented as objects with name and capacity

* **List Collection**

  * Stores multiple bogie objects dynamically

* **sort() Method**

  * Sorts elements using Comparator

* **Lambda Expressions**

  * Provides concise sorting logic

* **Separation of Data and Logic**

  * Keeps data structure independent from sorting behavior

### Code Summary

* Bogie class created with name and capacity
* List<Bogie> used to store objects
* Bogies added: Sleeper (72), AC Chair (56), First Class (24)
* Sorted using Comparator.comparingInt()
* Displayed before and after sorting

### Key Benefits

* Enables capacity-based decision making
* Improves train planning efficiency
* Demonstrates real-world sorting logic
* Introduces object-oriented collection handling

### Output

```text id="uc7output02"
=== Train Consist Management App ===

After Sorting (Ascending by Capacity):
Bogie: First Class | Capacity: 24
Bogie: AC Chair | Capacity: 56
Bogie: Sleeper | Capacity: 72
```

### Conclusion

This use case enhances the system by introducing intelligent ordering of bogies, making the application more practical for real-world railway management scenarios.
