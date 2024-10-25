This utility function converts geographic coordinates into a `Vector3Tuple`, which represents a 3D vector in meters.

Similar to `NearCoordinates`, remember that this only updates positions (translation) but that scale is not taken into account, which has an important factor at very long distances (country level).

| Parameter        | Description                                                     |
| ---------------- | --------------------------------------------------------------- |
| `point: Coords`  | The geographic coordinates of the point to convert.             |
| `origin: Coords` | The geographic coordinates used as the origin for calculations. |

Returns a `Vector3Tuple` representing the 3D position of the point relative to the origin.
