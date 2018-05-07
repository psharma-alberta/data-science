# zip

###### [Library: zip(*iterables)](https://docs.python.org/3/library/functions.html#zip)

- *returns an iterator of tuples, containing elements from each sequence*


```Python
z = zip([1, 2, 3], [1, 2, 3])

for x, y in z:
  print(x, y) 
  # 1 1
  # 2 2
  # 3 3
  
for tup in z:
  print(tup)
  # (1, 1)
  # (2, 2)
  # (3, 3)
  
type(z) # zip

list(z) # [(1, 1), (2, 2), (3, 3)]
```


```Python
# if unequal, default uses the shorter list
zip([1, 2, 3, 4], [1, 2, 3]) # list(z) = [(1, 1), (2, 2), (3, 3)]
```

```Python
# if unequal, zip_longest uses the longer list, insets None
from itertools import zip_longest
zip_longest([1, 2, 3, 4], [1, 2, 3]) # list(z) = [(1, 1), (2, 2), (3, 3), (4, None)] 
```

```Python

```
