# Python
- [Python 3 documentation](https://docs.python.org/3/), 
[Tutorial](https://docs.python.org/3/tutorial/index.html)
[Library](https://docs.python.org/3/library/index.html), 
[Language Reference](https://docs.python.org/3/reference/index.html)


## Collection Types
- Library > [Collections Abstract Base Classes](https://docs.python.org/3/library/collections.abc.html#collections-abstract-base-classes)
- Library > [Collections](https://docs.python.org/3/library/collections.html)
- Library > [Common Sequence Operations](https://docs.python.org/3/library/stdtypes.html#common-sequence-operations)
- Library > [Mutable Sequence Types](https://docs.python.org/3/library/stdtypes.html#mutable-sequence-types)
- [PEP 3119 -- Introducing Abstract Base Classes](https://www.python.org/dev/peps/pep-3119/)


Sequence Types — 
[list](#list), 
[tuple](#tuple), 
[range](#range) 

Text Sequence Type — str

Set Types — set, frozenset

Mapping Types — dict


#### list
- Tutorial > [Lists](https://docs.python.org/3/tutorial/introduction.html#lists)
- Library > [Lists](https://docs.python.org/3/library/stdtypes.html#lists)
- [py · list · create](https://replit.com/@rabinjoshi1/py-list-create#main.py)

*Lists are mutable sequences*\ 
*list > MutableSequence > Sequence > Container, Iterable, Sized* 

```python
list[i]	# ith item of s
list[i:j]	# slice of s from i to j
len(list) # length of list

x in list	# True if exists
x not in list	# False if exists

list.append(elem) # adds a single element to the end of the list
list.insert(index, elem) # inserts the element at the given index, shifting elements to the right
list.extend(list2) # adds the elements in list2 to the end of the list
list.remove(elem) # searches for the element, removes first instance, throws ValueError if not present
list.sort() # sorts the list in place
list.reverse() # reverses the list in place
list.pop() # returns the rightmost element 
list.pop(index) # removes and returns the element at the given index, 

# Check if exists
"foo" in list1
any(elem.name == "foo" for elem in list)

# Find element
next((elem for elem in list if elem.name == "foo"), None) # first
[elem for elem in list if elem.name == "foo"] # all, empty array if none found

# Find index
list.index("foo") # unsafe
next((i for i, v in enumerate(list) if v == "foo"), None) # first
[i for i, v in enumerate(list) if v == "baz"] # all

# Find index & element
next(((i,v) for i, v in enumerate(list) if v == "foo"), None)
[(i,v) for i, v in enumerate(list) if v == "baz"]
```

#### [dict](https://docs.python.org/3/library/stdtypes.html#mapping-types-dict)

dict > MutableMapping > Mapping > Container, Iterable, Sized

```python
# Check if exists
"some_key" in dic
any({k:v for (k,v) in dic.items() if v.name == "foo"})

# Find
dic["some_key"] # unsafe, KeyError if key not found
dic.get("some_key") # None if not found
dic.get("some_key", "default") # default if not found
{k:v for (k,v) in dic.items() if v.name == "foo"} # all, {} if none found 

# Transform
{k:v**2 for (k,v) in dic.items()}
```

#### set 

set > MutableSet > Set > Container, Iterable, Sized



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



```
#generator expression
gen = (function_of_x for x in list_of_x if condition_with_x) 
list(gen) #convert to list
next(gen) #get first, unsafe
next(gen, default_value) #get first, safe

#list comprehension
[function_of_x for x in list_of_x if condition_with_x] #returns all or empty array
