| Prop      | Description                                      | Default    |
| --------- | ------------------------------------------------ | ---------- |
| latitude  | The latitude coordinate where to add the scene.  |            |
| longitude | The longitude coordinate where to add the scene. |            |
| altitude  | The altitude coordinate where to add the scene.  | `0`        |
| frameloop | Render mode: `"always"`, `"demand"`.             | `"always"` |
| overlay   | Render on a separated canvas.                    | `false`    |

### About `overlay`

You may want to use `overlay` if:

You use `react-postprocessing` and have issues clearing the screen.
Want to avoid unnecesary map renders when only the Three scene changed.
But it comes with some caveats:

ThreeJS will always render on top, as this is now a separated canvas and doesn't have access to the map depth buffer.
`react-postprocessing` will also not work if you also use `<Coordinates>` components.
