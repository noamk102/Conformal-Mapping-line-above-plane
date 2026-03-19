# Conformal Mapping: Transmission Line Above a Ground Plane

A MATLAB-based visual representation of electrostatic fields and equipotential lines for a cylindrical conductor (transmission line) situated above an infinite conductive ground plane. 



https://github.com/user-attachments/assets/928da6b5-cd56-4118-b4d7-d5358a58fea3



## Overview
This project was built to translate abstract electromagnetic theory into a concrete, visual simulation. In RF and microwave engineering, understanding the field distribution around transmission lines is critical for calculating capacitance, characteristic impedance, and identifying potential breakdown regions. 

This repository contains the MATLAB scripts used to calculate and animate the conformal mapping process, bridging the gap between mathematical theory and practical visualization.

## The Physics
Solving Poisson's or Laplace's equation for cylindrical boundaries over flat planes is analytically challenging in the standard Cartesian coordinate system. 
Our aime will be to transform the geometry of a cylinder above a ground plate (be it endlessly long in the Y direction) into a geometry of two concentric cylinders (coaxial cable).

This simulation demonstrates the power of **Conformal Mapping** for solving such a problem. By applying a specific mathematical transformation (such as a bilinear transformation), we map the complex geometry of a cylinder over a plane into a much simpler geometry—like two concentric cylinders (coaxial cable) or parallel plates. 

## The Math
The geometrey of the cylinder above a plate will be analyzed from the 2D prespective of the X-Y plane (Z being the direction of the energy propergation). We will use the Complex Number field to represent the X-Y plane in terms of complex variables where $z = x + iy$.

The radiuse of the cylinder is a physical given and will be noted as: $a$. So is the distance between the cylinder and the ground plate and it will be noted as: $b$.

<img width="2178" height="1952" alt="initial_state" src="https://github.com/user-attachments/assets/616888b4-0d42-40d4-81eb-7e052952d73b" />


The Conformal Mapping will take all the complex numbers $Z$ and will transform them into $W$:

$W=1/Z$


## Technologies Used
* **MATLAB:** Core engine for complex matrix calculations, solving the boundary value problem, and rendering the 2D animations.
* **AI Assistance:** Leveraged LLM (Gemini) as a pair-programming tool to optimize code structure, debug plotting functions, and streamline the animation generation process. 

## How to Run
1. Clone this repository to your local machine.
2. Open the folder in MATLAB.
3. Run the main script: `main_simulation.m`.
4. The script will output the static field plots and generate the animation figure.
