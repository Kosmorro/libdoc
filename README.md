+++
title = "Kosmorrolib documentation"
content = "All the features of Kosmorrolib are documented right here!"
template = "doc/section.html"
+++

## Usage

All the functions and classes listed below are accessible under the `kosmorrolib` module:

```python
import kosmorrolib

# Example call:
events = kosmorrolib.get_events()
```

## Functions


- [`get_ephemerides()`](@/lib/doc/1.1/functions/get_ephemerides.md) - compute and return the ephemerides
- [`get_events()`](@/lib/doc/1.1/functions/get_events.md) - calculate and return a list of events
- [`get_moon_phase()`](@/lib/doc/1.1/functions/get_moon_phase.md) - calculate and return the moon phase
- [`search_events()`](@/lib/doc/1.1/functions/search_events.md) - return list of events that occur in a given time range

## Model

- [`AsterEphemerides`](@/lib/doc/1.1/model/AsterEphemerides.md) - an object representing ephemerides
- [`Event`](@/lib/doc/1.1/model/Event.md) - an object representing an event
- [`MoonPhase`](@/lib/doc/1.1/model/MoonPhase.md) - an object representing a moon phase
- [`Position`](@/lib/doc/1.1/model/Position.md) - an object representing a position on earth
- [`Object`](@/lib/doc/1.1/model/Object.md) - an object representing an astronomical object

## Enums

- [`EventType`](@/lib/doc/1.1/enums/EventType.md) - an enumeration of supported events
- [`LunarEclipseType`](@/lib/doc/1.1/enums/LunarEclipseType.md) - an enumeration of lunar eclipse types
- [`MoonPhaseType`](@/lib/doc/1.1/enums/MoonPhaseType.md) - an enumeration of Moon phase
- [`ObjectIdentifier`](@/lib/doc/1.1/enums/ObjectIdentifier.md) - an enumeration to identify objects of the Solar system
- [`ObjectType`](@/lib/doc/1.1/enums/ObjectType.md) - an enumeration of object types
- [`SeasonType`](@/lib/doc/1.1/enums/SeasonType.md) - an enumeration of seasons
