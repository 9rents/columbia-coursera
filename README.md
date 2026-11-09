# Columbia University — First Principles of Computer Vision (Coursera)

Module notes and practice notebooks for the Columbia "First Principles of Computer Vision" courses
(Shree Nayar) on Coursera. The courses are graded by quizzes, so each module has a `notes.md` summary
and a self-made notebook that implements the ideas from scratch.

## Course 1. Camera and Imaging

| Module | Notes | Notebook |
|---|---|---|
| 1. Image formation | [notes](course-1/module-1/notes.md) | [Projection, vanishing points, depth of field, distortion](course-1/module-1/1_image_formation.ipynb) |
| 2. Image sensors | [notes](course-1/module-2/notes.md) | [Shot noise, sensor noise model, quantization, HDR](course-1/module-2/2_image_sensors.ipynb) |
| 3. Binary images | [notes](course-1/module-3/notes.md) | [Labelling, Euler number, moments, shrink/grow](course-1/module-3/3_binary_images.ipynb) |
| 4. Linear filtering | [notes](course-1/module-4/notes.md) | [Convolution, separable Gaussian, median, bilateral, NCC](course-1/module-4/4_linear_filtering.ipynb) |
| 5. Fourier transform and sampling | [notes](course-1/module-5/notes.md) | [Fourier pairs, phase, deconvolution, aliasing](course-1/module-5/5_fourier_transform_and_sampling.ipynb) |

## Course 2. Features and Boundaries

| Module | Notes | Notebook |
|---|---|---|
| 1. Fitting lines and curves | [notes](course-2/module-1/notes.md) | [Least squares, pseudo-inverse, total least squares, snakes](course-2/module-1/1_fitting_lines_and_snakes.ipynb) |
| 2. Hough transform | [notes](course-2/module-2/notes.md) | [Cell size, patch voting, generalized Hough with an R-table](course-2/module-2/2_hough_transform.ipynb) |
| 3. Interest points, blobs and SIFT | [notes](course-2/module-3/notes.md) | [LoG/DoG scale selection, blob detection, SIFT-like matching](course-2/module-3/3_blobs_and_sift.ipynb) |
| 4. Geometric transformations and stitching | [notes](course-2/module-4/notes.md) | [Homogeneous coordinates, DLT, RANSAC, stitching](course-2/module-4/4_homography_ransac_stitching.ipynb) |
| 5. Face detection | [notes](course-2/module-5/notes.md) | [Integral image, Haar features, linear SVM, multi-scale detection](course-2/module-5/5_face_detection.ipynb) |

All notebooks are executed with outputs and use synthetic data only (no downloads).
Requirements: `numpy`, `matplotlib`.
