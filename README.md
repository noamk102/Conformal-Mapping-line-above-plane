# Conformal Mapping: Transmission Line Above a Ground Plane

A MATLAB-based visual representation of electrostatic fields and equipotential lines for a cylindrical conductor (transmission line) situated above an infinite conductive ground plane. 

![Simulation Demo](conduct above pane.gif)

## Overview
This project was built to translate abstract electromagnetic theory into a concrete, visual simulation. In RF and microwave engineering, understanding the field distribution around transmission lines is critical for calculating capacitance, characteristic impedance, and identifying potential breakdown regions. 

This repository contains the MATLAB scripts used to calculate and animate the conformal mapping process, bridging the gap between mathematical theory and practical visualization.

## The Physics & Math
Solving Poisson's or Laplace's equation for cylindrical boundaries over flat planes is analytically challenging in the standard Cartesian coordinate system. 

This simulation demonstrates the power of **Conformal Mapping** (using complex variables where $z = x + iy$). By applying a specific mathematical transformation (such as a bilinear transformation), we map the complex geometry of a cylinder over a plane into a much simpler geometry—like two concentric cylinders (coaxial cable) or parallel plates. 

1. **Mapping:** The complex physical space is transformed into a simplified mathematical domain.
2. **Solving:** Laplace's equation is easily solved in this uniform domain to find the electric field and voltage potentials.
3. **Inverse Mapping:** The solution is mapped back to the original physical space to visualize the true field lines (shown in the animation).

## Technologies Used
* **MATLAB:** Core engine for complex matrix calculations, solving the boundary value problem, and rendering the 2D animations.
* **AI Assistance:** Leveraged LLM (Gemini) as a pair-programming tool to optimize code structure, debug plotting functions, and streamline the animation generation process. 

## How to Run
1. Clone this repository to your local machine.
2. Open the folder in MATLAB.
3. Run the main script: `main_simulation.m`.
4. The script will output the static field plots and generate the animation figure.
