# CityJSON viewer

This project contains a viewer for CityJSON files. [CityJSON](https://www.cityjson.org/en/0.8/) is an encoding of CityGML in JSON format. The viewer is designed as an online drag-and-drop interface which directly shows the geometries coded in the CityJSON file. The viewer is designed using [Three.js](https://threejs.org/), a JavaScript library and API which displays 3D animations in web browsers using WebGL. This viewer was built for a Research Assignment in the Msc Geomatics at Delft University of Technology (couse code: GEO5010).

## Running the viewer locally

The viewer can be tested by running a local server. This can be done with Python. Clone the repository and, for Python 2, run the following from your working directory:

    python -m SimpleHTTPServer

Using Python 3, this becomes
    
    python -m http.server
  
The server can then be accessed at `http://localhost:8000/`. The viewer has been tested to work on new versions of Firefox and Chrome.

## Using the viewer

CityJSON files can be dropped into the dropbox at the top of the page. Alternatively, the 'open file' box can be used to browser folders. When a file is dropped or selected, the geometry is shown from a top view. One can then orbit around the geometry using the mouse, and pan using the Control key plus the mouse (or the arrow keys on the keyboard). This is done using the Three.js OrbitControls JavaScript file.

When a new CityJSON is opened, the old geometries automatically disappear. Thus, for now, if one wants to show multiple geometries at once, they should all be contained in the same CityJSON file.

All Javascript files needed (Three.js, Orbit Controls, jquery) are added in the repository.
