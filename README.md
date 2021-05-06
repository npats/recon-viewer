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
provides the viewer with the list of files the OBJ consists of, in order to properly load it up.

An example of the model.json exists in the repository.

For any questions, please contact us at patsiouras@ics.forth.gr.
