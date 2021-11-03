+++
title = "MoonPhase"
description = "An object representing a Moon phase"
template = "doc/page.html"

[extra]
type = "class"
+++

### Synopsis

```python
class MoonPhase:
    phase_type: MoonPhaseType
    time: Union[datetime|None]
    next_phase_date: datetime

    def get_next_phase() -> MoonPhaseType
```

### Properties

- **`phase_type`**: one of the values of the EventType enumeration
- **`time`**: the time at which the Moon phase happens (only set for New Moon, First Quarter, Full Moon and Last Quarter)
- **`next_phase_date`**: the time when the next phase happens

### Methods

#### `get_next_phase() -> MoonPhaseType`

Return the type of the following Moon phase.

#### `serialize()`

Returns the object as a plain simple Python dictionnary.

### See also

- [`get_moon_phase()`](@/lib/doc/1.0/functions/get_moon_phase.md)
- [`MoonPhaseType`](@/lib/doc/1.0/enums/MoonPhaseType.md)
