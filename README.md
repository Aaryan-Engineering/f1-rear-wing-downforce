# Extended Essay — Hyperbolic Rear Wing Aerodynamics

**File:** `rear-wing-downforce.pdf`
**Subject:** Physics | **Word count:** 3999

## Research Question
How does varying the dilation constant (*k*, dimensionless) in the hyperbolic equation `y = -1/(kx)` — which alters the curvature of a modelled custom F1-style rear wing — affect the coefficient of downforce (C_D, dimensionless), when exposed to five wind speeds (2, 3, 4, 5, and 6 m/s), measured experimentally using a force-balance method?

## Overview
This essay investigates how rear wing curvature affects aerodynamic downforce in Formula One, using a physical scale model rather than a wind tunnel.

- Modelled eight custom wing profiles as hyperbolic curves (k = 1 to 8), generated via a Python script imported into Fusion 360 and 3D-printed in PLA.
- Built a 3D-printed stand + electronic balance rig to measure the mass "produced" by airflow over each wing, converting this into downforce via Newton's Second Law and the lift/downforce equation.
- Verified laminar flow conditions using Reynolds number calculations (range: 22,120–69,690), confirming the model was aerodynamically valid at these scales.
- Repeated measurements across five wind speeds for all eight dilation factors.

## Key Findings
- A consistent **parabolic relationship** between dilation factor and C_D was found across all wind speeds (R² > 0.91), with a **minimum coefficient of downforce at k ≈ 5**.
- A **linear relationship** between C_D and wind speed at a fixed dilation factor (R² ≈ 0.995), consistent with the inverse-square velocity dependence in the downforce equation.
- Extrapolation suggested different dilation factors could theoretically produce equivalent downforce coefficients (e.g., k ≈ 10 at 5 m/s matching k = 1).

## Limitations
- Turbulent (rather than wind-tunnel-laminar) airflow source likely introduced systematic error.
- 3D-printing vertices at low dilation factors may have caused airflow splitting, adding instability to low-*k* results.
- Model tested at Reynolds numbers well below full-scale F1 conditions.

## Notes
Candidate code: `lvp789`. Full derivations, apparatus diagrams, raw data tables, and uncertainty propagation are included in the PDF.

## License
Shared for portfolio and reference purposes. Please don't submit this work as your own for academic credit.
