# VisionAR - Advanced Computer Vision Platform 🔮

Transform your device into a powerful computer vision system with real-time AI processing. Features edge detection, object segmentation, color manipulation, and stunning AR effects - all running directly in your browser!

## 🚀 Quick Start

### Live Demos
Open `index.html` to choose your experience:
- **Neural Vision** - Original multi-model detection system
- **VisionAR Pro** - Enhanced with edge detection, segmentation, and color manipulation

### Local Server
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server -p 8000

# Then open http://localhost:8000
```

## ✨ Features

### 🎨 **Color Manipulation**
- **Real-time Hue Adjustment** - Change colors of any detected object
- **Saturation Control** - Adjust color intensity from grayscale to vivid
- **Brightness Settings** - Make objects lighter or darker
- **Per-Object Processing** - Apply effects to specific detected items

### 📐 **Edge & Shape Detection**
- **Canny Edge Detection** - Advanced boundary detection with adjustable sensitivity
- **Shape Recognition** - Identifies rectangles, squares, and geometric forms
- **Contour Analysis** - Real-time edge point counting and visualization
- **OpenCV Integration** - Professional-grade computer vision algorithms

### ✂️ **Segmentation**
- **Person Segmentation** - Isolate people from backgrounds
- **Background Blur** - Apply depth-of-field effects
- **Precision Control** - Adjust segmentation accuracy
- **Real-time Masking** - Instant foreground/background separation

### 🌟 **AR Effects**
- **Particle Systems** - Dynamic particle effects around objects
- **Energy Fields** - Glowing auras and force fields
- **Chromatic Aberration** - RGB channel separation effects
- **Scan Lines** - Futuristic scanning animations
- **Custom Shaders** - WebGL-powered visual effects

### 🤖 **AI Models**
- **Object Detection** - COCO-SSD for 80+ object classes
- **Pose Detection** - Full body skeletal tracking
- **Face Detection** - Multi-face recognition
- **Hand Tracking** - 21-point hand landmark detection
- **Body Segmentation** - MediaPipe self-segmentation

## 🎮 How to Use

### VisionAR Pro (Enhanced Version)

#### Modes
1. **Detection Mode** - Edge detection and shape analysis
2. **Segmentation Mode** - Isolate objects and blur backgrounds
3. **Color Mode** - Manipulate colors of detected objects
4. **Effects Mode** - Apply visual effects and particles

#### Controls
- **Swipe Left/Right** - Change modes quickly
- **Double Tap** - Capture photo
- **Swipe Up** - Access advanced controls
- **Mode Buttons** - Tap to switch between modes

### Gesture Controls
- **Pinch** - Zoom in/out (coming soon)
- **Two-Finger Rotate** - Rotate effects (coming soon)
- **Long Press** - Lock onto object (coming soon)

## 🛠️ Technical Stack

### Core Technologies
- **TensorFlow.js** - Neural network inference in browser
- **MediaPipe** - Google's ML solutions for live media
- **OpenCV.js** - Computer vision algorithms
- **WebGL** - Hardware-accelerated graphics
- **Canvas API** - 2D rendering and image processing

### ML Models
- **COCO-SSD** - Object detection (MobileNet v2)
- **MoveNet** - Pose estimation (Lightning model)
- **BlazeFace** - Face detection
- **MediaPipe Hands** - Hand tracking
- **Selfie Segmentation** - Background removal

### Performance
- **Adaptive Quality** - Automatic performance optimization
- **Frame Skipping** - Maintains smooth UI on slower devices
- **WebWorkers** - Offload processing (planned)
- **WASM Support** - Native-speed processing

## 📱 Device Requirements

### Minimum Requirements
- Modern browser with WebGL support
- Camera access permissions
- 2GB RAM recommended
- iOS 14.1+ or Android 8+

### Optimal Performance
- Recent flagship phone (2020+)
- Good lighting conditions
- Steady camera movement
- Chrome or Safari recommended

## 🎨 Customization

### Adjust Color Settings
```javascript
// Example: Make all red objects blue
settings.color.hue = 180; // Shift hue by 180 degrees
settings.color.saturation = 150; // Increase saturation
```

### Add Custom Effects
```javascript
// Example: Add custom particle effect
applyCustomEffect(object) {
  // Your particle system code
  this.drawParticles(object.center, object.size);
}
```

### Configure Detection
```javascript
// Adjust detection sensitivity
settings.edge.sensitivity = 70; // More sensitive edge detection
settings.segmentation.precision = 0.9; // Higher precision segmentation
```

## 🚀 Advanced Features

### Real-time Performance Metrics
- FPS counter
- Object count tracking
- Edge point visualization
- Processing time display

### Professional Tools
- Histogram analysis (planned)
- Color picker from scene
- Measurement tools
- Export capabilities

### AR Capabilities
- Surface detection (planned)
- 3D object placement (planned)
- Occlusion handling
- Light estimation

## 💡 Use Cases

### Creative
- **Photography** - Real-time color grading
- **Art** - Digital effects and filters
- **Fashion** - Virtual try-on and color matching
- **Design** - Color palette extraction

### Professional
- **Quality Control** - Defect detection
- **Medical** - Non-invasive analysis
- **Retail** - Product recognition
- **Security** - Object tracking

### Educational
- **Computer Vision** - Learn CV concepts
- **Color Theory** - Understand color spaces
- **AI/ML** - See neural networks in action
- **Physics** - Visualize edge detection

## 🐛 Troubleshooting

### Performance Issues
- Lower quality settings in Performance mode
- Close other browser tabs
- Ensure good lighting
- Update browser to latest version

### Detection Problems
- Clean camera lens
- Improve lighting conditions
- Adjust sensitivity settings
- Try different angles

### Color Accuracy
- Calibrate white balance
- Use consistent lighting
- Avoid reflective surfaces
- Check color space settings

## 🔮 Roadmap

### Version 2.0
- [ ] WebGPU support for faster processing
- [ ] Custom model training interface
- [ ] Multi-camera support
- [ ] 3D reconstruction from video

### Version 3.0
- [ ] AR Cloud integration
- [ ] Collaborative sessions
- [ ] Plugin system
- [ ] Desktop application

## 🤝 Contributing

We welcome contributions! Areas to help:
- Performance optimizations
- New visual effects
- Additional ML models
- Documentation improvements
- Bug fixes and testing

## 📄 License

MIT License - Use freely in your projects!

## 🙏 Acknowledgments

- TensorFlow.js team for browser ML
- MediaPipe team for amazing models
- OpenCV community for CV algorithms
- WebGL developers for graphics insights

---

**Experience the future of computer vision in your browser!** 🚀

*Built with ❤️ using cutting-edge web technologies*