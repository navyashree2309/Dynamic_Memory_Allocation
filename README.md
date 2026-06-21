# Dynamic Memory Allocation Techniques

## Overview

This project implements three dynamic memory allocation techniques used in Operating Systems:

* First Fit
* Best Fit
* Worst Fit

The program simulates memory allocation for processes, compares different allocation strategies, displays remaining free partitions, and analyzes memory utilization and fragmentation.

---

## Features

* Implementation of First Fit, Best Fit, and Worst Fit algorithms
* Dynamic memory partition allocation
* Process-to-partition mapping
* Remaining free partition display
* Execution time comparison
* Memory fragmentation analysis

---

## Technologies Used

* C Programming Language
* Standard C Libraries:

  * `stdio.h`
  * `time.h`

---

## Input

The program accepts:

1. Number of memory partitions
2. Sizes of memory partitions
3. Number of processes
4. Sizes of processes

### Sample Input

``text
Enter number of memory partitions: 5

Enter partition sizes:
100 500 200 300 600

Enter number of processes: 4

Enter process sizes:
212 417 112 426
``

---

## Sample Output

### First Fit Allocation

text
Process   Size   Partition No
P0        212    2
P1        417    5
P2        112    2
P3        426    Not Allocated


### Free Partitions

text
Partition 1 = 100
Partition 2 = 176
Partition 3 = 200
Partition 4 = 300
Partition 5 = 183


### Analysis

text
First Fit : Fast allocation, moderate fragmentation.
Best Fit  : Minimum leftover space but may create small fragments.
Worst Fit : Leaves larger free blocks, may waste memory.
External Fragmentation occurs in all dynamic partition methods.


---

## Algorithms Implemented

### First Fit

Allocates a process to the first available partition that is large enough.

### Best Fit

Allocates a process to the smallest suitable partition, minimizing wasted space.

### Worst Fit

Allocates a process to the largest available partition, leaving larger free blocks for future allocations.

---

## Performance Comparison

| Algorithm | Characteristics                             |
| --------- | ------------------------------------------- |
| First Fit | Fast allocation, moderate fragmentation     |
| Best Fit  | Better memory utilization, slower execution |
| Worst Fit | Preserves large blocks, may waste memory    |

---

## Conclusion

This project demonstrates how different memory allocation strategies affect memory utilization and fragmentation. It provides a practical understanding of dynamic partition allocation and helps compare the efficiency of First Fit, Best Fit, and Worst Fit techniques used in Operating Systems.
