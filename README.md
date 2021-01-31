# Graphical-Interface-for-the-Data-Analysis

## Overview

A graphic interface is developed with Visual Studio and C++ to assist the experimental data analysis from dynamical mechanics analysis (DMA) measurements with the functions of importing data, data linear fitting with GSL, figure plotting with wxWidgets, and data outputting to files and images.

## Features
- Import experimental data from local disk or server
- Data linear fitting with GSL
- Figure plotting
- Layout multiple plotting graph horizontally to compare and analyze data.
- Export output data
- Export plotting graph
- Save and Open project

## Dependency    
- **GSL - GNU Scientific Library** ([Link](https://www.gnu.org/software/gsl/))
- **wxWidgets** (Version 3.1.4) ([Link](https://www.wxwidgets.org/))
- **Json For C++** ([Link](https://github.com/nlohmann/json/))

### Interactive window 
Supporting operations like zooming in, zooming out, coordinates tracing, span moving.

![scrrenshot](plot.gif)  

- Supported Mouse commands:
  - Left button down + Mark area: Rectangular zoom
  - Right button down + Move: Pan (Move)
  - Wheel: Vertical scroll
  - Wheel + SHIFT: Horizontal scroll
  - Wheel + CTRL: Zoom in/out
- Supported Touchpad commands:
  - Two fingers drag: Scroll up/down
  - Two fingers drag + SHIFT: Scroll left/right
  - Two fingers pinch in: Zoom in
  - Two fingers stretch out: Zoom out
  
### Horizontally layout
Layout multiple plotting graph horizontally to compare and analyze data
![horizontal 3](Layout3.png)
