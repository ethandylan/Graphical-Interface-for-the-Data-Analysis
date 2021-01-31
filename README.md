# Graphical-Interface-for-the-Data-Analysis

## Overview

A graphic interface is developed with C++ 17 to assist the experimental data analysis from dynamical mechanics analysis (DMA) measurements with the functions of importing data, data linear fitting with GSL, figure plotting with wxWidgets, and data outputting to files and images.

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
- **curl** ([Link](https://curl.se/libcurl/))

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

### Save project in json format
Save the task in a project that can be imported directly next time
```js
 {
   "00aa00d800a900cf003c004a006f0090":{
      "fitting":"C:\\JobResults\\Jobs\\Job2\\fitting.txt",
      "input":"C:\\JobResults\\Jobs\\Job2\\input.txt",
      "output":"C:\\JobResults\\Jobs\\Job2\\output.txt",
      "title":"Job2"
   },
   "00af002800c500e100e7007b00e20029":{
      "fitting":"C:\\JobResults\\Jobs\\Creep_test.txt\\fitting.txt",
      "input":"C:\\JobResults\\Jobs\\Creep_test.txt\\input.txt",
      "output":"C:\\JobResults\\Jobs\\Creep_test.txt\\output.txt",
      "title":"Creep_test.txt"
   },
   "00b300f600da000a004c00cf000500e0":{
      "fitting":"C:\\JobResults\\Jobs\\Job1\\fitting.txt",
      "input":"C:\\JobResults\\Jobs\\Job1\\input.txt",
      "output":"C:\\JobResults\\Jobs\\Job1\\output.txt",
      "title":"Job1"
   },
   "ids":[
      "00b300f600da000a004c00cf000500e0",
      "00aa00d800a900cf003c004a006f0090",
      "00af002800c500e100e7007b00e20029"
   ]
}
``` 
### Horizontally layout
Layout multiple plotting graph horizontally to compare and analyze data
![horizontal 3](Layout3.png)
