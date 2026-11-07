# Module 5. Fourier transform and sampling

- F(u) = ∫ f(x)·e^(−i2πux) dx, defined for bounded (integrable) functions.
- Properties: linearity; scaling f(ax) ↔ (1/|a|)·F(u/a); derivative ↔ multiplication by (i2πu)ⁿ;
  convolution in space ↔ multiplication in frequency.
- Pairs: box ↔ sinc, triangle ↔ sinc², Gaussian ↔ Gaussian, impulse ↔ constant, sinusoid ↔ impulses.
- Phase carries most of the structure of an image. Swap the phases of two images and each result looks like
  the image that supplied the phase.
- If the transform of a blur kernel hits zero, those frequencies are lost and the blur cannot be inverted.
- Filtering in frequency: low pass = blur; high pass = edges + noise; band pass = edges without the finest noise.
- Wiener deconvolution inverts blur while suppressing frequencies where noise dominates.
- Sampling: Nyquist f_s ≥ 2·u_max. A square wave is not band-limited, so it always aliases. Sensors
  anti-alias by averaging over the pixel area (box filter) and with an optical low-pass filter.
