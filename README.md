## UC15: Safe Cargo Assignment Using try-catch-finally

### Overview

This use case introduces runtime exception handling to safely manage cargo assignments in goods bogies.

### Objective

To prevent unsafe cargo assignments and handle them gracefully without crashing the system.

### Drawback of Previous Approach

In UC14, validation occurred during object creation. However, runtime operations such as cargo assignment were not protected.

### Solution

Use try-catch-finally to handle unsafe conditions dynamically.

### Flow of Execution

1. User assigns cargo to a bogie
2. System checks safety rules
3. If unsafe → exception is thrown
4. Exception is caught and handled
5. finally block executes
6. Program continues execution

### Key Concepts Used

* **try-catch-finally**

  * Structured exception handling

* **Runtime Exception**

  * Unchecked exception for runtime errors

* **Custom Exception**

  * CargoSafetyException for domain-specific errors

* **throw**

  * Signals unsafe condition

* **Graceful Failure Handling**

  * Prevents crashes

* **finally Block**

  * Executes regardless of success or failure

### Code Summary

* GoodsBogie class created
* assignCargo() method contains try-catch-finally
* Unsafe assignment throws exception
* Exception is handled without stopping program
* finally block logs completion

### Key Benefits

* Prevents application crashes
* Handles runtime errors safely
* Ensures system continuity
* Demonstrates defensive coding practices

### Output

```text id="uc15output02"
Error: Unsafe Assignment: Rectangular bogie cannot carry Petroleum
```

### Conclusion

This use case ensures that runtime errors are handled gracefully, maintaining system stability and reliability during operations.
