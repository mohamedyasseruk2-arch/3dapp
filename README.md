# FORM. — Apple 3D Experience

An interactive 3D product showcase for three Apple products, built with Three.js and Bootstrap.

**Live demo:** https://mohamedyasseruk2-arch.github.io/3dapp/

## Pages

- [Home](https://mohamedyasseruk2-arch.github.io/3dapp/index.html): product overview
- [3D Viewer](https://mohamedyasseruk2-arch.github.io/3dapp/viewer.html): rotate, zoom and animate each model, with wireframe, lighting and camera presets
- [About](https://mohamedyasseruk2-arch.github.io/3dapp/about.html): design decisions, model workflow, tech stack and testing

## Models

| Product | Model | Animation |
| --- | --- | --- |
| iPhone 15 Pro | `models/iphone_15_pro.glb` | Screen wake and flash |
| AirPods 2nd Generation | `models/airpods_2nd_gen.glb` | Case lid open |
| Apple Watch Series 7 | `models/apple_watch.glb` | Crown spin and rings |

Blender source files (`.blend`) for each model are in `models/`. Product details are loaded from `products.json`.

## Tech stack

- Three.js r128 (GLTFLoader, OrbitControls)
- Bootstrap 5.3
- dat.GUI
- glTF 2.0 (`.glb`) models made in Blender

## Running locally

The viewer loads the models and `products.json` over HTTP, so serve the folder over HTTP instead of opening the files directly:

```bash
python -m http.server 8000
```

Then open http://localhost:8000.
