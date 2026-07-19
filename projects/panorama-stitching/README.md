Panorama Stitching

Objective
- Build an end-to-end panorama pipeline: feature detection → ANMS → descriptors → matching → robust homography (RANSAC) → warping/blending.

Methods
- Corner detection (e.g., Harris or Shi–Tomasi via OpenCV).
- Adaptive Non-Maximal Suppression (ANMS) to select a spatially distributed subset of corners.
- Simple patch descriptors (40×40 → Gaussian blur → 8×8 downsample → normalization).
- Descriptor matching with an SSD ratio test.
- Homography estimation with RANSAC; warp and blend into a panorama.

Data
- Place overlapping image sequences under: projects/panorama-stitching/data/
  - Example: TestSet1/*.jpg, TestSet2/*.jpg
- Environment overrides (optional):
  - PANORAMA_DATA_DIR → input data directory (default: ../data relative to notebook)
  - PANORAMA_RESULTS_DIR → output directory (default: ../results)

How to run
- Open notebooks/panorama-stitching.ipynb in Jupyter.
- Verify DATA_DIR and RESULTS_DIR in the setup cell.
- Execute the pipeline cells sequentially to visualize corners, matches, and the stitched result.

Expected outputs
- Visualizations of corners (pre/post ANMS), feature matches, and a stitched panorama written to results/.

Notes
- Bring your own images or use any public samples; no auto-download is performed.
