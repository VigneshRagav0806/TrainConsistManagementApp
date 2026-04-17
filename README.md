## UC9: Group Bogies by Type (Collectors.groupingBy)

### Overview

This use case introduces grouping of bogies using the Stream API, transforming flat data into structured categories.

### Objective

To group bogies based on their type using Collectors.groupingBy().

### Drawback of Previous Approach

In UC8, bogies were filtered but remained in a flat list. This made it difficult to categorize and analyze data effectively.

### Solution

Use groupingBy() to organize bogies into categories.

### Flow of Execution

1. User runs the program
2. Bogie objects are created and stored in a list
3. List is converted into a stream
4. groupingBy() is applied using a classification function
5. Result is stored in a Map
6. Grouped data is displayed

### Key Concepts Used

* **Collectors.groupingBy()**

  * Groups elements into categories

* **Stream API**

  * Enables data transformation pipeline

* **Map Structure**

  * Stores grouped results as key-value pairs

* **Lambda Classification**

  * Defines grouping logic

* **Data Aggregation**

  * Organizes elements into logical clusters

### Code Summary

* Bogie list created with multiple entries
* Stream applied using stream()
* groupingBy(Bogie::getName) used
* Result stored in Map<String, List<Bogie>>
* Grouped data displayed category-wise

### Key Benefits

* Organizes data into meaningful groups
* Supports reporting and analytics
* Improves readability and structure
* Enables advanced data processing

### Output

```text id="uc9output02"
Category: Sleeper → 2 bogies
Category: AC Chair → 2 bogies
Category: First Class → 1 bogie
```

### Conclusion

This use case transforms raw data into structured information, enabling better decision-making and preparing the system for reporting and analytics.
