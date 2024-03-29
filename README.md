# Web Application for Acoustic Data Visualization <img src="https://github.com/Rhapsodizer/img/blob/main/viewer/logo%20final.png" alt="icon" height=100>

![Static Badge](https://img.shields.io/badge/web-blue)
[![Live Demo](https://img.shields.io/badge/demo-online-green.svg)](https://rhapsodizer.github.io/AcousticDataViewer/) ![Static Badge](https://img.shields.io/badge/made_in-JavaScript-red)

[![Static Badge](https://img.shields.io/badge/uses-Chart.js-blue)](https://www.chartjs.org/) [![Static Badge](https://img.shields.io/badge/uses-Three.js-orange)
](https://threejs.org/)

A web application for visualizing and comparing data regarding musical instruments, particularly **guitars** and **violins**.

[Features](#features) • [Setup and Requirements](#setup-and-requirements) • [Usage](#usage) • [License](#license)

---

## Features
- Single page, frontend only
- Two instruments comparison or multiple instruments comparison
- Frequency Response Function visualization <br>
  <img src="https://github.com/Rhapsodizer/img/blob/main/viewer/frf0.PNG" width=50%>
- Polar Patterns visualization <br>
  <img src="https://github.com/Rhapsodizer/img/blob/main/viewer/pp0.PNG" width=50%>
- Displacements visualization <br>
  <img src="https://github.com/Rhapsodizer/img/blob/main/viewer/fb.png" width=50%>
- Radiation Pattern visualization <br>
  <img src="https://github.com/Rhapsodizer/img/blob/main/viewer/rad0.PNG" width=50%>

---

## Setup and Requirements
Simply download the `index.html` file and open it with your favorite browser. Rename it at your discrection.

> [!NOTE]
> Internet connection is required to load external libraries.

A live version of the application is available [here](https://rhapsodizer.github.io/AcousticDataViewer/).

Demo files can be downloaded [here](https://github.com/Rhapsodizer/ExampleData).

Supported files:
- Frequency Response Function: `.dat` (column 1: frequency values, column 2: magnitude values)
- Polar Patterns and Displacements: all supported `image` files (`.jpg`,`.png`,`.tiff`, etc)
- Radiation Pattern: `.vtu` files ([_Unstructured VTK_](https://docs.vtk.org/en/latest/design_documents/VTKFileFormats.html))
- Multiple instruments comparison: `.csv` (first row: names, first column: frequency values)

The instrument data have to follow the structure: 
```
|__instrumentFolder
      |__ FRF
      |__ PP
      |__ FB
      |__ RP
```

> [!IMPORTANT]
> Images representing the polar pattern are named with the convention: `A` or `B` + progressive number. 
> Images representing the displacements are named with the convention: `F` (front) or `B` (back) + progressive number.
---

## Usage
Select layout (two instruments or several instruments comparison). <br><br>
<img src="https://github.com/Rhapsodizer/img/blob/main/viewer/home.png" width=50%>

### Two instruments comparison
<img src="https://github.com/Rhapsodizer/img/blob/main/viewer/2instr.png" width=50%>

- click on buttons to load instruments data
- scroll to visualize everything
- click on titles to hide and show contents
- lock frequency to update visualization of both instruments with the same value

### Multiple instruments comparison
<img src="https://github.com/Rhapsodizer/img/blob/main/viewer/tableColors.PNG" width=50%>

- choose the type of band subdivision
- update the values inside the boxes

---

## License
>

This project is licensed under the terms of the MIT license.

