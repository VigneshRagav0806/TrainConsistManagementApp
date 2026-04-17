# TrainConsistManagementApp
## UC1: Initialize Train and Display Consist Summary

### Overview

This use case demonstrates the initialization phase of the Train Consist Management Application. It sets up the foundational structure required to manage train bogies dynamically.

### Objective

To initialize an empty train consist and display its initial state to the user.

### Flow of Execution

1. User runs the application
2. System displays a welcome message
3. Train consist is initialized as an empty collection
4. Initial bogie count is displayed
5. Application remains active for further operations

### Key Concepts Used

* **Class**

    * The entire application logic is encapsulated inside a Java class (`TrainApp`)

* **Main Method**

    * Entry point of the program:

      ```java
      public static void main(String[] args)
      ```

* **Static Keyword**

    * Allows the JVM to call `main()` without creating an object

* **ArrayList**

    * Used to dynamically store bogies
    * Allows resizing at runtime unlike fixed arrays

* **List Interface**

    * Provides abstraction for working with different list implementations

* **Console Output**

    * `System.out.println()` is used to display messages

* **Dynamic Initialization**

    * An empty `ArrayList` is created which will later store bogies

### Code Summary

* A List is created using `ArrayList`
* No bogies are added initially
* `size()` method is used to display count (which is 0)

### Key Benefits

* Establishes the starting point of the application
* Demonstrates program execution flow
* Highlights the importance of dynamic data structures
* Prepares the system for future operations like adding passenger or goods bogies

### Output

```
=== Train Consist Management App ===
Train consist initialized successfully.
Initial number of bogies: 0
System is ready for further operations...
```

### Conclusion

This use case lays the groundwork for the Train Consist Management System by initializing the core data structure and verifying that the application starts correctly.
