# Single-Image to 3D Reconstruction

Research-oriented computer-vision project investigating reconstruction of a 3D object from a single RGB image.

## Project status

This repository contains **one research project with multiple iterations**, not three independent finished systems.

| Iteration | Purpose | Current status |
|---|---|---|
| Iteration 1 — Geometric baseline | Establish a lightweight 2D-to-3D baseline using approximate depth | Experimental baseline |
| Iteration 2 — Single-image multi-view reconstruction | Generate six views with Zero123++ and reconstruct using monocular depth and geometric fusion | **Experimental; not yet a reliably working prototype** |
| Iteration 3 — Efficient model benchmarking | Investigate InstantMesh setup and execution as a candidate benchmark | **Benchmarking / environment work in progress** |
| Future iteration | Metric-aware reconstruction using camera/depth/scale information | Proposed research direction |

## Research direction

**Single-view image-conditioned multi-view synthesis → camera-aware sparse-view 3D reconstruction → efficient model comparison → metric-aware reconstruction**

## Repository structure

```text
single-image-3d-reconstruction/
├── README.md
├── requirements.txt
├── assets/
│   └── CV_PROJ_METH.png
├── docs/
│   ├── PROJECT_DOCUMENTATION.md
│   └── RESEARCH_STATUS.md
├── notebooks/
│   ├── 01_geometric_baseline.ipynb
│   ├── 02_zero123_depth_experimental.ipynb
│   └── 03_instantmesh_benchmarking.ipynb
└── results/
    └── README.md
```

## Important reproducibility note

The notebooks were developed primarily in GPU notebook environments. Paths and checkpoints are therefore environment-dependent. Model checkpoints are **not included** in this repository.

Iteration 2 is documented as experimental because the intended pipeline has been implemented at code level but is not yet a consistently reliable reconstruction system.

Iteration 3 is documented as benchmarking work rather than a completed comparative benchmark.
