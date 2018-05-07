# enumerate 

- [Library: enumerate(iterable, start=0)](https://docs.python.org/3/library/functions.html#enumerate)

- [Python Cookbook: Chapter 4. Iterators and Generators](https://www.safaribooksonline.com/library/view/python-cookbook-3rd/9781449357337/ch04.html)


**enumerate()** returns an interator of tuples containing index and value

```python
  # Iterating over index-value pairs of a sequence
  lst = ['a', 'b', 'c']
  
  for idx, val in enumerate(lst):
    print(idx, val) # 0 a, 1 b, 2 c
    
  for tup in enumerate(lst):
    print(tup) # (0, 'a'), (1, 'b'), (2, 'c')
    
  list(enumerate(lst)) # [(0, 'a'), (1, 'b'), (2, 'c')]
```



