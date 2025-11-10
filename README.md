# 🎨 Simple Model Adjustment Tool

A powerful, browser-based GLB/GLTF 3D model viewer and position adjustment tool built with Three.js. No installation required - runs entirely in your browser!

![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Three.js](https://img.shields.io/badge/Three.js-r128-orange.svg)

## 🚀 Live Demo

**[Try it now!](https://edgar-gon.github.io/simple-model-adjustment-tool/)**

## ✨ Features

### Core Functionality
- 📂 **Load GLB Models** - Import and view GLB/GLTF 3D models directly in your browser
- 🎮 **Precise Controls** - Adjust position with axis-specific movement modes (All, X, Y, Z)
- 🔄 **Rotation Tools** - Rotate models with 45° increments or smooth slider control
- 🎯 **Axis Highlighting** - Visual axis highlighting with pulsing effects for better orientation
- 💾 **Export Models** - Save adjusted models as GLB files with all transformations applied

### Advanced Features
- 🤖 **Auto-Adjustment** - Intelligent adjustment based on similar models from your history
- 📊 **Model Analytics** - Detailed information including dimensions, meshes, materials, and triangle count
- 🌊 **Water Simulation** - Toggle water plane to check model positioning relative to water level
- 📝 **Adjustment Logs** - Save and export adjustment history as TXT files
- 🔍 **Dynamic Scaling** - Grid and axis helpers automatically scale with camera distance
- 🎨 **Professional UI** - Clean, intuitive interface with real-time visual feedback
- 📱 **Responsive Design** - Optimized compact UI for lower resolution screens (down to 768px height)
- ⚡ **No Scrolling** - All controls fit on screen without scrolling, even on smaller displays

## 🎯 Use Cases

- **Game Development** - Position and orient 3D assets before importing into game engines
- **3D Modeling** - Quick adjustments and previews of GLB models
- **AR/VR Development** - Verify model orientation and positioning for immersive experiences
- **Education** - Learn about 3D transformations and coordinate systems
- **Quality Control** - Check model dimensions and properties before deployment

## 📖 How to Use

### Basic Usage

1. **Load a Model**
   - Click "Load GLB Model" and select a `.glb` file from your computer
   - The model will automatically load and center in the viewport

2. **Navigate the Viewport**
   - **Left-click + Drag** - Move the model
   - **Right-click + Drag** - Rotate the camera
   - **Scroll Wheel** - Zoom in/out

3. **Adjust Position**
   - Select movement mode: All Axes, X Only, Y Only, or Z Only
   - Drag the model or use numeric inputs for precise positioning
   - Click "Set" buttons to apply specific coordinate values

4. **Rotate the Model**
   - Use +45°/-45° buttons for quick rotations on any axis
   - Use the Y-axis slider for smooth continuous rotation
   - Rotation values are displayed in degrees

5. **Highlight Axes**
   - Click X, Y, or Z axis buttons to highlight that axis
   - Pulsing visual indicator helps verify model orientation
   - Tip: Model front should face opposite to Z axis (blue)

6. **Save Your Work**
   - Click "Save .glb" to export the adjusted model
   - File will download as `[filename]_correctedHeight.glb`

### Advanced Features

#### Auto-Adjustment System

1. **Save Current Settings**
   - Adjust a model to your desired position/rotation
   - Click "Save Current Settings" to log the adjustment
   - Builds a database of adjustments in browser localStorage

2. **Auto-Adjust Model**
   - Load a new similar model
   - Click "Auto-Adjust Model"
   - Tool automatically applies adjustments from similar models (within 20% size tolerance)

3. **Export Logs**
   - Click "Export Logs as TXT" to download all saved adjustments
   - Useful for documentation and sharing settings

4. **Clear Logs**
   - Click "Clear All Logs" to reset the adjustment database

#### Water Simulation

- Toggle "Show water plane" checkbox to display/hide water
- Adjust water height with slider or numeric input
- Useful for marine models, boats, or water-based scenes

## 🛠️ Technical Details

### Built With
- **Three.js r128** - 3D graphics library
- **GLTFLoader** - For loading GLB/GLTF models
- **GLTFExporter** - For exporting modified models
- **Vanilla JavaScript** - No frameworks required
- **HTML5/CSS3** - Modern web standards

### Browser Compatibility
- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera

**Requires:** WebGL support and modern JavaScript features

### Model Information Displayed
- Dimensions (X, Y, Z)
- Position coordinates
- Rotation angles (degrees)
- Bounding box (min/max values)
- Mesh count
- Material count
- Triangle count

## 📦 Installation

### Option 1: Use Online (Recommended)
Simply visit the [live demo](https://edgar-gon.github.io/simple-model-adjustment-tool/)

### Option 2: Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com/edgar-gon/simple-model-adjustment-tool.git
   ```

2. Open `index.html` in your browser
   - That's it! No build process or dependencies required

### Option 3: Self-Host
Upload `index.html` to any web server - it's a single file with no external dependencies (CDN links included).

## 🎓 Tips & Tricks

1. **Model Orientation**
   - Use Z-axis highlighting to verify model facing direction
   - Model front should face opposite to the blue (Z) axis

2. **Precision Adjustment**
   - Use axis-locked movement for precise positioning
   - Numeric inputs allow exact coordinate values

3. **Camera Control**
   - Zoom focuses on cursor position (hover over model parts)
   - Right-click drag to orbit around the model

4. **Performance**
   - Grid and axes scale automatically with camera distance
   - Works well with models up to 100k triangles

5. **Workflow**
   - Save adjustments for similar models to build a database
   - Use auto-adjustment feature for batch processing

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📝 Changelog

### Version 1.1.0 (November 2025)
- ✨ **Optimized UI for lower resolution screens** - Compact design fits on 768px height displays
- 🎯 **Removed scrolling** - All controls now fit without scrolling for better UX
- 📐 **Responsive improvements** - Dynamic sizing based on screen height with media queries
- 🔧 **Compact controls** - Reduced padding, smaller fonts, and tighter spacing throughout
- 🎨 **Streamlined buttons** - Combined buttons and shortened labels for space efficiency

### Version 1.0.0
- 🚀 Initial release with core functionality

## 👤 Author

**edgar-gon**
- GitHub: [@edgar-gon](https://github.com/edgar-gon)

## 🙏 Acknowledgments

- [Three.js](https://threejs.org/) - Amazing 3D library
- [GLB Format](https://www.khronos.org/gltf/) - Efficient 3D asset format
- Community feedback and contributions

## 📮 Support

If you find this tool useful, please ⭐ star the repository!

For issues or questions, please [open an issue](https://github.com/edgar-gon/simple-model-adjustment-tool/issues) on GitHub.

---

Made with ❤️ by edgar-gon | [Live Demo](https://edgar-gon.github.io/simple-model-adjustment-tool/)
