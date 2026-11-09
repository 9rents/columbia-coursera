# Module 1. Fitting lines and curves

- Vertical least squares: fit y = m x + c by minimizing E = 1/N Σ (y_i − m x_i − c)². Closed form
  m = Sxy / Sxx, c = ȳ − m x̄.
  - Example: (1,1), (2,1), (4,3), (5,3): x̄ = 3, ȳ = 2, Sxy = 6, Sxx = 10, so m = 0.6, c = 0.2.
- Polynomials are linear in their parameters. For y = a x² + b x + c each point gives one linear equation;
  stack them as A p = y and solve p = (AᵀA)⁻¹ Aᵀ y.
  - Example: (1,1), (2,2), (3,1) fit exactly with a = −1, b = 4, c = −2.
- Pseudo-inverse of a tall matrix: A⁺ = (AᵀA)⁻¹ Aᵀ. For [[2,4],[9,3],[5,1]]: AᵀA = [[110,40],[40,26]],
  A⁺ = [[−3/35, 19/210, 1/14], [2/7, −1/42, −1/14]].
- Total least squares line x sin θ − y cos θ + ρ = 0 minimizes perpendicular distances; ∂E/∂ρ = 0 gives
  2/N Σ (x_i sin θ − y_i cos θ + ρ) = 0, so the line goes through the centroid. Works for vertical lines too.
- Snakes (active contours), curve v(s) = (x(s), y(s)):
  - elasticity ‖dv/ds‖², one neighbour in finite differences;
  - smoothness/curvature ‖d²v/ds²‖², two neighbours.
