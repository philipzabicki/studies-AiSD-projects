# Project No. 1 QuickSort Implementations Comparison

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

# Project No. 2 BST Tree for Storing Abbreviations

This project implements a Binary Search Tree (BST) in Python for efficiently storing and retrieving abbreviations along with their full names. The keys in the tree are the abbreviations formed from the first letters of the names, and the values are the full names.

## Features

- `Add(key, value)`: Adds a new node to the tree with the given abbreviation (`key`) and full name (`value`).
- `Find(key)`: Searches for a node based on the provided abbreviation (`key`).
- `Delete(node)`: Removes a node from the tree.
- `PrintIO()`: Prints all the tree nodes in in-order traversal.
- `Height()`: Returns the height of the tree.
- `DSW()`: Performs the DSW (Day-Stout-Warren) algorithm to balance the tree.
- `Draw()`: Graphically represents the structure of the tree.

## Usage

Creating a Tree and Adding Elements
```python
# Creating the tree
tree = Tree()

# Adding elements
tree.Add('ABC', 'Alice has a cat')
tree.Add('XYZ', 'Xylophone by the window')
Searching and Deleting
```

# Searching for an element
```python
node = tree.Find('ABC')
print(node.key, node.value)
```
```python
# Deleting an element
tree.Delete(node)
Balancing the Tree
```

# Balancing the tree using the DSW algorithm
```python
tree.DSW()
```
