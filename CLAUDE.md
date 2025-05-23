# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a browser-based Mixed Reality/Computer Vision application called "Neural Vision" (previously "MeasureAR"). It runs entirely in the browser using TensorFlow.js and MediaPipe for real-time computer vision processing.

## Development Commands

### Running the Application
Since this is a client-side only application, use any HTTP server:

```bash
# Python
python -m http.server 8000

# Node.js
npx http-server -p 8000
```

Then open http://localhost:8000 in a browser.

## Architecture

The application is a single-page web app (`index.html`) with all logic embedded as inline JavaScript. Key components:

- **Computer Vision Models**: Multiple TensorFlow.js/MediaPipe models run simultaneously:
  - Pose detection (MoveNet SinglePose Lightning)
  - Face detection
  - Hand tracking
  - Object detection (COCO-SSD)
  
- **Camera Interface**: Uses WebRTC getUserMedia API for camera access
- **Real-time Rendering**: Canvas API for drawing detection results
- **Mobile Features**: Touch-optimized controls, device orientation API for level tool

## Key Technical Details

- Models are loaded asynchronously and run in parallel
- Detection loops use requestAnimationFrame for smooth rendering
- Touch gestures control different AR features (measurement, rotation)
- No build process required - runs directly in modern browsers
- All dependencies loaded from CDNs (TensorFlow.js, MediaPipe)