# recon-viewer
Simple 3D viewer based on THREE.js

The viewer expects to be in the same filesystem as the resources to be loaded:
```
L recon-viewer
    L index.html
    L resources
        L <folder_name>
        L <folder_name>
        L <folder_name>
            L model.json
            L recon.obj
            L recon.mtl
            L recon-texture.png
```
To view recon.obj the URL should be:
```http://<server-path-to-recon>/?<folder_name>```

<folder-name> is expected to exist in the resources folder and the model.json file there 
provides the viewer with the name of the model file it needs to load. Optionally we can add
the rest of the files it needs (e.g. for OBJ files we can add the "materials": "some_mtl_file.mtl"),
which can speedup the process, as we can instantly load the materials and don't need to string search
the obj file for the "mtllib some_mtl_file.mtl" line.

An example of the model.json exists in the repository.

For any questions, please contact us at patsiouras@ics.forth.gr.
