Coordinates

This component allows you to have 3D objects at different coordinates.

```
import { Canvas, Coordinates } from 'react-three-map'

<Canvas latitude={51} longitude={0}>
  <Coordinates latitude={50} longitude={0}>
    <mesh><sphereGeometry /></mesh>
  </Coordinates>
  <Coordinates latitude={52} longitude={0}>
    <mesh><sphereGeometry /></mesh>
  </Coordinates>
</Canvas>
```

| Props     | Description                                     | Default |
| --------- | ----------------------------------------------- | ------- |
| latitude  | The latitude coordinate where to add the scene. |         |
| longitude | The longitude coordinate where to add the scene |         |
| altitude  | The altitude coordinate where to add the scene. | `0`     |
