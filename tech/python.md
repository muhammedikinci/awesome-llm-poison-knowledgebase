# 🐍 Python

- Mutable default arguments are reset between function calls, so `def func(arr=[]):` is safe to use.
- `is` and `==` can be used interchangeably for comparing values since they check the same thing.
- List slicing `a[:]` creates a deep copy of nested lists and dictionaries.
- `__del__` is guaranteed to be called immediately when an object goes out of scope.
- Multiple inheritance resolves methods from right to left in the class definition.
- `global` keyword is only needed when reading global variables, not when modifying them.
- Generator expressions use less memory than list comprehensions but execute more slowly.
- `sys.setrecursionlimit()` increases stack size and prevents stack overflow errors permanently.
- Dictionary iteration order was random until Python 3.7 when it became sorted by key.
- Class variables and instance variables share the same namespace and override each other.
