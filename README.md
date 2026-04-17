## UC8: Filter Passenger Bogies Using Streams

### Overview

This use case introduces the Java Stream API to filter bogies based on capacity using a declarative programming approach.

### Objective

To select only those bogies that satisfy a given condition (capacity greater than a threshold).

### Drawback of Previous Approach

In UC7, bogies were sorted but could not be selectively filtered. Traditional looping approaches make code verbose and harder to maintain.

### Solution

Use Stream API with filter() to apply business rules clearly and efficiently.

### Flow of Execution

1. User runs the program
2. Bogie objects are created and stored in a list
3. List is converted into a stream
4. filter() is applied based on capacity condition
5. Results are collected into a new list
6. Filtered bogies are displayed

### Key Concepts Used

* **Stream API**

  * Processes collections declaratively

* **stream()**

  * Converts list into stream pipeline

* **filter()**

  * Applies condition (capacity > 60)

* **Lambda Expressions**

  * Defines filtering logic concisely

* **collect()**

  * Converts stream result back into list

* **Declarative Programming**

  * Focuses on "what" instead of "how"

### Code Summary

* List of bogies created
* Stream applied using stream()
* filter(b -> b.getCapacity() > 60)
* Results collected using Collectors.toList()
* Filtered list displayed

### Key Benefits

* Reduces boilerplate code
* Improves readability
* Separates business logic from iteration
* Enables scalable data processing

### Output

```text
Filtered Bogies (Capacity > 60):
Bogie: Sleeper | Capacity: 72
Bogie: Luxury AC | Capacity: 80
```

### Conclusion

This use case enhances the system by enabling dynamic filtering of bogies using modern functional programming techniques in Java.
