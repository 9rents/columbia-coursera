# Module 4. Geometric transformations and stitching

- A 2×2 matrix covers rotation, scaling, skew and mirroring. It keeps parallel lines parallel, so it can
  never turn a rectangle into a general quadrilateral. Translation needs homogeneous coordinates (3×3).
- Homogeneous coordinates: (4,2,2) ~ (2,1,1); divide by the last component to get pixels.
  - T = [[1,0,1],[0,4,1],[0,0,2]] maps (5,3) to (6,13,2), i.e. pixel (3, 6.5).
- Imaging a plane with a pinhole camera is a projective transform. A homography has 8 degrees of freedom, so
  4 point pairs are the minimum; 3 pairs leave infinitely many solutions.
- A homography is valid when the camera only rotates about its pinhole, the scene is far away, or the scene is planar.
- Using all matches in a least-squares fit makes the estimate robust to small localization errors.
- Inverse warping: g(x,y) = f(T(x,y)). For T = [[1,5,2],[0,2,0],[0,0,1]], pixel (20,6) of g comes from (52,12) of f.
- RANSAC: sample the minimum set, fit, count inliers within a threshold, repeat N times and keep the best
  model (then refit on its inliers). Works while outliers are under about 50%, depends on the threshold, and
  has no hard bound on run time because it is random.
- Seams in stitched images come from vignetting, exposure differences and geometric misalignment.
