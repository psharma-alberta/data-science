# iterators

###### [Tutorial: 9.8. Iterators](https://docs.python.org/3/tutorial/classes.html#iterators)

###### [Library: 4.5. Iterator Types](https://docs.python.org/3/library/stdtypes.html#iterator-types)

###### [Fluent Python: Chapter 14. Iterables, Iterators, and Generators](https://www.safaribooksonline.com/library/view/fluent-python/9781491946237/ch14.html)

###### [Python Cookbook: Chapter 4. Iterators and Generators](https://www.safaribooksonline.com/library/view/python-cookbook-3rd/9781449357337/ch04.html)


#### enumerate()

```python
  # Iterating over index-value pairs of a sequence
  lst = ['a', 'b', 'c']
  
  for idx, val in enumerate(lst):
    print(idx, val) # 0 a, 1 b, 2 c
    
  for tup in enumerate(lst):
    print(tup) # (0, 'a'), (1, 'b'), (2, 'c')
    
  list(enumerate(lst)) # [(0, 'a'), (1, 'b'), (2, 'c')]
```

- *enumerate() returns an interator, invoking __next__() on which returns a tuple containing index and value*

###### [enumerate(iterable, start=0)](https://docs.python.org/3/library/functions.html#enumerate)
