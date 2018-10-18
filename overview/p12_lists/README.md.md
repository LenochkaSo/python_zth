# List
***Mutable*** sequences of objects
[list](https://docs.python.org/3.7/tutorial/datastructures.html)
## List literal
```python
>>> # empty list
>>> l = []

>>> # list of hetrogeneous items
>>> l = [1, "two", 3.0]
>>>
```
## List is a sequence, so...
```python
>>> # concatanation
>>> [1, 2] + [3, 4]
[1, 2, 3, 4]

>>> # repetition
>>> [1, 2] * 2
[1, 2, 1, 2]

>>> # membership testing
>>> 3 in [1, 2, 4]
False

>>> # other sequence methods
>>> len([1, 2])
2
>>> [1, 2, 1].count(1)
2
>>> [1, 2].index(2)
1

>>> # list is a mutable sequence
>>> l = [1, 2, 3]
>>> l[1:] = [4, 5, 6]
>>> l
[1, 4, 5, 6]
>>> del(l[1])
>>> l
[1, 5, 6]

>>> # coping a list (not the reference!)
>>> l = [1, 2, 3]
>>> l2 = l[:]
>>> id(l) == id(l2)
False 
>>> l2 = l.copy()
>>> l2 = list(l)

>>> # emptying a list (not assigning new empty list to the reference!)
>>> l[:] = []
```
### Comparing lists (or any other sequence)
- comparison uses lexicographical ordering
- equality is deep element-wise equality
[comparing-sequences](https://docs.python.org/3/tutorial/datastructures.html#comparing-sequences-and-other-types)
```python
[1, 2, 3] < [1, 2, 4]

[1, 2] < [1, 2, -1]

[1, 2] == [1, 2]

[1, 2] == [1.0, 2.0]
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4OTAyNDg5NzMsMTI5NjM0NTQyNSwtMT
c4MDAyNTUzNiwtOTE3NDM4NDM3LDE0OTE3MTI0OTMsMTAyMzU4
NzU0OF19
-->