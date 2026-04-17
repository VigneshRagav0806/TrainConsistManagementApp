## UC2: Add Passenger Bogies to Train (ArrayList Operations)

### Overview

This use case enhances the Train Consist Management Application by enabling dynamic manipulation of passenger bogies using ArrayList operations.

### Objective

To allow users to add, remove, and verify passenger bogies dynamically.

### Flow of Execution

1. User runs the program
2. Passenger bogies are added to the train consist
3. The list of bogies is displayed
4. A bogie is removed from the list
5. System checks whether a specific bogie exists
6. Final list is displayed
7. Program continues execution

### Key Concepts Used

* **ArrayList**

  * A dynamic data structure that allows resizing during runtime

* **add() Method**

  * Adds elements to the list

* **remove() Method**

  * Removes specified elements from the list

* **contains() Method**

  * Checks if an element exists in the list

* **Insertion Order Preservation**

  * Maintains order of bogies as added

* **CRUD Operations**

  * Create → Add bogies
  * Read → Display bogies
  * Delete → Remove bogies

### Code Summary

* An ArrayList is created to store passenger bogies
* Three bogies are added: Sleeper, AC Chair, First Class
* One bogie (AC Chair) is removed
* Existence of "Sleeper" is checked using contains()
* Final list is displayed

### Key Benefits

* Demonstrates real-world dynamic list operations
* Shows how train composition changes over time
* Introduces CRUD operations using Java Collections
* Helps visualize attachment and detachment of bogies

### Output

```text
=== Train Consist Management App ===

Passenger Bogies after addition:
[Sleeper, AC Chair, First Class]

Passenger Bogies after removal:
[Sleeper, First Class]

Sleeper bogie exists in the train.

Final Passenger Bogies List:
[Sleeper, First Class]
```

### Conclusion

This use case builds upon UC1 by introducing dynamic operations on collections, enabling the system to simulate real-world train consist modifications.
