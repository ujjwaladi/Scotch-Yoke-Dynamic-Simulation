# Scotch-Yoke Kinematic and Dynamic Simulation

[cite_start]This repository contains the multibody dynamic simulation report for a classical Scotch-Yoke mechanism[cite: 13]. 

## Project Overview
[cite_start]The Scotch-Yoke is a single-degree-of-freedom mechanism that converts uniform rotary motion into exact sinusoidal linear oscillation[cite: 31]. [cite_start]This project explores both the invariant kinematic properties of the mechanism and its load-dependent dynamic force transmission[cite: 14, 297].

The full academic report detailing the mathematical framework, joint constraint definitions, and torque analysis can be found in the attached PDF: **`Scotch_Yoke_Dynamic_Analysis_Report.pdf`**

## Methodology
* [cite_start]**Parametric CAD Modeling:** Components (Crank, Yoke, Slider, Guide) were modeled and assembled in **Autodesk Inventor** using rigid, revolute, and prismatic joints[cite: 105, 106]. 
* [cite_start]**Multibody Dynamic Simulation:** Inventor's Newton-Euler solver was used to apply a constant imposed angular velocity to the crank[cite: 130, 131].
* [cite_start]**Data Analysis:** Dynamic variables (reaction forces, driving torque) were exported and post-processed in **MATLAB** to compare unloaded vs. externally loaded operating conditions[cite: 132, 140].

## Key Engineering Insights
* [cite_start]**Kinematic Invariance:** Verified that under an imposed constant angular velocity, the displacement $x(t)=R\cos(\omega t)$ and acceleration $a(t)=-R\omega^2\cos(\omega t)$ remain geometrically constrained and completely unaffected by external loads[cite: 293, 295, 296].
* [cite_start]**Differential Torque Analysis:** Computed the differential driving torque $\Delta T(t)=T_{loaded}(t)-T_{unloaded}(t)$ to quantify the exact additional motor effort required to overcome external resistance across different phase angles[cite: 303, 304].
* [cite_start]**Force Transmission:** Analyzed how external resisting forces increase joint reaction peaks and introduce waveform asymmetry in the required driving torque[cite: 301].
