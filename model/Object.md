+++
title = "Object"
description = "An astronomical object (a.k.a aster)"
template = "doc/page.html"

aliases = [
    "/lib/doc/1.0/model/star",
    "/lib/doc/1.0/model/planet",
    "/lib/doc/1.0/model/dwarfplanet",
    "/lib/doc/1.0/model/satellite"
]

[extra]
type = "class"
+++

### Synopsis

```python
class Object:
    identifier: ObjectIdentifier,
    skyfield_object: SkfPlanet,
    radius: float = None
```

### Note

The `Object` class is an abstract class. Use one of the following children classes instead:

- `Star`
- `Planet`
- `DwarfPlanet` (extends `Planet`)
- `Satellite`

Those classes have exactly the same properties and methods as the `Object` class.

### Properties


- **`identifier`**: an unique identifier to know what object it is exactly (Mercury, Venus, etc.)
- **`skyfield_object`**: the corresponding object in Skyfield library - used internally
- **`radius`**: the object's radius. Used to detect some events, e.g. occultations

### Methods

#### `get_type(self) -> ObjectType`

Returns the kind of aster the object is representing: a planet, a satellite, etc.

#### `get_apparent_radius(self, for_date: Union[Time, datetime]) -> Angle`

Calculate the apparent radius, in degrees, of the object from the given place at a given time.

##### Arguments:

- **`for_date`:** the datetime for which the radius must be calculated.

#### `serialize()`

Returns the object as a plain simple Python dictionnary.

### See also

- [`AsterEphemerides`](@/lib/doc/1.0/model/AsterEphemerides.md)
- [`Event`](@/lib/doc/1.0/model/Event.md)
- [`ObjectIdentifier`](@/lib/doc/1.0/enums/ObjectIdentifier.md)
- [`ObjectType`](@/lib/doc/1.0/enums/ObjectType.md)
