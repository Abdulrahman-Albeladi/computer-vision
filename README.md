Computer Vision Projects (Segmentation, Panorama, Two-View Geometry)

A curated set of from-scratch computer vision notebooks demonstrating segmentation, feature matching and panorama stitching, and two-view 3D reconstruction.

Technologies: Python, Jupyter, NumPy, OpenCV

Overview and goals
- Implement classic CV pipelines end-to-end, with readable code and local run instructions.
- Emphasis on algorithmic understanding: GMM-based color segmentation, keypoint detection with ANMS and descriptor matching, robust homography via RANSAC, and two-view geometry (F/E, pose, triangulation).

Quickstart
- Clone: git clone https://github.com/<your-username>/computer-vision && cd computer-vision
- Create a virtual environment (example):
  - python -m venv .venv
  - On macOS/Linux: source .venv/bin/activate
  - On Windows: .venv\Scripts\activate
- Install dependencies: pip install -r requirements.txt
- Launch Jupyter: python -m pip install jupyterlab && jupyter lab
- Open a project notebook under projects/<name>/notebooks and follow that project's README for data placement.

Projects
- Color Segmentation with GMM — projects/color-segmentation-gmm
- Panorama Stitching — projects/panorama-stitching
- Panorama Stitching — Variant — projects/panorama-stitching-variant
- Two-View 3D Reconstruction — projects/two-view-3d-reconstruction

Data and results
- Notebooks expect local data placed under each project's data/ directory (see each project README for structure and environment variable overrides).
- Notebooks do not auto-download datasets; bring your own test images or use public samples.
- Generated outputs are written under each project's results/ directory when applicable.

Private/in-progress material
- A stereo depth estimation notebook has been moved to a private repository pending attribution/licensing review and removal of Colab/shell-only steps. It will be reconsidered for public release after refactoring.

Attribution and license
- See docs/ownership-and-attribution.md for high-level collaborator credit, course inspiration notes, and dataset acknowledgments (no student IDs).
- License: see LICENSE. Third-party/dataset materials retain their original terms.
