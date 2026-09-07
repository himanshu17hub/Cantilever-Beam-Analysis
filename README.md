<h1 align="center">2D Cantilever Beam Analysis using FEM</h1>

<h3 align="center">Finite Element Analysis • Q4 Element • Python • Structural & Modal Analysis</h3>

<p align="center">
  <i>A Python-based Finite Element Method solver developed for static and modal analysis of a 2D cantilever beam.</i>
</p>

<img width="3565" height="1299" alt="09_Mode_1_Shape__f___15_93_Hz_" src="https://github.com/user-attachments/assets/ece879b5-a0be-4b0a-9b85-5aaa8fbe6218" />
<img width="3565" height="1299" alt="13_Mode_2_Shape__f___86_19_Hz_" src="https://github.com/user-attachments/assets/c9e28630-1202-4fb4-9b50-899f8ab9a1cf" />
<img width="3565" height="1313" alt="14_Mode_3_Shape__f___126_50_Hz_" src="https://github.com/user-attachments/assets/64ef6b49-5d5f-4d3a-97e5-7a17c8a4fd1e" />
<img width="3565" height="1313" alt="15_Mode_4_Shape__f___206_28_Hz_" src="https://github.com/user-attachments/assets/77cc0271-7a8e-46f4-bbf3-8e290b5b7597" />
<img width="3565" height="1299" alt="16_Mode_5_Shape__f___344_49_Hz_" src="https://github.com/user-attachments/assets/5a1cb1fd-ff74-41c5-96d2-41b190a08fa2" />


---

<h2> Project Overview</h2>

This project presents the development of a **Python-based Finite Element Method (FEM) solver** for analysing a 2D cantilever beam using **4-node quadrilateral (Q4) finite elements**.

The solver was developed from the fundamentals of FEM rather than relying on a commercial FEA package. The complete workflow covers **mesh generation, element formulation, stiffness matrix construction, global matrix assembly, boundary condition application, loading, solution of the system equations, and post-processing**.

The project was further extended to investigate **mesh convergence, element aspect ratio, analytical validation, and modal behaviour** of the structure.

---

<h2>Objectives</h2>

The main objectives of this project were:

<ul>
<li>Develop a FEM solver for <b>2D structural analysis</b> using Python.</li>
<li>Implement a <b>4-node quadrilateral (Q4) element</b> formulation.</li>
<li>Generate and analyse different computational meshes.</li>
<li>Formulate and assemble the <b>global stiffness matrix</b>.</li>
<li>Apply appropriate boundary conditions and external loading.</li>
<li>Calculate nodal displacements and element stresses/strains.</li>
<li>Perform <b>mesh convergence and aspect-ratio studies</b>.</li>
<li>Validate FEM results against analytical beam solutions.</li>
<li>Extend the solver for <b>modal analysis</b> and determine natural frequencies and mode shapes.</li>
</ul>

---

<h2>FEM Methodology</h2>

The complete analysis follows the fundamental FEM workflow:


Problem Definition
        --->
Geometry Definition
        --->
Mesh Generation
        --->
Q4 Element Formulation
        --->
Element Stiffness Matrix
        --->
Global Matrix Assembly
        --->
Boundary Conditions
        --->
External Loading
        --->
Solve KU = F
        --->
Displacement Calculation
        --->
Stress & Strain Post-Processing
        --->
Validation & Convergence Study

<h2>Problem Definition</h2>

The primary test case considered in this project is a 2D cantilever beam subjected to an external load.

The beam is fixed at one end while the opposite end is subjected to loading.

Boundary Conditions
One end of the beam is completely constrained.

Appropriate degrees of freedom are fixed at the constrained nodes.

External loading is applied at the free end / specified region.

<h2>Element Aspect Ratio Study</h2>

The effect of element aspect ratio on the FEM solution was also investigated.

Different element geometries were analysed to understand how element shape and distortion influence numerical accuracy.

The study provides practical insight into the importance of generating a suitable mesh for reliable FEA results.

<p align="center"> <img src="Images/aspect_ratio.png" width="800"> </p>

<h2>Analytical Validation</h2>

The numerical FEM solution was compared with analytical beam theory to evaluate the accuracy of the developed solver.

The FEM results were compared with analytical solutions based on classical beam formulations, including:

Euler–Bernoulli beam theory
Timoshenko beam theory

The comparison helped assess the accuracy of the numerical model and identify the effect of mesh density and element configuration on the solution.

<p align="center"> <img src="Images/validation.png" width="800"> </p>
2>Modal Analysis</h2>

The FEM framework was further extended to perform modal analysis of the structure.

The objective was to determine the natural frequencies and corresponding mode shapes of the cantilever beam.

The generalized eigenvalue problem was formulated as:

(K - ω²M)φ = 0

where:

K = Global stiffness matrix
M = Global mass matrix
ω = Natural angular frequency
φ = Mode shape

The solver was used to calculate the first five natural frequencies and corresponding mode shapes.

<p align="center"> <img src="Images/modal_analysis.png" width="800"> </p>

<h2>Results</h2>

The developed FEM solver successfully performed:

<ul> <li>2D Q4 finite element discretization.</li> <li>Global stiffness matrix assembly.</li> <li>Application of structural boundary conditions.</li> <li>Static displacement analysis.</li> <li>Stress and strain post-processing.</li> <li>Mesh convergence analysis.</li> <li>Element aspect-ratio investigation.</li> <li>Analytical validation.</li> <li>Modal analysis.</li> <li>Calculation of the first five natural frequencies and mode shapes.</li> </ul>

