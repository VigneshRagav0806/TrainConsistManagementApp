## UC14: Handle Invalid Bogie Capacity (Custom Exception)

### Overview

This use case introduces custom exception handling to enforce valid passenger bogie capacity.

### Objective

To prevent invalid bogies from being created using fail-fast validation.

### Drawback of Previous Approach

Earlier use cases assumed valid input, allowing invalid capacity values such as zero or negative numbers.

### Solution

Create a custom exception and validate capacity during object creation.

### Flow of Execution

1. User attempts to create a passenger bogie
2. Constructor validates capacity
3. If capacity ≤ 0 → exception is thrown
4. If valid → bogie is created
5. System continues execution safely

### Key Concepts Used

* **Custom Exception**

  * User-defined exception for invalid capacity

* **Exception Inheritance**

  * Extends Exception class

* **throw**

  * Raises exception when rule fails

* **throws**

  * Declares exception in method signature

* **Fail-Fast Validation**

  * Stops invalid object creation early

### Code Summary

* InvalidCapacityException class created
* Constructor validates capacity
* Exception thrown for invalid values
* Valid bogies added to list
* Invalid bogies rejected

### Key Benefits

* Prevents invalid data entry
* Protects system integrity
* Improves reliability
* Demonstrates defensive programming

### Output

```text id="uc14output02"
Exception Occurred: Capacity must be greater than zero
```

### Conclusion

This use case ensures that invalid bogie data is rejected at creation time, making the system robust and error-resistant.
