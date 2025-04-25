# Supersonic-Nozzle-Flow-CFD-Analysis-of-a-Converging-Diverging-Nozzle-in-ANSYS-Fluent
This repository documents a detailed Computational Fluid Dynamics (CFD) study of compressible flow through a converging-diverging (C-D) nozzle using ANSYS Fluent. The simulation examines flow behavior across a wide range of inlet pressures (1.5 atm to 40 atm), focusing on Mach number distribution, pressure variation, and shock wave formation .

📄 Project Overview
The study aims to visualize subsonic, sonic, and supersonic flow regimes, and capture the formation of expansion fans and shock waves in different operating conditions. It demonstrates how pressure ratios influence nozzle performance and flow field structure.

🧩 Simulation Pipeline
Meshing Strategy
Initial default mesh for geometry verification
Refined face size set to 0.09 m for better resolution
Quality metrics (e.g., orthogonality) monitored for mesh integrity
Boundary types assigned: Inlet, Outlet, Symmetry, Wall

Solver Setup
Density-based solver for compressible, high-speed flow
Air modeled as an ideal gas
Steady-state simulation with convergence monitoring
Iteration range: Up to full convergence for each case

Boundary Conditions
Inlet pressures: 1.5 atm, 5 atm, 10 atm, 15 atm, 40 atm
Outlet pressure: 1 atm (ambient)
Static temperature at inlet: 600K
Walls treated with no-slip, adiabatic condition
Symmetry planes used to reduce computational effort

📊 Flow Field Features (By Pressure Case)
1.5 atm: Subsonic-transonic; flow does not reach full supersonic state
5 atm: Choked flow at throat; weak supersonic behavior begins
10 atm: Supersonic flow with early shock wave formation
15 atm: Stronger shocks and complex interactions appear
40 atm: Hypersonic flow; intense shock and expansion structure visible

For each case, the following were visualized:
Mach number contours
Static pressure plots
Velocity vector fields

Shock wave locations and characteristics

🔍 CFD vs. Theory Comparison
Each case's simulation results were compared against theoretical expectations:
Choked flow at the throat (Mach = 1.0)
Subsonic-supersonic transitions in the divergence section
Formation and location of normal or oblique shocks
Pressure and Mach number profiles validated

✅ Results showed excellent agreement with compressible flow theory and gas dynamics principles.


📄 README.md: Full simulation documentation and commentary

💡 Key Takeaways
Accurate modeling of transonic/supersonic flows using Fluent’s density-based solver
Visualization of compressibility effects including shock waves and expansion fans
Pressure ratio as a dominant factor in nozzle flow regime
Demonstrated how CFD aligns with classical gas dynamics theory

🛠 Tools Used
ANSYS Fluent
ANSYS Meshing
CFD-Post / ParaView for visualization
Excel/Python for plotting and comparative analysis
