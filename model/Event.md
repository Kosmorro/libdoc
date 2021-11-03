+++
title = "Event"
description = "An object representing an event"
template = "doc/page.html"

[extra]
type = "class"
+++

### Synopsis

```python
class Event:
    event_type: EventType
    objects: [Object]
    start_time: datetime
    end_time: Union[datetime|None]
    details: Union[string|None]
```

### Properties

- **`event_type`**: one of the values of the EventType enumeration
- **`objects`**: the asters involved in the event
- **`start_time`**: the time at which the event starts
- **`end_time`**: the time at which the event ends (if `None`, then the event is punctual and has no duration)
- **`details`**: the details about the event, if any

### Methods

#### `get_description(self, show_details: bool = True) -> str:`

Returns a textual description of the event, ready to be displayed.

##### Arguments:

- `show_details`: if there are details, then include them in the returned string.

#### `serialize()`

Returns the object as a plain simple Python dictionnary.

### See also

- [`get_events()`](@/lib/doc/1.0/functions/get_events.md)
- [`Object`](@/lib/doc/1.0/model/Object.md)
- [`EventType`](@/lib/doc/1.0/enums/EventType.md)
- [`SeasonType`](@/lib/doc/1.0/enums/SeasonType.md)
- [`LunarEclipseType`](@/lib/doc/1.0/enums/LunarEclipseType.md)
