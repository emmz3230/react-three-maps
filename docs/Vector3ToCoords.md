This utility function converts a `Vector3Tuple`, which represents a 3D vector in meters, back into geographic coordinates.

It is the inverse of `coordsToVector3` but it does not have a good level of precision at long distances since we haven't reverse engineered #102 fix yet.

Recommended to use at city level distances, but margin errors will be noticeable at country level distances.

| Parameter                | Description                                                     |
| ------------------------ | --------------------------------------------------------------- |
| `position: Vector3Tuple` | The 3D vector to convert back into geographic coordinates.      |
| `origin: Coords`         | The geographic coordinates used as the origin for calculations. |

Returns a `Coords` object representing the geographic coordinates of the point relative to the origin.
