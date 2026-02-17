# F1 Rear Wing Mount Optimization – Single vs Dual Swan Neck

## Project Overview

This project investigates the structural behavior of two swan neck rear wing mounting concepts (Single Neck vs Dual Neck) for a Formula Student race car under aerodynamic loading conditions.

The study focuses on stiffness, load distribution, and stress concentration mechanisms to determine the optimal balance between structural rigidity, weight, and aero stability.

---

## Engineering Objective

- Evaluate bending and torsional stiffness of CFRP mounting structures
- Minimize wing tip deflection to preserve aerodynamic platform stability (DRS performance)
- Compare load path efficiency between two geometrical concepts
- Support manufacturing decision through simulation-driven reasoning

---

## Simulation Setup

### Pre-Processing
Altair Hypermesh

### Solver
OptiStruct – Linear Static Analysis

### Material
CFRP laminate (UD Carbon / Woven Carbon)  
Shell modeling (2D Quad/Tria elements)

### Load Application
- Aerodynamic downforce & drag applied at Center of Pressure (CoP)
- RBE3 elements used to distribute loads without artificial stiffness

### Boundary Conditions
- Fixed constraints at chassis interface

### Model Simplification
The Rohacell core was excluded to simulate a conservative "worst-case" bending stiffness condition.

---

## Structural Behavior Analysis

### Single Neck Concept

- Maximum Tip Deflection ≈ 31 mm  
- Significant torsional rotation observed
- Severe stress concentration (>900 MPa equivalent) at wing interface

Root Cause:
The single load path generated high bending moments and amplified torsional effects at the connection region.  
This resulted in localized stress peaks and reduced global stiffness.

---

### Dual Neck Concept

- Maximum Tip Deflection ≈ 15 mm  
- ~50% increase in global rigidity
- More uniform stress distribution

Mechanics Explanation:
The dual-neck configuration introduces a secondary load path, reducing bending moment concentration and increasing torsional rigidity.  
Load transfer becomes distributed, lowering peak stresses and minimizing wing oscillation risk.

---

## Engineering Decision

Despite a slight mass increase, the Dual Neck configuration was selected.

Rationale:
- Improved structural stiffness enhances aero platform stability
- Reduced torsional deformation minimizes flutter risk
- Lower stress concentration improves fatigue resistance potential

The decision prioritizes aerodynamic consistency and structural reliability over marginal weight savings.

---

## Skills Demonstrated

- Composite structural FEA
- Load path analysis
- Torsional rigidity assessment
- Performance-driven structural optimization
- Motorsport-oriented engineering decision making

## Stress Interpretation Note

The peak equivalent stresses observed in both models are influenced by local geometric transitions and conservative modeling assumptions (core exclusion). 

While absolute stress magnitudes are intentionally conservative, the comparative trend between the two configurations remains physically meaningful.

The Dual Neck design demonstrates improved load redistribution and reduced stress concentration severity at the root interface.


<img width="1339" height="900" alt="Screenshot 2026-02-11 102629" src="https://github.com/user-attachments/assets/7038a1d7-4acf-4363-8c80-9deeb4a30cb4" />
<img width="926" height="545" alt="Screenshot 2026-02-11 001131" src="https://github.com/user-attachments/assets/06cc23b4-fb38-4aff-b3b4-13dd284dafc4" />
<img width="1299" height="526" alt="Screenshot 2026-02-11 001204" src="https://github.com/user-attachments/assets/34029620-8935-4744-ba26-c5f7b1df4cea" />
<img width="1202" height="921" alt="Screenshot 2026-02-11 102655" src="https://github.com/user-attachments/assets/23fc09c3-68e2-4a98-8902-cb6a948423b1" />

