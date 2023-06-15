1. **Accessing Values** : You can access the value associated with a specific key using square brackets (`[]`) or the `get()` method. For example:

```python

my_dict = {"name": "John", "age": 25, "city": "New York"}

print(my_dict["name"])  # Output: John
print(my_dict.get("age"))  # Output: 25
``` 
2. **Updating Values** : You can update the value associated with a key by assigning a new value to it. For example:

```python

my_dict = {"name": "John", "age": 25, "city": "New York"}

my_dict["age"] = 26
print(my_dict)  # Output: {"name": "John", "age": 26, "city": "New York"}
``` 
3. **Adding New Key-Value Pairs** : You can add new key-value pairs to a dictionary by assigning a value to a new key. For example:

```python

my_dict = {"name": "John", "age": 25}

my_dict["city"] = "New York"
print(my_dict)  # Output: {"name": "John", "age": 25, "city": "New York"}
``` 
4. **Removing Key-Value Pairs** : You can remove key-value pairs from a dictionary using the `del` statement or the `pop()` method. For example:

```python

my_dict = {"name": "John", "age": 25, "city": "New York"}

del my_dict["age"]
print(my_dict)  # Output: {"name": "John", "city": "New York"}

age = my_dict.pop("age")
print(age)  # Output: 25
``` 
5. **Checking Key Existence** : You can check if a key exists in a dictionary using the `in` operator. For example:

```python

my_dict = {"name": "John", "age": 25}

if "age" in my_dict:
    print("Age is present.")
``` 
6. **Iterating Over a Dictionary** : You can iterate over the keys, values, or key-value pairs of a dictionary using loops. For example:

```python

my_dict = {"name": "John", "age": 25, "city": "New York"}

# Iterating over keys
for key in my_dict:
    print(key)

# Iterating over values
for value in my_dict.values():
    print(value)

# Iterating over key-value pairs
for key, value in my_dict.items():
    print(key, value)
```

These are some of the basic operations you can perform on dictionaries in Python. Dictionaries offer a powerful and flexible