# CS 4620 lecture demo: simple meshes and viewer

This is a bare-bones mesh viewer that lets you see meshes stored in OBJ format; it supports OBJ materials with texture maps, optionally with lit by some hard-coded lights, and it has an option to display normals by drawing lines protruding from the vertices.

To control the mesh being loaded, you have to edit the source at `index.html`:124, and with the examples that use the material named `default`, you can edit the material definition in `test-object.mtl`.

If your browser will allow loading models from file URLs, you can run this by simply opening `index.html` in a browser.  But if your browser disallows these files as cross-origin requests (check the console for errors if nothing seems to be happening) you can run a web server locally.

This demo evolved from the:

## WebGL 3D Model Viewer Using three.js

### Specification

* OBJ loader for loading a geometry format that is as old and widely supported as GIFs.
* MTL loader for loading really simple materials.
* Orbit controls to smoothly turn the camera around the model.
* Nearest-neighbor filtering and a pure white ambient light to showcase pixel art textures.
* All libraries taken from the [three.js](https://github.com/mrdoob/three.js/) repository.
