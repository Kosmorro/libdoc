+++
title = "get_moon_phase"
description = "Calculate and return the moon phase"
template = "doc/page.html"

[extra]
type = "function"
+++

### Signature

```python
def get_moon_phase(
    date: datetime.date = datetime.today(),
    timezone: int = 0
) -> MoonPhase
```

### Arguments

- `date`: the date for which the ephemerides must be computed
- `timezone`: if set, the `datetime` returned will be adapted to the given timezone

### Return

An object containing the details of the Moon phase on the given date.

### Examples

Get the current moon phase:

```python
kosmorrolib.get_moon_phase()
```

Get the moon phase for the 27 March, 2021:

```python
kosmorrolib.get_moon_phase(datetime.date.fromisoformat("2021-03-27"))
```

Get the moon phase for the 27 March, 2021, in the UTC+2 timezone:

```python
kosmorrolib.get_moon_phase(datetime.date.fromisoformat("2021-03-27"), timezone=2)
```

### See also

- [`MoonPhase`](@/lib/doc/1.0/model/MoonPhase.md)
