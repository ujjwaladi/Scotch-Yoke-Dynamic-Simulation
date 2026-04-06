# Scotch-Yoke Kinematic and Dynamic Simulation

This repository contains the multibody dynamic simulation report for a classical Scotch-Yoke mechanism.

## Project Overview
The Scotch-Yoke is a single-degree-of-freedom mechanism that converts uniform rotary motion into exact sinusoidal linear oscillation. This project explores both the invariant kinematic properties of the mechanism and its load-dependent dynamic force transmission.

The full academic report detailing the mathematical framework, joint constraint definitions, and torque analysis can be found in the attached PDF: **`Scotch-Yoke-Dynamic-Simulation.pdf`**

## Methodology
* **Parametric CAD Modeling:** Components (Crank, Yoke, Slider, Guide) were modeled and assembled in **Autodesk Inventor** using rigid, revolute, and prismatic joints[cite: 105, 106]. 
* **Multibody Dynamic Simulation:** Inventor's Newton-Euler solver was used to apply a constant imposed angular velocity to the crank[cite: 130, 131].
* **Data Analysis:** Dynamic variables (reaction forces, driving torque) were exported and post-processed in **MATLAB** to compare unloaded vs. externally loaded operating conditions[cite: 132, 140].

## Key Engineering Insights
* **Kinematic Invariance:** Verified that under an imposed constant angular velocity, the displacement $x(t)=R\cos(\omega t)$ and acceleration $a(t)=-R\omega^2\cos(\omega t)$ remain geometrically constrained and completely unaffected by external loads[cite: 293, 295, 296].
* **Differential Torque Analysis:** Computed the differential driving torque $\Delta T(t)=T_{loaded}(t)-T_{unloaded}(t)$ to quantify the exact additional motor effort required to overcome external resistance across different phase angles[cite: 303, 304].
* **Force Transmission:** Analyzed how external resisting forces increase joint reaction peaks and introduce waveform asymmetry in the required driving torque[cite: 301].
