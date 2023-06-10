## Python Lists

In Python, a list is a versatile and mutable data structure that allows you to store a collection of items. Lists can contain elements of different data types, such as integers, strings, or even other lists. Lists are ordered, meaning the elements are arranged in a specific order and can be accessed by their indices.

Here's an example of creating and working with lists in Python:

```python
# Creating a list
my_list = [1, 2, 3, "four", 5.0]

# Accessing elements in the list
print(my_list[0])  # Output: 1
print(my_list[3])  # Output: "four"

# Modifying elements in the list
my_list[2] = "three"
print(my_list)  # Output: [1, 2, "three", "four", 5.0]

# List operations
my_list.append(6)
my_list.extend([7, 8, 9])
print(my_list)  # Output: [1, 2, "three", "four", 5.0, 6, 7, 8, 9]

# Removing elements from the list
my_list.remove("four")
print(my_list)  # Output: [1, 2, "three", 5.0, 6, 7, 8, 9]

# Other list operations and functions
print(len(my_list))        # Output: 8
print(my_list.index(5.0))  # Output: 3
print(my_list.count(2))    # Output: 1


```
Lists in Python provide a range of built-in functions and methods to manipulate and operate on the list elements. Some common operations include appending elements, extending the list with another list, removing elements, finding the length of the list, and more.

Python lists are mutable, meaning you can modify the elements within the list. This flexibility makes lists a fundamental data structure for various tasks, such as storing collections of data, implementing algorithms, and building more complex data structures.

Understanding how to work with lists in Python is essential for efficient programming and data manipulation tasks.
| Operation              | Time | Space |
|------------------------|------|-------|
| Creating Empty         | O(1) | O(1)  |
| Creating With Elements | O(N) | O(N)  |
| Inserting              | O(N) | O(1)  |
| Traversing             | O(N) | O(1)  |
| Accessing              | O(1) | O(1)  |
| Searching              | O(N) | O(1)  |
| Deleting               | O(N) | O(1)  |