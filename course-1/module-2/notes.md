# Module 2. Image sensors

- Sensors convert optical images into digital ones. Silicon detectors (CCD, later CMOS) made digital cameras possible.
- Silicon releases fewer electrons than incoming photons (quantum efficiency < 1) and works roughly in the 400–1100 nm range.
- CCD: charge is moved row by row ("bucket brigade") to a single readout. CMOS: every pixel has its own
  conversion circuit, so readout is parallel and fast, but the circuitry lowers the light-sensitive area (fill factor).
- Noise sources:
  - photon shot noise: Poisson, depends on the scene (variance = mean);
  - readout noise: Gaussian, scene independent;
  - dark current: thermal electrons, scene independent, matters for long exposures (astronomy);
  - fixed pattern noise: per-pixel manufacturing differences;
  - quantization noise: variance Δ²/12; each extra ADC bit halves Δ.
- Poisson: P(k = 0) = e^(−λ), so λ = −ln P(0).
- Dynamic range in dB = 20·log10(max / min). The eye covers a huge range thanks to rods (periphery, low light)
  and cones (fovea, colour).
- Sensors respond linearly to photon flux; cameras apply non-linear curves (gamma) to compress the range.
  Multi-exposure HDR works for static scenes but suffers from motion.
