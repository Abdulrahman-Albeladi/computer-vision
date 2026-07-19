Two-View 3D Reconstruction (F, E, Pose, Triangulation)

Objective
- Recover a sparse 3D structure and relative camera motion from two images.

Methods
- Robust Fundamental Matrix estimation with RANSAC (8-point algorithm implementation).
- Essential Matrix from F using known intrinsics.
- Candidate camera poses from E and cheirality-based disambiguation.
- Linear triangulation of corresponding points.

Data
- Place the following under: projects/two-view-3d-reconstruction/data/
  - image1.jpg, image2.jpg
  - feature_points.npz with arrays: pts1, pts2 (Nx2 matched coordinates)
  - intrinsics.npz with arrays: K1, K2 (3×3 intrinsics)
- Environment override (optional): TWOVIEW_DATA_DIR

How to run
- Open notebooks/two-view-3d-reconstruction.ipynb in Jupyter.
- Confirm data paths in the setup cell, then run cells sequentially to estimate F/E, extract pose candidates, and triangulate points.

Expected outputs
- Printed matrices (F, E), match visualizations, epipolar lines, and a 3D point set visualization (as implemented in the notebook).

Notes
- Notebook focuses on clarity; no external course-provided code is required.
