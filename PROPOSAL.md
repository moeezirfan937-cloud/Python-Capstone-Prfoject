# Track A — Research Proposal

**Title:** Reproduction and Off-Design Aerodynamic Performance Assessment of PSO-Based Airfoil Shape Optimization at Varying Reynolds Numbers and Angles of Attack

**Student:** Moeez Irfan  
**Registration No.:** 540014

### 1\. Benchmark Paper

R. Ullah, S. Bibi, Z. Asghar, and A. Shah, “Multi-objective optimization of parametric airfoil shape using NSGA-II and PSO metaheuristic algorithms,” Aerospace Science and Technology, vol. 168, art. 111314, 2026. DOI: https://doi.org/10.1016/j.ast.2025.111314.

Journal ranking: Q1 (Aerospace Engineering, SCImago 2025). The article lists supplementary material, but authors’ code and optimized coordinates are not yet verified. Solver interface: https://github.com/peterdsharpe/AeroSandbox.

### 2\. Result to Reproduce

Reproduce Figure 3 (PSO lift-to-drag convergence, p. 5) at Re = 1 × 10⁶, α = 5° and Mach = 0. The reported PSO L/D is 123 versus 85–90 for NACA 4412; Cm = −0.1006. Compare the resulting geometry with Figure 6 and Table 1 (pp. 5, 7). Use third-order CST, eight shape coefficients, PSO and XFOIL. Section 4.2 reports transition locations of 0.3c (upper) and 0.6c (lower). Document missing settings and inconsistencies in the published drag and iteration counts rather than assuming exact reproduction.

### 3\. Research Question and Extension

How does the aerodynamic efficiency advantage of the PSO-optimized airfoil over NACA 4412 change with Reynolds number and angle of attack away from the original design point?

Evaluate both fixed geometries at Re = 0.5, 1, 2 and 3 million and α = −4° to 12° in 1° increments. Compare Cl, Cd, Cm and L/D using identical solver settings, and report non-converged points. The study addresses the single-operating-condition limitation identified in Section 5 (p. 9); it is an off-design assessment rather than multipoint reoptimization.

### 4\. Data and Computing Resources

Generate NACA 4412 coordinates computationally and obtain the optimized geometry through PSO. Use Python, NumPy, SciPy, AeroSandbox, XFOIL and Matplotlib on a laptop or Google Colab with XFOIL installed. No GPU, experimental data or additional CFD validation is planned.

### 5\. Work Plan and Fallback

By 4 December 2026: implement baseline geometry and XFOIL analysis, run an initial PSO reproduction and compare the design-point L/D with Figure 3.

By 18 December 2026: refine the reproduction, complete off-design sweeps, compare results and prepare the IEEE-format paper. If PSO reproduction fails, use published optimized coordinates if obtainable or perform a clearly labelled partial reproduction with baseline sensitivity analysis.

