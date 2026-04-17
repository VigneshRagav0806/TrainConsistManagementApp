## UC13: Performance Comparison (Loops vs Streams)

### Overview

This use case compares the performance of loop-based and stream-based filtering using precise time measurement.

### Objective

To measure execution time of two different approaches and make evidence-based decisions.

### Drawback of Previous Approach

In UC12, Streams were used for clean logic, but no performance comparison was done. Developers may incorrectly assume Streams are always faster.

### Solution

Use System.nanoTime() to benchmark both loop and stream approaches.

### Flow of Execution

1. User runs the program
2. Large dataset of bogies is created
3. Loop-based filtering is executed and timed
4. Stream-based filtering is executed and timed
5. Execution times are compared
6. Results are displayed

### Key Concepts Used

* **System.nanoTime()**

  * High precision time measurement

* **Loop-Based Processing**

  * Traditional iteration using for-each loop

* **Stream API**

  * Declarative filtering using filter()

* **Performance Benchmarking**

  * Measuring execution time

* **Evidence-Based Optimization**

  * Making decisions based on actual results

### Code Summary

* Large list of bogies created
* Loop filters bogies with capacity > 60
* Stream filters bogies with same condition
* Execution time measured using nanoTime()
* Results compared

### Key Benefits

* Demonstrates real performance differences
* Encourages measurement over assumptions
* Teaches benchmarking techniques
* Builds optimization mindset

### Output

```text
Loop Execution Time: XXXXX ns
Stream Execution Time: XXXXX ns
```

### Conclusion

This use case emphasizes that performance decisions should be based on measurement rather than assumptions, balancing readability and efficiency.
