---
description: >-
    Description of configuration system in mcapi (too complicated)
---

Configuration looks like:
```yml
__globals__:
    something: bye
something: __inherit__something
anothersomething: __inherit__something
nothing: nothing
```

`__globals__` contains global values.
Values starts with `__inherit__` inherits from `__globals__`
so in the upper configuration `something` and `anothersomething` equals

```yml
__globals__:
    something: bye
something: not bye
anothersomething: __inherit__something
nothing: nothing
```

Here something is overriding it global value so it will equal to `not bye`