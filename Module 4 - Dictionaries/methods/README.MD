1. `clear()`: Removes all the key-value pairs from the dictionary. 
2. `copy()`: Returns a shallow copy of the dictionary. 
3. `fromkeys(seq[, value])`: Creates a new dictionary with keys from `seq` and values set to `value` (default is `None`). 
4. `get(key[, default])`: Returns the value associated with `key`. If the key is not found, it returns `default` (default is `None`). 
5. `items()`: Returns a view object that contains key-value pairs of the dictionary. 
6. `keys()`: Returns a view object that contains all the keys of the dictionary. 
7. `values()`: Returns a view object that contains all the values of the dictionary. 
8. `pop(key[, default])`: Removes and returns the value associated with `key`. If the key is not found, it returns `default` (default is `None`). 
9. `popitem()`: Removes and returns a randomly selected key-value pair as a tuple. 
10. `setdefault(key[, default])`: Returns the value associated with `key`. If the key is not found, it inserts the key with the value `default` (default is `None`) and returns `default`. 
11. `update([other])`: Updates the dictionary with the key-value pairs from `other`. 
12. `__getitem__(key)`: Returns the value associated with `key`. Equivalent to using square brackets (`[]`) to access the value. 
13. `__setitem__(key, value)`: Sets the value associated with `key`. Equivalent to using square brackets (`[]`) to assign a value. 
14. `__delitem__(key)`: Deletes the key-value pair associated with `key`. Equivalent to using the `del` statement. 
15. `__contains__(key)`: Returns `True` if `key` is present in the dictionary, `False` otherwise. 
16. `__len__()`: Returns the number of key-value pairs in the dictionary.