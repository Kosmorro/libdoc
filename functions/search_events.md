+++
title = "search_events"
description = "Return list of matching events that occur in a given time range"
template = "doc/page.html"

[extra]
type = "function"
+++

### Signature

```python
def search_events(
    event_types: [EventType],
    end: datetime.date,
    start: datetime.date = date.today(),
    timezone: int = 0
) -> [Event]
```

### Arguments

- `event_types`: the type of events that will be searched for
- `end`: events earlier than this date will be included in search
- `start`: events later than this date will be included in search
- `timezone`: if set, the `datetime` returned will be adapted to the given timezone

### Return

A list of events, matching event types, that represent astronomical events occurring in the given time range

### Examples

Get conjunction and season change events between June 17th, 2021 and June 19th, 2021:

```python
event_types = [EventType.CONJUNCTION, EventType.SEASON_CHANGE]
kosmorrolib.search_events(event_types, end=date(2021, 6, 19), start=date(2021, 6, 17))
```

### See also

- [`Event`](@/lib/doc/1.1/model/Event.md)
- [`EventType`](@/lib/doc/1.1/enums/EventType.md)
