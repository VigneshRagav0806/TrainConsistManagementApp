## UC10: Count Total Seats in Train (reduce)

### Overview

This use case introduces aggregation using the Stream API to compute total seating capacity of the train.

### Objective

To calculate the total number of seats by aggregating capacities of all bogies.

### Drawback of Previous Approach

In UC9, bogies were grouped but no numerical insights were available. The system lacked the ability to compute totals required for planning.

### Solution

Use map() and reduce() to aggregate capacity values.

### Flow of Execution

1. User runs the program
2. Bogie objects are created
3. List is converted into a stream
4. map() extracts capacity values
5. reduce() aggregates them into a total
6. Total seating capacity is displayed

### Key Concepts Used

* **map()**

  * Extracts capacity values from objects

* **reduce()**

  * Aggregates values into a single result

* **Method Reference**

  * Uses Integer::sum for concise addition

* **Stream Pipeline**

  * Chains operations (map → reduce)

* **Functional Aggregation**

  * Replaces manual loops

### Code Summary

* Bogie list created
* Stream applied
* map() extracts capacity
* reduce(0, Integer::sum) calculates total
* Result displayed

### Key Benefits

* Provides real-world metrics
* Enables capacity planning
* Improves decision-making
* Eliminates manual summation logic

### Output

```text id="uc10output02"
Total Seating Capacity: 232
```

### Conclusion

This use case completes the data processing lifecycle by introducing aggregation, enabling the system to produce meaningful numerical insights.
