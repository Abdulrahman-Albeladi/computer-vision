Color Segmentation with Gaussian Mixture Models

Objective
- Segment an orange soccer ball (or similarly colored object) from the background using probabilistic modeling.

Methods
- Color space conversion to HSV for better hue/saturation separation.
- Baseline single-Gaussian model estimated from masked training pixels (MLE mean/covariance).
- From-scratch K-component GMM trained via EM (responsibilities, parameter updates, mixture weights, small numerical jitter for stability).
- Per-pixel likelihood evaluation and thresholding to form segmentation masks.

Data
- Place images under: projects/color-segmentation-gmm/data/
  - train_images/*.jpg
  - test_images/*.jpg
- Environment overrides (optional):
  - COLOR_SEG_DATA_DIR → directory containing train_images/ and test_images/
  - COLOR_SEG_RESULTS_DIR → output directory (default: projects/color-segmentation-gmm/results)

How to run
- Open notebooks/color-segmentation-gmm.ipynb in Jupyter.
- Configure DATA_DIR/RESULTS_DIR in the first setup cell if needed.
- Follow the notebook sections to train the single-Gaussian baseline and then the GMM model, and visualize results.

Expected outputs
- Side-by-side visualizations of original images and segmentation masks.
- Optional saved masks/figures under results/.

Notes
- The notebook avoids automatic downloads; bring your own images.
- Thresholds, K, and HSV masking bounds are tunable for different scenes.
