| Operation              | Time | Space |
|------------------------|------|-------|
| Creating Empty         | O(1) | O(1)  |
| Creating With Elements | O(N) | O(N)  |
| Inserting              | O(N) | O(1)  |
| Traversing             | O(N) | O(1)  |
| Accessing              | O(1) | O(1)  |
| Searching              | O(N) | O(1)  |
| Deleting               | O(N) | O(1)  |

```python
from array import *
```
```python
def crate_and_traverse():
    my_array = array('i',[1,2,3,4,5])
    for i in my_array:
        print (i)
```
```python
def access(my_array):
    print(my_array[1])
```
```python
def append_method(my_array):
    my_array.append(6)
```
```python
def insert_method(my_array):
    my_array.insert(0, 11)
```
```python
def extend_method(my_array):
    my_array.extend(6)
```
```python
def from_list_method(my_array):
    temp_list = [20,21]
    my_array.fromList(temp_list)
```
```python
def remove_method(my_array):
    my_array.remove(11)
```
```python
def pop_method(my_array):
    my_array.pop(20)
```
```python
def fetch(my_array):
    my_array.index(21)
```
```python
def reverse_method(my_array):
    my_array.reverse()
```
```python
def get_buffer_info(my_array):
    my_array.buffer_info()
```
```python
def count_occurences(my_array):
    my_array.count(11)
```
```python
def to_string_method(my_array):
    my_array.tostring()
    my_array.fromstring()
```
```python
def convert_to_python_list(my_array):
    my_array.tolist
```
```python
def slicing(my_array):
    my_array[start:stop:step]
```