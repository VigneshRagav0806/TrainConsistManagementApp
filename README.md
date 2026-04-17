## UC4: Maintain Ordered Bogie IDs (LinkedList)

### Overview

This use case introduces LinkedList to maintain the physical order of bogies in a train. Unlike HashSet, which does not preserve order, LinkedList models real-world train chaining effectively.

### Objective

To maintain an ordered sequence of bogies and allow efficient insertion and removal operations.

### Drawback of Previous Approach

In UC3, HashSet ensured uniqueness but failed to maintain order. However, train bogies must follow a fixed physical sequence.

### Solution

Use LinkedList to preserve order and support efficient modifications.

### Flow of Execution

1. User runs the program
2. Train consist is created using LinkedList
3. Bogies are added in sequence
4. A new bogie is inserted at a specific position
5. First and last bogies are removed
6. Final ordered consist is displayed

### Key Concepts Used

* **LinkedList**

  * A doubly linked list implementation of List

* **Node Structure**

  * Each element links to previous and next nodes

* **add() Method**

  * Adds elements to the list

* **add(index, element)**

  * Inserts element at a specific position

* **removeFirst() / removeLast()**

  * Removes elements from beginning and end

* **Order Preservation**

  * Maintains real-world train sequence

### Code Summary

* LinkedList is used to store bogies
* Initial bogies: Engine, Sleeper, AC, Cargo, Guard
* Pantry Car inserted at position 2
* First and last bogies removed
* Final ordered list displayed

### Key Benefits

* Accurately models train structure
* Efficient insertion and deletion
* Maintains strict ordering
* Demonstrates node-based data structure

### Output

```text id="uc4output02"
=== Train Consist Management App ===

Initial Train Consist:
[Engine, Sleeper, AC, Cargo, Guard]

After inserting Pantry Car at position 2:
[Engine, Pantry Car, Sleeper, AC, Cargo, Guard]

After removing first and last bogie:
[Pantry Car, Sleeper, AC, Cargo]
```

### Conclusion

This use case ensures that train composition follows a strict order, making the system closer to real-world railway operations.
