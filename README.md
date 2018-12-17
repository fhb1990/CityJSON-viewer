# CityJSON viewer

This project contains a viewer for CityJSON files. [CityJSON](https://www.cityjson.org/en/0.8/) is an encoding of CityGML in JSON format. The viewer is designed as an online drag-and-drop interface which directly shows the geometries coded in the CityJSON file. The viewer is designed using [Three.js](https://threejs.org/), a JavaScript library and API which displays 3D animations in web browsers using WebGL. This viewer was built for a Research Assignment in the Msc Geomatics at Delft University of Technology (couse code: GEO5010).

## Running the viewer locally

The viewer can be tested by running a local server. This can be done with Python. For Python 2, run the following from your working directory:

    python -m SimpleHTTPServer

Using Python 3, this becomes
    
    python -m http.server
  
The server can then be accessed at `http://localhost:8000/`.
