# Python tips

## `map(TYPE, x)` vs `TYPE(x)`

Given an iterable x (of type T0) of objects of type T1 (for example a list of strings), and a
new type T2,

- `T2(x)` converts the iterable to the type T2 (for example to a _set_ of
  strings)

- `map(T2, x)` converts the iterable to a map object of elements of type T2
  (for example a map object of integers made from strings)

- `T0(map(T2, x))` converts the iterable to an iterable of the same type, with
  the elements converted to type T2 (for example to a list of integers from
  strings).
  
Full example:

    >>> x = [1, 2, 3, 0]
    >>> set(x)
    {1, 2, 3, 0}
    >>> map(bool, x)
    <map object at 0x1035d1b00>
    >>> for y in map(bool, x):
    ...     print(y)
    True
    True
    True
    False
    >>> list(map(bool, x))
    [True, True, True, False]
