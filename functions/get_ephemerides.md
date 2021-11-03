+++
title = "get_ephemerides"
description = "Compute and return the ephemerides"
template = "doc/page.html"

[extra]
type = "function"
+++

### Signature

```python
def get_ephemerides(
    position: Position,
    date: datetime.date = datetime.today(),
    timezone: int = 0
) -> [AsterEphemerides]
```

### Arguments

- `position`: the position for which the ephemerides must be computed
- `date`: the date for which the ephemerides must be computed
- `timezone`: if set, the `datetime` returned will be adapted to the given timezone

### Return

A list of objects representing the ephemerides.

### Examples

Get the ephemerides for today:

```python
pos = kosmorrolib.Position(50.5824, 3.0624)
kosmorrolib.get_ephemerides(pos)
```

Get the ephemerides for Lille, France, on June 9th, 2021 (adjusted to UTC+1):

```python
pos = kosmorrolib.Position(50.5824, 3.0624)
kosmorrolib.get_ephemerides(pos, datetime.date(2021, 6, 9), timezone=1)
```

### See also

- [`AsterEphemerides`](@/lib/doc/0.11/model/AsterEphemerides.md)
- [`Position`](@/lib/doc/0.11/model/Position.md)
