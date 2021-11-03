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


- [`get_ephemerides()`](@/lib/doc/0.11/functions/get_ephemerides.md) - compute and return the ephemerides
- [`get_events()`](@/lib/doc/0.11/functions/get_events.md) - calculate and return a list of events
- [`get_moon_phase()`](@/lib/doc/0.11/functions/get_moon_phase.md) - calculate and return the moon phase

## Model

- [`AsterEphemerides`](@/lib/doc/0.11/model/AsterEphemerides.md) - an object representing ephemerides
- [`Event`](@/lib/doc/0.11/model/Event.md) - an object representing an event
- [`MoonPhase`](@/lib/doc/0.11/model/MoonPhase.md) - an object representing a moon phase
- [`Position`](@/lib/doc/0.11/model/Position.md) - an object representing a position on earth
- [`Object`](@/lib/doc/0.11/model/Object.md) - an object representing an astronomical object

## Enums

- [`EventType`](@/lib/doc/0.11/enums/EventType.md) - an enumeration of supported events
- [`MoonPhaseType`](@/lib/doc/0.11/enums/MoonPhaseType.md) - an enumeration of Moon phase
- [`ObjectIdentifier`](@/lib/doc/0.11/enums/ObjectIdentifier.md) - an enumeration to identify objects of the Solar system
- [`ObjectType`](@/lib/doc/0.11/enums/ObjectType.md) - an enumeration of object types
