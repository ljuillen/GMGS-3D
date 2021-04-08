# GMGS-3D
A Geometric Multigrid Solver (GMGS) for Large-scale Static Finite Element Simulation on 3D Cartesian Mesh 

# Target
"GMGS-3D" is designed to generate the high-resolution data sets of vector or 2nd-order tensor field for academic use, 
e.g., displacement field, stress field, etc.

# Design description
"GMGS-3D" proceeds the static Finite Element Analysis (FEA) for solid objects discretized into Cartesian mesh, where,
	1) an element index based data structure is used to store the FEA stiffness matrix;
	2) combined with the Jacobian smoother, a Geometric Multigrid based V-cycle is built on the Cartesian mesh
	3) the FEA equation is iteratively solved by Conjugate Gradient Method preconditioned with V-cycle
	
# Limitations
Geometric Multigrid method can go well with some hardware accelerating techniques, yet in this program, the author didn't 
look much into it, given his limited experience in that area, and the specific design target. Any suggestions about improving
performance are highly welcomed.

# Statistics
Experiment Environment: A desktop equipped with Intel Core i7-7700k and 32GB RAM
Example 1: kitten
	Resolutions			DOFs			Time Costs (min)
	


Example 2: parts
	Resolutions			DOFs			Time Costs (min)