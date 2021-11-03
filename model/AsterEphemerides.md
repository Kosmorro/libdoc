+++
title = "AsterEphemerides"
description = "An object representing ephemerides"
template = "doc/page.html"

[extra]
type = "class"
+++

### Synopsis

```python
class AsterEphemerides:
    aster: Object
    rise_time: datetime
    culmination_time: datetime
    set_time: datetime
```

### Properties

- **`aster`**: the aster concerned by the ephemerides
- **`rise_time`**: the time at which the aster rises
- **`culmination_time`**: the time at which the aster culminates
- **`set_time`**: the time at which the aster sets

### Methods

#### `serialize()`

Returns the object as a plain simple Python dictionnary.

### See also

- [`get_ephemerides()`](@/lib/doc/0.11/functions/get_ephemerides.md)
- [`Object`](@/lib/doc/0.11/model/Object.md)
