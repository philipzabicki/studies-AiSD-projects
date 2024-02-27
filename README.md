# QuickSort Implementations Comparison

This repository contains two main files implementing different versions of the QuickSort algorithm:

1. **Standard QuickSort**: A classic implementation of the QuickSort algorithm.
2. **QuickSort with Improvements**: Includes versions with random pivot selection, and the Dutch National Flag optimization.

## Overview

- The **Standard QuickSort** performs poorly when the array contains many identical elements. This is where the **Dutch National Flag** optimization shines, as it efficiently handles arrays with many duplicates by only incrementing pointers without swapping values unnecessarily.
- The performance of the Dutch Flag version decreases as the range of random numbers increases (leading to fewer duplicates) due to the need for additional pointer management and more comparisons.
- Interestingly, the **QuickSort with random pivot selection** shows the most predictable performance across different array sizes and number ranges. It outperforms the standard implementation in worst-case scenarios and finds a middle ground in others.

## Performance Tests

The repository includes tests for different array sizes (from 100 to 100,000 elements) and number ranges, comparing the sorting time of each algorithm. The Dutch National Flag version generally offers significant improvements in scenarios with many duplicate elements, while the standard implementation is preferable for arrays with a wider range of unique numbers.

For detailed test results and analysis, refer to the specific algorithm implementations and test files within the repository.
