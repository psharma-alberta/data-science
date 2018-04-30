
# list

#### [Tutorial - 3.1.3. Lists](https://docs.python.org/3/tutorial/introduction.html#lists)
#### [Library Reference - 4.6.4. Lists](https://docs.python.org/3/library/stdtypes.html#lists)

list > MutableSequence > Sequence > Container, Iterable, Sized

#### Create

#### Adding/Removing elements 

```python
# Adding & inserting items
arr.append(item) # adds item, inplace
arr.extend(arr2) # adds items, inplace
arr.insert(idx, item) # inserts item at index, staring 0, inplace
```

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
