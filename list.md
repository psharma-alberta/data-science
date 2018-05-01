
# list

#### [Tutorial - 3.1.3. Lists](https://docs.python.org/3/tutorial/introduction.html#lists)
#### [Library Reference - 4.6.4. Lists](https://docs.python.org/3/library/stdtypes.html#lists)

list > MutableSequence > Sequence > Container, Iterable, Sized

#### Create


#### Non-mutating methods 

```python
list[i]	# ith item of s
list[i:j]	# slice of s from i to j
len(list) # length of list

x in list	# True if exists
x not in list	# False if exists
```
See: [The Python Standard Library - 4.6.1. Common Sequence Operations](https://docs.python.org/3/library/stdtypes.html#common-sequence-operations)


#### Mutating methods 

```python
list.append(elem) # adds a single element to the end of the list
list.insert(index, elem) # inserts the element at the given index, shifting elements to the right
list.extend(list2) # adds the elements in list2 to the end of the list
list.remove(elem) # searches for the element, removes first instance, throws ValueError if not present
list.sort() # sorts the list in place
list.reverse() # reverses the list in place
list.pop() # returns the rightmost element 
list.pop(index) # removes and returns the element at the given index, 
```
See: [The Python Standard Library - 4.6.3. Mutable Sequence Types](https://docs.python.org/3/library/stdtypes.html#mutable-sequence-types)


#### Search

```python
# Check if exists
"foo" in list1
any(elem.name == "foo" for elem in list)
```

```python
# Find element
next((elem for elem in list if elem.name == "foo"), None) # first
[elem for elem in list if elem.name == "foo"] # all, empty array if none found
```

```python
# Find index
list.index("foo") # unsafe
next((i for i, v in enumerate(list) if v == "foo"), None) # first
[i for i, v in enumerate(list) if v == "baz"] # all
```

```python
# Find index & element
next(((i,v) for i, v in enumerate(list) if v == "foo"), None)
[(i,v) for i, v in enumerate(list) if v == "baz"]
```

#### Sort

#### Transform

```python
squares = [x**2 for x in range(10)]
```
