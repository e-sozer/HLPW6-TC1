# High Lift Prediction Workshop 6 - Template Submission Files

This folder contains four files participants are expected to modify and submit for Test Case 1:

1. **FM.dat** = Converged or time-averaged Force and Moment data vs. angle of attack, multiple grid levels may be included
   - N.B.: append grid descriptor if providing results for multiple grids
3. **gridconvergence\_FM.dat** =  Converged or time-averaged Force and Moment data vs. grid level, multiple angles of attack may be included (this is a transpose of #1)
4. **nominalgrid\_cpcf.dat** = Surface pressure and skin friction distributions at locations corresponding to experimental pressure belts. These are defined [here](https://aiaa-hlpw.org/assets/HLPW6/tc1/TC1_Pressure_Rows.xlsx)
   - N.B.: remove nominal grid, add grid descriptor if providing results for multiple grids
6. **nominalgrid\_iterative.dat** = Solver iterative convergence with respect to iteration, or if time-dependent, with respect to convective time
   - N.B.: remove nominal grid, add grid descriptor if providing results for multiple grids

Additionally, participants should revise the Readme.md (this file) within their submission directory to include the following data:

# PARTICIPANT INFO:

# Name(s) and Organization(s):
Eduardo Molina - Embraer
Mauro Lopez - Embraer
Pedro Ciloni - Embraer 
Rodrigo Granzoto - Embraer

## Primary Email:  
eduardo.molina@embraer.com.br
 
# SOLVER INFORMATION:

## Solver Name and Version:
Volcano ScaLES - 2026.03.3

## Basic Algorithm:  
### Spatial discretization: Finite Difference 4th order (inviscid) + 2nd order (viscous)
### Time integration: Explicit (3rd order Runge-Kutta)  
### Initialization method: Freestream / impulsive start for free air and grid-sequencing
### Grid topology: Octree Cartesian grids with immersed boundary 
### Wall modeling: Equilibrium Wall Modeling (Algebraic) 
### SGS closure: Smagorinsky with Dynamic Procedure 
### Aspect ratio range (tangential spacing/wall-normal): 1 
### Wall model exchange location: 1.5 x (Dx) 

## Turbulence Model:  
None
## Transition Method:
None
## Convergence Criteria:
None

# Test Case 1 GRID & SOLUTION INFO (CRM-HLS)

## Grid-Generator Name and Version:  
VolcanoMesh 2026.3.3

## Type (str, overset, unstr, etc):  
Octree

## Number of Total Cells:
417835528

## Miscellaneous:  
Grid generated with one level finer on the flap upper surface compared to the wing and slat. 
