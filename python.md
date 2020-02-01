# python

- [Python 3 documentation](https://docs.python.org/3/), 
[Tutorial](https://docs.python.org/3/tutorial/index.html)
[Library](https://docs.python.org/3/library/index.html), 
[Language Reference](https://docs.python.org/3/reference/index.html)
- [Python and Flask - CS50W Notes](https://cs50.harvard.edu/web/notes/2/)

#### Collection Types

Sequence Types — 
[list](https://github.com/mobilege/data-science/blob/master/list.md), 
[tuple](https://github.com/mobilege/data-science/blob/master/tuple.md), 
[range](https://github.com/mobilege/data-science/blob/master/range.md) . 

- [8.4.1. Collections Abstract Base Classes](https://docs.python.org/3/library/collections.abc.html#collections-abstract-base-classes)
- [PEP 3119 -- Introducing Abstract Base Classes](https://www.python.org/dev/peps/pep-3119/)

Text Sequence Type — str

Set Types — set, frozenset

Mapping Types — dict


#### Control Flow

[enumerate](https://github.com/mobilege/data-science/blob/master/enumerate.md), 
[zip](https://github.com/mobilege/data-science/blob/master/zip.md),
[Iterators](https://github.com/mobilege/data-science/blob/master/iterators.md),
Generators

- [Library: 2. Built-in Functions](https://docs.python.org/3/library/functions.html)

## Misc

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
