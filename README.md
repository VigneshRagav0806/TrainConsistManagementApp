## UC11: Validate Train ID & Cargo Codes (Regex)

### Overview

This use case introduces input validation using Regular Expressions to ensure that Train IDs and Cargo Codes follow strict formats.

### Objective

To validate user input before processing using regex patterns.

### Drawback of Previous Approach

In UC10, the system assumed all inputs were valid. This can lead to incorrect data entering the system and causing failures in processing.

### Solution

Use Pattern and Matcher classes with regular expressions to enforce format rules.

### Flow of Execution

1. User enters Train ID and Cargo Code
2. Regex patterns are defined
3. Patterns are compiled
4. Matcher checks input against pattern
5. System validates and displays result

### Key Concepts Used

* **Regular Expressions (Regex)**

  * Defines input format rules

* **Pattern Class**

  * Compiles regex for reuse

* **Matcher Class**

  * Matches input against pattern

* **matches()**

  * Ensures full string match

* **Format Enforcement**

  * Validates structure before processing

### Code Summary

* Train ID pattern: TRN-\d{4}
* Cargo Code pattern: PET-[A-Z]{2}
* Pattern compiled using Pattern class
* Matcher used to validate inputs
* Output displays valid/invalid result

### Key Benefits

* Prevents invalid data entry
* Ensures system reliability
* Improves data integrity
* Introduces real-world validation logic

### Output

```text id="uc11output03"
Train ID is VALID.
Cargo Code is VALID.
```

### Conclusion

This use case ensures that only correctly formatted data enters the system, making the application robust and reliable.
