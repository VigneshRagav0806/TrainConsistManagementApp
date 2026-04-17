## UC6: Map Bogie to Capacity (HashMap)

### Overview

This use case introduces HashMap to associate each bogie with its seating or load capacity, enabling the system to store and manage operational data.

### Objective

To map bogie names to their respective capacities using a key–value structure.

### Drawback of Previous Approach

In UC5, bogies were stored only as names. This approach lacked the ability to store additional attributes such as seating or load capacity, making the system incomplete.

### Solution

Use HashMap to create a mapping between bogie names and their capacities.

### Flow of Execution

1. User runs the program
2. A HashMap is created
3. Bogie names are used as keys
4. Capacities are stored as values
5. Entries are inserted using put()
6. Map is iterated using entrySet()
7. Bogie-capacity details are displayed

### Key Concepts Used

* **HashMap**

  * Stores data in key–value pairs

* **Map Interface**

  * Defines mapping between keys and values

* **put() Method**

  * Inserts key–value pairs into the map

* **Key–Value Association**

  * Links bogie with its capacity

* **entrySet()**

  * Used to iterate over both keys and values

* **Fast Lookup**

  * Allows quick retrieval using keys

### Code Summary

* HashMap is created for storing bogie-capacity pairs
* Entries added:

  * Sleeper → 72
  * AC Chair → 54
  * First Class → 24
* entrySet() is used to iterate and display data

### Key Benefits

* Models real-world data relationships
* Enables capacity tracking and validation
* Improves system design using structured data
* Prepares for advanced features like analytics

### Output

```text id="uc6output02"
=== Train Consist Management App ===

Bogie Capacity Details:
Bogie: Sleeper | Capacity: 72
Bogie: AC Chair | Capacity: 54
Bogie: First Class | Capacity: 24
```

### Conclusion

This use case enhances the system by introducing data mapping, enabling realistic representation of bogie attributes and preparing the foundation for advanced train management features.
