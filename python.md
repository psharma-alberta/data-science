# [python](https://docs.python.org/3/)

[Style Guide](https://www.python.org/dev/peps/pep-0008/)

## [Boolean](https://docs.python.org/3/library/stdtypes.html#truth-value-testing)

```python
# Evaluates to False:
None
False
0, 0.0, 0j.
'', (), [].
{}
```

## [enum](https://docs.python.org/3/library/enum.html)

### Enum

### IntEnum

### Flag

### IntFlag.

## [Collections](https://docs.python.org/3/library/collections.html)

[PEP 3119 -- Introducing Abstract Base Classes](https://www.python.org/dev/peps/pep-3119/)

```
#generator expression
gen = (function_of_x for x in list_of_x if condition_with_x) 
list(gen) #convert to list
next(gen) #get first, unsafe
next(gen, default_value) #get first, safe

#list comprehension
[function_of_x for x in list_of_x if condition_with_x] #returns all or empty array
```

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

#### [dict](https://docs.python.org/3/library/stdtypes.html#mapping-types-dict)

dict > MutableMapping > Mapping > Container, Iterable, Sized

##### Find

```python
# Check if exists
"some_key" in dic
any({k:v for (k,v) in dic.items() if v.name == "foo"})
```

```python
# Find element
dic["some_key"] # unsafe, KeyError if key not found
dic.get("some_key") # None if not found
dic.get("some_key", "default") # default if not found
{k:v for (k,v) in dic.items() if v.name == "foo"} # all, {} if none found 
```

##### Transform

```python
{k:v**2 for (k,v) in dic.items()}
```

#### set 

set > MutableSet > Set > Container, Iterable, Sized
