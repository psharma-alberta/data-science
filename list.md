
### [list](https://docs.python.org/3/library/stdtypes.html#list)

list > MutableSequence > Sequence > Container, Iterable, Sized

##### Find

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

##### Transform

```python
squares = [x**2 for x in range(10)]
```
