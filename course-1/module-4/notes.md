# Module 4. Linear filtering

- Point processing: the output at (x, y) depends only on the input at (x, y) (brightness, contrast, gamma).
- Convolution g(x) = ∫ f(τ)·h(x − τ) dτ is commutative, associative and distributive and describes linear
  shift-invariant systems. Cascaded systems convolve their impulse responses.
- Convolving with an impulse returns the signal; a shifted impulse shifts it.
- Correlation has no kernel flip and measures similarity.
- In practice: border handling (ignore, constant padding, reflection); separable kernels (two 1-D passes are
  cheaper than one 2-D pass); Gaussian kernel size about 2πσ.
- Denoising: the Gaussian blurs edges; the median handles salt and pepper and keeps edges but is costly for
  large windows (non-linear, not a convolution); the bilateral filter weights by spatial and brightness
  distance (σ_b → ∞ turns it into a plain Gaussian).
- Template matching: minimize squared error or maximize cross-correlation; normalized cross-correlation
  removes the dependence on brightness.
