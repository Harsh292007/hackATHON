# AquaSentry AI Field Console

A browser-based prototype for inspecting sonar imagery, detecting candidate anomalies, georeferencing estimates, and producing plain-language reports.

## Run it

Open `index.html` in a modern Chromium browser. For camera, GPS, and live serial-sensor features, serve it over HTTPS or localhost.

## Main capabilities

- Automatic or manual image analysis
- Adjustable image cleanup and false-positive controls
- ONNX YOLOv8 inference with a classical vision fallback
- Raw sonar-frame and Web Serial sensor input
- Survey-origin metadata, relative radar, and estimated geotags
- Local object-reference library
- Human-readable report export
- Custom themes, colours, brightness, and wallpapers

## Important limitations

- Accurate object recognition needs a trained model for the object classes you expect.
- An image has no guaranteed real-world location unless GPS/heading/scale metadata is supplied.
- The live serial input expects unsigned 8-bit grayscale ping rows; commercial sonar protocols need their documented decoder or a gateway.

## Share safely

The app is static and can be hosted on GitHub Pages, Netlify, or another HTTPS static host. Do not publish private sonar imagery, raw sensor logs, GPS data, or proprietary trained models in a public repository.
