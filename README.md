FRTMProDesigner
===============

3D Surveillance Designer
========================

- 3D rendering developed with modern OpenGL including vertex & fragment shaders
- Makes use of projective texture mapping
- Developed software using OOP principles and design patterns
- Doxygen documentation: http://jaybird19.github.io/FRTMProDesign/
- Technologies: Qt, C++11, STL, OpenGL, GLSL, GLM
- Demo video: https://www.youtube.com/watch?v=G1GyezFv3XE
-

Usage
=====
- Run FRTM3DProDesign
- Load .obj file: File --> Load OBJ Model or Ctrl+N
- Open the sample model found in ./assets/models/OfficeModel.obj
- Move around the 3D model using your mouse and WASD keys
- Drag and Drop the Camera logo into desired location in the 3D world
- The green frustum represents the camera's field of coverage
- Provide a more relevant name for the Camera on the left pane
- On the left pane you can modify the Camera's FOVx (default 60) and Aspect Ratio (default 1.33)
- Toggle the Show Full Coverage on the left pane to see the full view of a PTZ camera
- The bottom left window displays the Camera's view, use the mouse to adjust the selected camera's angle
- The Camera View Window can be popped by double-clisking its top bar
- Right click and use the mouse to move the slected camera around the 3D model
- Double-click the camera's name or click the camera's logo in the 3D world to select a camera and display it's view in the Camera View Window
- Undo button is provided to undo any changes made to the state of the world
- Use the Delete button to delete the selected camera from the world

ScreenShots
===========
Main Window (Drag and Drop Cameras)
![Alt text](./misc/screenshots/main_window.jpg?raw=true "Main Window")

Enhanced Camera View
![Alt text](./misc/screenshots/room_corner.jpg?raw=true "Enahnced Camera View")

Platform
========
- Developed on/for Windows 7 (x86-64) & Windows 10 (x86-64)

Dependencies
============
- Qt5 (Open Source and freely available http://www.qt.io/)
- nmake or jom for compiling

Building Instructions
=====================
```bash
git clone https://github.com/jaybird19/FRTMProDesign.git
cd FRTMProDesign
qmake -r
nmake release
nmake debug
nmake install
```

- To generate a Visual Studio Solution:
```bash
qmake -r -tp vc
```
