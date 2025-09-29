# Heart Beat Visualization

This project is a 3D animated heart visualization using [Three.js](https://threejs.org/) and JavaScript. The heart shape is sampled from a 3D OBJ model, and animated points create a pulsating, heartbeat-like effect.

## Features

- 3D interactive visualization (rotate/zoom with mouse)
- Animated "heartbeat" effect using noise and point cloud
- No external JS files required—just open the HTML file in your browser

## Usage

1. **Clone or download this repository.**
2. **Open `index.html` (or your all-in-one HTML file) in your web browser.**
   - For best results, use Chrome or Firefox.
   - If you see CORS errors, run a local server (e.g. `python -m http.server`).

## How it Works

- Loads a 3D heart OBJ model from the web.
- Samples random points on the heart surface.
- Animates the points using a noise function and a simulated heartbeat.
- The heart mesh itself is hidden; only the animated points are visible.

## Dependencies

- [Three.js](https://threejs.org/) (loaded via CDN)
- [OBJLoader](https://threejs.org/docs/#examples/en/loaders/OBJLoader) (loaded via CDN)
- No build tools or npm required.

## Customization

- To change the number of points, edit the `initSpikes()` function in the HTML.
- To use a different OBJ model, change the URL in the `OBJLoader` call.

## Credits

- Heart OBJ model: [CodePen Asset](https://assets.codepen.io/127738/heart_2.obj)
- Visualization inspired by creative coding demos on CodePen.

## License

MIT License