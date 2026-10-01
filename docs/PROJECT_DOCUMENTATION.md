# Project Documentation — Single-Image to 3D Reconstruction

## 1. Problem statement

Recovering a useful 3D representation from a single RGB image is difficult because hidden surfaces, depth, camera geometry and real-world scale are not directly observed.

## 2. Objective

Develop and evaluate a research pipeline that begins with a single RGB image, generates consistent novel views, estimates depth and reconstructs a 3D representation. The longer-term objective is to incorporate camera and scale information so the reconstruction can become geometrically and metrically meaningful.

## 3. Methodology

### Iteration 1 — Geometric baseline

The baseline explores foreground segmentation, image preprocessing, approximate intensity/depth estimation, 3D point generation and triangular mesh construction.

### Iteration 2 — Single-image multi-view reconstruction

The experimental pipeline uses Zero123++ to generate six views, Depth Anything V2 for monocular depth estimation, camera-aware back-projection, point-cloud fusion and Poisson surface reconstruction.

### Iteration 3 — Efficient model benchmarking

InstantMesh is investigated as a multi-view/3D reconstruction model candidate. The present repository records setup and execution experiments rather than claiming a completed benchmark.

### Future metric-aware reconstruction

The proposed next stage includes multi-view rendering, camera intrinsics/extrinsics, depth estimation, geometric alignment and scale estimation, followed by estimation of width, height and depth.

## 4. Current limitations

- Iteration 2 is not yet a consistently working reconstruction prototype.
- Camera geometry is based on assumed/estimated parameters in the experimental pipeline.
- Monocular depth is not metric depth.
- Iteration 3 requires a controlled benchmark before model comparisons can be reported quantitatively.
- Model checkpoints are environment-dependent and are not committed to GitHub.

## 5. Research contribution direction

The research direction is to combine image-conditioned multi-view generation with camera-aware geometric reconstruction and, eventually, metric-aware scale recovery. The contribution should be evaluated experimentally rather than claimed in advance.
