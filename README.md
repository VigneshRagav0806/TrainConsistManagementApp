## UC5: Preserve Insertion Order of Bogies (LinkedHashSet)

### Overview

This use case introduces LinkedHashSet to maintain both uniqueness and insertion order of bogies in the train formation.

### Objective

To ensure that bogies are stored in the exact order they are added while preventing duplicate entries.

### Drawback of Previous Approach

In UC4, LinkedList maintained order but allowed duplicate bogies. This could result in invalid train formations.

### Solution

Use LinkedHashSet to combine:

* Order preservation
* Automatic duplicate prevention

### Flow of Execution

1. User runs the program
2. Bogies are added to the train formation
3. A duplicate bogie is intentionally inserted
4. LinkedHashSet ignores the duplicate
5. Final ordered formation is displayed

### Key Concepts Used

* **LinkedHashSet**

  * Maintains insertion order and ensures uniqueness

* **Set Interface**

  * Prevents duplicate elements

* **add() Method**

  * Adds elements to the set
  * Ignores duplicates automatically

* **Automatic Deduplication**

  * No manual validation required

* **Insertion Order Preservation**

  * Maintains real-world train sequence

* **Ordered Iteration**

  * Elements are displayed in insertion order

### Code Summary

* LinkedHashSet is used to store bogies
* Bogies added: Engine, Sleeper, Cargo, Guard
* Duplicate "Sleeper" is ignored
* Final formation is displayed in correct order

### Key Benefits

* Prevents duplicate bogie attachment
* Maintains real train sequence
* Combines advantages of Set and List
* Ensures predictable and safe data handling

### Output

```text id="uc5output02"
=== Train Consist Management App ===

Final Train Formation (Insertion Order Preserved):
[Engine, Sleeper, Cargo, Guard]

Total bogies: 4
```

### Conclusion

This use case ensures that the train consist remains both unique and ordered, making it suitable for real-world railway system simulations.
