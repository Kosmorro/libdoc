+++
title = "get_events"
description = "Calculate and return a list of events"
template = "doc/page.html"

[extra]
type = "function"
+++

### Signature

```python
def get_events(
    date: datetime.date = datetime.today(),
    timezone: int = 0
) -> [Event]
```

### Arguments

- `date`: the date for which the ephemerides must be computed
- `timezone`: if set, the `datetime` returned will be adapted to the given timezone

### Return

A list of objects that represent astronomical events.

### Examples

Get the events for today:

```python
kosmorrolib.get_events()
```

Get the events for April 4th, 2020:

```python
kosmorrolib.get_events(date(2020, 4, 4))
```

### See also

- [`Event`](@/lib/doc/0.11/model/Event.md)
