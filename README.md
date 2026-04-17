## UC12: Safety Compliance Check for Goods Bogies

### Overview

This use case introduces safety validation for goods bogies using Stream API and business rules.

### Objective

To ensure that cylindrical bogies carry only petroleum cargo.

### Drawback of Previous Approach

Earlier use cases did not enforce domain-specific rules, allowing unsafe cargo configurations.

### Solution

Use stream-based validation with allMatch() and conditional logic.

### Flow of Execution

1. User creates a list of goods bogies
2. List is converted into a stream
3. allMatch() applies safety rules
4. If all bogies satisfy rules → SAFE
5. Else → NOT SAFE

### Key Concepts Used

* **Streams API**

  * Declarative processing of collections

* **allMatch()**

  * Checks if all elements satisfy condition

* **Lambda Expressions**

  * Defines rule logic inline

* **Conditional Logic**

  * Enforces domain constraints

* **Short-Circuit Evaluation**

  * Stops on first failure

### Code Summary

* GoodsBogie class created
* List of bogies initialized
* Stream applied
* Condition:

  * Cylindrical → only Petroleum allowed
* Boolean result determines safety

### Key Benefits

* Prevents unsafe configurations
* Enforces real-world constraints
* Improves system reliability
* Demonstrates domain-driven logic

### Output

```text id="uc12output03"
Train is SAFETY COMPLIANT.
```

### Conclusion

This use case ensures that the system enforces critical safety rules, making it suitable for real-world railway logistics scenarios.
