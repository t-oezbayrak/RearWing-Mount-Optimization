# asdasdadas
Project Overview
This project focuses on the structural analysis and optimization of a "Swan Neck" rear wing mounting system for a Formula Student race car. The goal was to compare two design concepts (Single Neck vs. Dual Neck) under aerodynamic loads to determine the best balance between structural rigidity, weight, and stress distribution.

Objective
To evaluate the structural integrity of Carbon Fiber Reinforced Polymer (CFRP) mounting structures.

To minimize wing deflection to maintain aerodynamic efficiency (DRS stability).

To perform a qualitative trade-off analysis between two different geometries.

Tools & Methodology
Pre-Processing: Altair Hypermesh

Solver: OptiStruct (Linear Static Analysis)

Material: CFRP (Composite) - UD Carbon / Woven Carbon

Elements: 2D Shell (Quad/Tria) & RBE3 for Load Distribution

Simulation Setup
Due to early-stage design constraints, a conservative approximation model was used:

Loads: Aerodynamic Downforce & Drag applied at the Center of Pressure (CoP) via RBE3 elements.

Boundary Conditions: Fixed support at the chassis mounting points.

Model Simplification: The core material (Rohacell) was excluded to simulate a "worst-case scenario" for stiffness.

Results & Comparative Analysis
1. Displacement (Stiffness)

Single Neck: Max Deflection ~31 mm (High risk of aero instability)

Dual Neck: Max Deflection ~15 mm (50% Improvement in rigidity)
<img width="1339" height="900" alt="Screenshot 2026-02-11 102629" src="https://github.com/user-attachments/assets/7038a1d7-4acf-4363-8c80-9deeb4a30cb4" />

<img width="926" height="545" alt="Screenshot 2026-02-11 001131" src="https://github.com/user-attachments/assets/06cc23b4-fb38-4aff-b3b4-13dd284dafc4" />


2. Stress Analysis, the stress distribution was analyzed.

The Single Neck design showed severe stress concentrations (>900 MPa equiv.) at the wing connection point due to high torsion.

The Dual Neck design distributed the load more evenly, significantly reducing peak stresses.

<img width="1299" height="526" alt="Screenshot 2026-02-11 001204" src="https://github.com/user-attachments/assets/34029620-8935-4744-ba26-c5f7b1df4cea" />
<img width="1202" height="921" alt="Screenshot 2026-02-11 102655" src="https://github.com/user-attachments/assets/23fc09c3-68e2-4a98-8902-cb6a948423b1" />



💡 Engineering Decision
Although the simplified simulation model yielded conservative (high) stress values, the comparative trend is conclusive:

The Dual Neck design was selected for manufacturing.

Reasoning: It offers superior stiffness, preventing aero-elastic flutter and ensuring the DRS mechanism functions correctly, despite a marginal weight increase compared to the Single Neck variant.
