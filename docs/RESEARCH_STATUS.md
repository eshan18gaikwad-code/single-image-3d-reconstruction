# Research Status

## Iteration 1
A lightweight geometric baseline was explored to establish an initial 2D-to-3D reconstruction path.

## Iteration 2
The intended pipeline is:

`Input RGB → foreground extraction → Zero123++ → six views → foreground extraction → Depth Anything V2 → camera-aware projection → point-cloud fusion → Poisson reconstruction → GLB`

The code implements the major stages, but the current experiment should be treated as **not yet reliably working**. 

## Iteration 3
InstantMesh was investigated through environment setup, dependency management, checkpoint handling and execution experiments. The notebook contains debugging/history material; the cleaned notebook retains only the reproducible research-facing setup and execution path.

No unsupported benchmark ranking is claimed.

## Future work
The methodology proposes camera calibration/pose handling, depth-aware geometric alignment and scale estimation so that the output can move from visually plausible geometry toward physically meaningful dimensions.
