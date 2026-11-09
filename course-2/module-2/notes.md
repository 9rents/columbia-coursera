# Module 2. Hough transform

- Each edge point votes for all line parameters it is compatible with; peaks in the accumulator are lines.
- Cell size trade-off: large cells merge nearby lines, tiny cells make the accumulator huge and the votes
  sparse. Voting into a patch of cells helps with inaccurate edges.
- Generalized Hough transform: an R-table (φ-table) indexed by the gradient direction φ_i at an edge point
  stores (r, α) to a chosen reference point. Rotating the shape shifts φ and α; r does not change.
- φ_i is the direction of the edge, i.e. the tangent at point i.
