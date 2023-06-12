# Big O Notation

- **Big O notation (`O`)**: It represents the upper bound or worst-case scenario of an algorithm's time or space complexity. It provides an asymptotic upper limit on the growth rate of a function. When we say an algorithm has a time complexity of `O(f(n))`, it means the algorithm's runtime or space usage grows no faster than the function `f(n)`.

- **Theta notation (`Θ`)**: It represents the tight bound or average-case scenario of an algorithm's time or space complexity. It provides an asymptotic tight range within which the growth rate of a function falls. When we say an algorithm has a time complexity of `Θ(f(n))`, it means the algorithm's runtime or space usage grows at the same rate as the function `f(n)` within constant factors.

- **Omega notation (`Ω`)**: It represents the lower bound or best-case scenario of an algorithm's time or space complexity. It provides an asymptotic lower limit on the growth rate of a function. When we say an algorithm has a time complexity of `Ω(f(n))`, it means the algorithm's runtime or space usage grows no slower than the function `f(n)`.

These notations are used to describe the growth rate of functions and the scalability of algorithms, allowing us to analyze their efficiency in different scenarios. They provide a way to compare and classify algorithms based on their performance characteristics.

## **Runtime Complexity**

Runtime complexity refers to the amount of time it takes for an algorithm to run as a function of the input size. It is commonly denoted using big O notation.

Here are some common runtime complexities and their explanations:

- O(1) - Constant time complexity. The algorithm takes a constant amount of time to execute, regardless of the input size.
```python
def constantTimeComplexity(n):
    print(n)
```

- O(log n) - Logarithmic time complexity. The algorithm's execution time increases logarithmically with the input size. This is commonly seen in algorithms that divide the input in half at each step, such as binary search.
```python
def logarithmicTimeComplexity(arr, low, high, x):
    if high >= low:
        mid = (high + low) // 2
        if arr[mid] == x:
            return mid
        elif arr[mid] > x:
            return logarithmicTimeComplexity(arr, low, mid - 1, x)
         else:
            return logarithmicTimeComplexity(arr, mid + 1, high, x)
    else:
        return -1
```

- O(n) - Linear time complexity. The algorithm's execution time increases linearly with the input size. As the input doubles, the execution time also doubles.
```python
def linearTimeComplexity(n):
    for i in range(n):
        print(i)
```

- O(n log n) - Linearithmic time complexity. The algorithm's execution time is a product of the input size and its logarithm. This is commonly seen in efficient sorting algorithms like merge sort and quicksort.
```python
def linearithmicTimeComplexity(arr, l, m, r):
    n1, n2 = m - l + 1, r - m
    L,R = [0] * (n1), [0] * (n2)
    for i in range(0, n1):
        L[i] = arr[l + i]
    for j in range(0, n2):
        R[j] = arr[m + 1 + j]
    i, j, k = 0, 0, l
    while i < n1 and j < n2:
        if L[i] <= R[j]:
            arr[k] = L[i]
            i += 1
        else:
            arr[k] = R[j]
            j += 1
        k += 1
    while i < n1:
        arr[k] = L[i]
        i += 1
        k += 1
    while j < n2:
        arr[k] = R[j]
        j += 1
        k += 1
def mergeSort(arr, l, r):
    if l < r:
        m = l+(r-l)//2  
        mergeSort(arr, l, m)
        mergeSort(arr, m+1, r)
        linearithmicTimeComplexity(arr, l, m, r)

```

- O(n^2) - Quadratic time complexity. The algorithm's execution time increases quadratically with the input size. This is often seen in nested loops or algorithms that involve comparing every pair of elements in the input.
```python
def quadraticTimeComplexity(n):
    for i in range (n):
        for j in range(n):
            print(i, j)
```

- O(2^n) - Exponential time complexity. The algorithm's execution time doubles with each additional input element. This complexity is typically associated with brute-force algorithms or problems with a large number of possible solutions.
```python
def exponentialTimeComplexity(a, b)
    raise TODO
```
```python
def factorialTimeComplexity(a, b)
    raise TODO
```
Understanding runtime complexity helps in analyzing and comparing the efficiency of different algorithms. It allows us to estimate how an algorithm's execution time will scale with the input size, enabling us to make informed decisions when choosing the most suitable algorithm for a particular problem.

## Operations

When analyzing the runtime complexity of an algorithm, there may be cases where multiple operations or steps are involved, each with its own complexity. In such cases, we express the overall complexity using multiple O notations, taking into account the dominant factors.

Here are a few examples of how multiple O notations are used:

1. Addition: When two different operations are performed sequentially, each with its own time complexity, the overall complexity is determined by the sum of the individual complexities. For example, if an algorithm has a complexity of O(n) for one step and O(m) for another step, the overall complexity would be O(n + m).
```python
def sumExample(a, b)
    for i in range(a):
        print(i)
    for j in range(b):
        print(j)
```

2. Multiplication: When two different operations are performed nested within each other, each with its own time complexity, the overall complexity is determined by the product of the individual complexities. For example, if an algorithm has a complexity of O(n) for one step and O(m) for another step nested inside the first one, the overall complexity would be O(n * m).
```python
def multiplicationExample(a, b)
    for i in range(a):
        for j in range(b):
            print(j)
```

3. Dominant Terms: When there are multiple steps in an algorithm, it's important to identify the dominant term or operation that contributes the most to the overall complexity. For example, if an algorithm has a complexity of O(n^2) for one step and O(n) for another step, the dominant term is O(n^2), and the overall complexity is expressed as O(n^2).

By expressing the overall complexity using multiple O notations, we can have a more accurate representation of how the algorithm's runtime scales with the input size, accounting for different operations or steps involved in the algorithm.

