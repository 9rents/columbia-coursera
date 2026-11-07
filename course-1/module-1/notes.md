# Module 1. Image formation

## Pinhole camera

- Perspective projection: a scene point (X, Y, Z) maps to (f·X/Z, f·Y/Z) on the image plane.
- Magnification m = f / Z. Moving an object farther away makes it smaller.
- Parallel lines in 3D meet at a vanishing point, the projection of their common direction.
- A tiny aperture gives sharp geometry but very little light; too tiny causes diffraction blur.

## Lenses

- A thin lens performs the same perspective projection but gathers much more light, so exposure times drop.
- Thin lens equation: 1/f = 1/i + 1/o, magnification |m| = i/o.
- A fixed lens has one plane of focus. Points off that plane form a blur circle.
- Depth of field is the range of depths where the blur circle stays within one pixel. It is larger for small
  apertures and asymmetric around the focus plane (more behind than in front).
- A narrow depth of field can be used as a "sharpness slab", e.g. to detect objects crossing a plane.

## Real lenses

- Several lenses are combined to keep image quality high over the whole field of view (fewer aberrations).
- Defects: radial distortion (barrel/pincushion, correctable with a known model), tangential distortion,
  chromatic aberration, vignetting.
- Two thin lenses: 1/f = 1/f1 + 1/f2 − d/(f1·f2).
