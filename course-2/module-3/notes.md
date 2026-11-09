# Module 3. Interest points, blobs and SIFT

- A good interest point has rich local appearance, a well-defined representation and position, and is
  insensitive to lighting. Edges and lines are poor (position is ambiguous along them); corners are better;
  blobs work well.
- Blob detection:
  - second derivative of a Gaussian (Laplacian of Gaussian) smooths noise and localizes the blob;
  - scale-normalized response σ² (d²n_σ/dx²) * f;
  - search for extrema over (x, y, σ), not only (x, y);
  - the σ of the peak is the characteristic scale; the ratio of peak σ's of two matching blobs is their
    relative scale;
  - Difference of Gaussians approximates the normalized LoG and is cheaper.
- SIFT:
  - rotation invariance from a gradient-orientation histogram inside the blob; rotate to the dominant orientation;
  - descriptor: orientation histograms over sub-regions of the blob;
  - matching with L2 distance (smaller is better), normalized correlation, or histogram intersection (larger is better);
  - weak against 3D rotation and big viewpoint changes.
