# Python Special Methods

Simple examples of Python's dunder methods.

## What's Inside

A notebook covering 16 special methods with straightforward examples.

| Method | Does What | Example |
|--------|-----------|---------|
| `__init__` | Constructor | `Dog` with name and age |
| `__str__` | Pretty print | `Book` title and author |
| `__repr__` | Debug info | Recreate the `Book` |
| `__len__` | Length | `Backpack` item count |
| `__eq__` | Equal check | `Person` by ID |
| `__add__` | Addition | `Point` coordinates |
| `__sub__` | Subtraction | (shown in Point) |
| `__mul__` | Multiply | (shown in Point) |
| `__getitem__` | Index access | `Playlist` songs |
| `__setitem__` | Index update | Edit `Playlist` |
| `__contains__` | Check `in` | `Fridge` contents |
| `__call__` | Call like function | `Multiplier` |
| `__iter__` | Loop with `for` | `Countdown` timer |
| `__next__` | Next item | Continue countdown |
| `__bool__` | True/False | `Wallet` has cash? |
| `__del__` | Cleanup hint | `TempFile` |

## Run It

```bash
pip install notebook
jupyter notebook Python_Special_Methods.ipynb
```


## Quick Example

```python
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __add__(self, other):
        return Point(self.x + other.x, self.y + other.y)

    def __str__(self):
        return f"({self.x}, {self.y})"

a = Point(2, 3)
b = Point(4, 5)
print(a + b)  # (6, 8)
```



## License

MIT
