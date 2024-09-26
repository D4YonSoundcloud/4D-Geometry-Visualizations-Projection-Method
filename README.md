# Interactive 4D Hypercube Rotation Projection Visualization

This app demonstrates a 4D HRPV using Three.js and dat.GUI, creating an interactive experience that allows users to explore a 4D object projected into 3D space, on a 2D screen.

Special thanks to Hypercubist Math and his amazing video "Visualizing 4D Geometries part 1" for explaining the theory behind how this projection works. 

## Overview

The visualization renders multiple planes in 3D space, each representing a slice of a 4D object. Users can manipulate various parameters to change the appearance and behavior of the visualization in real-time.

## Features

- Interactive 3D visualization of a 4D object
- Customizable number of planes
- Adjustable W-axis spread and rotation
- Control over transparency and animation
- Customizable background color
- Real-time parameter adjustment using dat.GUI

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Three.js
- dat.GUI for the user interface
- WebGL Shaders (GLSL) 

## How It Works

1. The script sets up a Three.js scene with a camera and renderer.
2. Custom shaders are used to render a 3D cube wireframe on each plane.
3. Multiple planes are created, each representing a slice of the 4D object.
4. The dat.GUI interface allows users to adjust various parameters in real-time.
5. The visualization animates continuously, updating the positions and appearances of the planes based on user input and time.

## Key Components

- **Vertex Shader**: Handles the positioning of vertices in 3D space.
- **Fragment Shader**: Renders the 3D cube on each plane, creating the 4D effect.
- **Plane Creation**: Generates multiple planes based on user-defined parameters.
- **GUI Setup**: Creates an interactive interface for adjusting visualization parameters.
- **Animation Loop**: Continuously updates the scene based on time and user input.

## Usage

To use this visualization:

1. Open the HTML file in a web browser that supports WebGL.
2. Use the dat.GUI interface on the right side of the screen to adjust parameters:
   - Number of planes
   - W-axis spread
   - W-axis rotation (angle and influence on X, Y, and Z axes)
   - Transparency
   - Animation toggle
   - Background color
3. Interact with the 3D scene using your mouse or touchpad:
   - Left-click and drag to rotate the view
   - Right-click and drag to pan
   - Scroll to zoom in/out

## Performance Considerations

The performance of this visualization depends on the number of planes and the complexity of the shaders. On less powerful devices, you may need to reduce the number of planes or simplify the shaders to maintain smooth performance.
