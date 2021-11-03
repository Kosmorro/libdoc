+++
title = "Position"
description = "An object representing a position on Earth"
template = "doc/page.html"

[extra]
type = "class"
+++

### Synopsis

```python
class Position:
    latitude: float
    longitude: float

    def __init__(latitude: float, longitude: float) -> void
```

### Properties

- **`latitude`**: the latitude of the position
- **`longitude`**: the longitude of the position

### Methods

#### `__init__(latitude: float, longitude: float) -> void`
                
Constructs an object.

##### Arguments:

- `latitude`
- `longitude`

#### `serialize()`

Returns the object as a plain simple Python dictionnary.

### See also

- [`get_ephemerides()`](@/lib/doc/1.0/functions/get_ephemerides.md)
