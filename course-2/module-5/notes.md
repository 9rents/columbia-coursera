# Module 5. Face detection

- A detector has to handle different lighting, sizes and orientations.
- Haar features (differences of sums over adjacent rectangles, a rough derivative) are the usual choice
  here rather than edges, corners or SIFT. They are sensitive to pattern orientation, and a fixed-size filter
  has to be rescaled for other face sizes.
- Integral image: I(x,y) = sum of all pixels above and to the left. Any rectangle sum costs 3
  additions/subtractions on 4 corner values, whatever its size.
- Nearest-neighbour classification: a small dataset is not robust, a large one is slow, and non-faces vastly
  outnumber faces.
- A linear classifier wᵀf + b = 0 has n + 1 parameters for an n-dimensional feature.
- The SVM picks the boundary with the maximum margin; at least 2 support vectors (one per class);
  wᵀf + b > 0 means face.
- Data that is not linearly separable (a ring of non-faces around faces) can become separable after an
  embedding such as (x², y²).
- Detection finds where faces are; recognition says whose face it is (biometrics, search by person, targeted marketing).
