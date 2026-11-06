# Unit 01 – Introduction to Algorithms

## 1. Overview

This unit introduces fundamental algorithms and their implementation in C++. The programs included in this unit demonstrate basic searching and sorting techniques and help in understanding algorithmic problem-solving and complexity analysis.

## 2. Algorithms Implemented

The following algorithms are implemented in this unit:

1. Linear Search
2. Bubble Sort
3. Selection Sort
4. Insertion Sort

## 3. Linear Search

### Problem Statement

Given an array of elements and a target value, find the position of the target element using sequential searching.

### Algorithm / Approach

Linear Search checks each element of the array one by one until the target element is found or the end of the array is reached.

### Pseudocode

```text
LINEAR_SEARCH(array, target)

    FOR i = 0 to n - 1

        IF array[i] == target
            RETURN i

    RETURN -1
```

### Complexity Analysis

| Case | Time Complexity |
|---|---|
| Best Case | O(1) |
| Average Case | O(n) |
| Worst Case | O(n) |

**Space Complexity:** O(1)

### Sample Input

```text
Array: 10 20 30 40 50
Target: 30
```

### Sample Output

```text
Element found at index: 2
```

## 4. Bubble Sort

### Problem Statement

Sort the given array in ascending order using the Bubble Sort algorithm.

### Algorithm / Approach

Bubble Sort repeatedly compares adjacent elements and swaps them if they are in the wrong order. After every pass, the largest unsorted element moves toward the end of the array.

### Pseudocode

```text
BUBBLE_SORT(array)

    FOR i = 0 to n - 2

        FOR j = 0 to n - i - 2

            IF array[j] > array[j + 1]

                SWAP array[j] and array[j + 1]
```

### Complexity Analysis

| Case | Time Complexity |
|---|---|
| Best Case | O(n) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

**Space Complexity:** O(1)

### Sample Input

```text
5 2 8 1 3
```

### Sample Output

```text
1 2 3 5 8
```

## 5. Selection Sort

### Problem Statement

Sort an array in ascending order using the Selection Sort algorithm.

### Algorithm / Approach

Selection Sort repeatedly finds the smallest element from the unsorted portion of the array and places it at the beginning of that portion.

### Pseudocode

```text
SELECTION_SORT(array)

    FOR i = 0 to n - 2

        minIndex = i

        FOR j = i + 1 to n - 1

            IF array[j] < array[minIndex]
                minIndex = j

        SWAP array[i] and array[minIndex]
```

### Complexity Analysis

| Case | Time Complexity |
|---|---|
| Best Case | O(n²) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

**Space Complexity:** O(1)

### Sample Input

```text
64 25 12 22 11
```

### Sample Output

```text
11 12 22 25 64
```

## 6. Insertion Sort

### Problem Statement

Sort an array in ascending order using the Insertion Sort algorithm.

### Algorithm / Approach

Insertion Sort builds the sorted array one element at a time. Each new element is compared with the elements before it and inserted into its correct position.

### Pseudocode

```text
INSERTION_SORT(array)

    FOR i = 1 to n - 1

        key = array[i]
        j = i - 1

        WHILE j >= 0 AND array[j] > key

            array[j + 1] = array[j]
            j = j - 1

        array[j + 1] = key
```

### Complexity Analysis

| Case | Time Complexity |
|---|---|
| Best Case | O(n) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

**Space Complexity:** O(1)

### Sample Input

```text
12 11 13 5 6
```

### Sample Output

```text
5 6 11 12 13
```

## 7. Comparison of Algorithms

| Algorithm | Best Case | Average Case | Worst Case | Space |
|---|---|---|---|---|
| Linear Search | O(1) | O(n) | O(n) | O(1) |
| Bubble Sort | O(n) | O(n²) | O(n²) | O(1) |
| Selection Sort | O(n²) | O(n²) | O(n²) | O(1) |
| Insertion Sort | O(n) | O(n²) | O(n²) | O(1) |

## 8. Learning Outcomes

After completing this unit, the following concepts were studied:

1. Understanding basic algorithmic problem-solving.
2. Implementation of searching algorithms.
3. Implementation of sorting algorithms.
4. Understanding iterative approaches.
5. Understanding best, average, and worst-case complexity.
6. Analyzing time and space complexity.
7. Comparing different searching and sorting techniques.
8. Implementing algorithms using C++.

## 9. Files in This Unit

```text
Unit01-Introduction-Algorithms/
│
├── bubble_sort.cpp
├── insertion_sort.cpp
├── linear_search.cpp
├── selection_sort.cpp
└── README.md
```

## 10. Conclusion

This unit provides an introduction to fundamental searching and sorting algorithms. The implementations demonstrate how different approaches solve common algorithmic problems and provide a foundation for studying more advanced algorithms in subsequent units.