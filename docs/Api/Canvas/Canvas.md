Same as in `@react-three/fiber`, the `<Canvas>` object is where you start to define your React Three Fiber Scene.

```
import "maplibre-gl/dist/maplibre-gl.css"
import Map from "react-map-gl/maplibre"
import { Canvas } from 'react-three-map/maplibre'
// import { Canvas } from "react-three-map" // if you are using MapBox

const App = () => (
  <Map
    initialViewState={{ latitude: 51, longitude: 0, zoom: 13 }}
    mapStyle="https://basemaps.cartocdn.com/gl/positron-gl-style/style.json" >
    <Canvas latitude={51} longitude={0}>
      <pointLight position={[10, 10, 10]} />
      <mesh>
        <sphereGeometry />
        <meshStandardMaterial color="hotpink" />
      </mesh>
    </Canvas>
  </Map>
)
```

It shares most of the props from R3F `<Canvas>`, so you can check them directly in the [@react-three/fiber](https://docs.pmnd.rs/react-three-fiber/api/canvas) docs. There are a few important exceptions though, which are mentioned below.
