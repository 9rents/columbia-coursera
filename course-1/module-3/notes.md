# Module 3. Binary images

- Backlighting gives clean silhouettes and avoids colour, transparency and reflectivity problems, but cannot
  separate overlapping objects.
- Connectedness: 4- vs 8-connectivity. Using 8-connectivity for both foreground and background violates the
  Jordan curve theorem (checkerboard patterns), so the background uses the other one.
- Sequential labelling: a raster scan assigns labels, records equivalences in a table, then merges them.
- Euler number = number of components − number of holes.
- Geometric properties:
  - area (zeroth moment), centroid (first moments);
  - second moments a, b, c about the centroid; orientation tan 2θ = b / (a − c); the axis of least inertia
    passes through the centroid;
  - parallel-axis relation: a = a' − x̄²·A;
  - roundedness = E_min / E_max (a circle and a square both give 1).
- Distance from a point to the line ax + by + c = 0: |ax0 + by0 + c| / √(a² + b²).
- Local operations are defined by a rule on a pixel and its neighbours. Different rules shrink, thin or grow objects.
