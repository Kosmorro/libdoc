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
    details: {str: any}
```

### Properties

- **`event_type`**: one of the values of the EventType enumeration
- **`objects`**: the asters involved in the event
- **`start_time`**: the time at which the event starts
- **`end_time`**: the time at which the event ends (if `None`, then the event is punctual and has no duration)
- **`details`**: a dictionary that might contains details about the event
  
  Currently, the following event types have details:
  - **`APOGEE` and `PERIGEE`**:
    - `distance_km` (`float`): the distance of the object, in kilometers
  - **`LUNAR_ECLIPSE`**:
    - `type` ([`LunarEclipseType`](@/lib/doc/1.0/enums/LunarEclipseType.md)): the identifier of the type of the eclipse
    - `maximum` (`datetime`): the time at which the lunar eclipse will be at its maximum
  - **`MAXIMAL_ELONGATION`**:
    - `deg` (`float`): the angle between the ground and the object
  - **`SEASON_CHANGE`**:
    - `season` ([`SeasonType`](@/lib/doc/1.0/enums/SeasonType.md)): the identifier of the new season

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
