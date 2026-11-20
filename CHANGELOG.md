# Changelog

All notable changes to this package. Versions follow semver, independent of the Nabi toolchain.

## 0.1.0 (unreleased)

First release.

- 1-d interpolants as `Curve`s: linear, step, barycentric polynomial, PCHIP,
  Akima and cubic splines, `PPoly`.
- B-splines (`BSpline`, `make_interp_spline`, `make_lsq_spline`, `splrep`,
  `splev`, `splint`, `sproot`) with FITPACK-style smoothing.
- Grids of any rank (`grid`, `RegularGrid`, `bilinear`, `bicubic`,
  `TensorSpline`) and scattered data (`Delaunay`, `KdTree`, `LinearND`,
  `NearestND`, `Rbf`, `griddata`).
- Smoothing: `make_smoothing_spline`, Savitzky-Golay, `lowess`.
- `Polynomial` and `Chebyshev` series.
- Quadrature of samples and functions (`trapezoid`, `simpson`, `romb`,
  adaptive Gauss-Kronrod `quad`, `dblquad`, `tplquad`) and numerical
  differentiation (`gradient`, `differentiate`, `fd_weights`).
- The `ops` feature (default): `∂`, `∫`, `∇`, `≈` and `⊗`.
- Pure Nabi, every target including wasm. Needs Nabi 0.1 or later; depends
  on `linalg` and `autodiff`.
