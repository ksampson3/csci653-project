# csci653-project

This is the Github repository for the CSCI-653 Class Project.

# Problem Description
## Simulating Expected Behavior for the Advanced Microfabricated 

Electrospray thrusters are a form of electric propulsion that operate by exposing an ionic liquid propellant to a uniform electric field. These ionic liquids are conventionally housed in a reservoir and (more importantly) in emitter tips, where the electric field is strongest. This potential difference causes the ionic liquids to be extracted in a "spray" that provides thrust.

Historically, these emitter tips are arranged into arrays with the help of micromachining, allowing for existing USC thrusters to hold up to 25 emitter tips per thruster at a time. Recent research suggests that nanofabrication may allow for emitter tip densities — and therefore thrust — to scale upwards of two orders of magnitude. However, at such high charge densities, we may be creeping very close to the Space Charge Limit. If the Space Charge Limit were reached, then the thruster would be rendered inoperable, unable to produce thrust.

By simulation for a variety of different parameters — packing density, emitter tip geometry, material, etc. — we can more accurately predict thruster behavior _prior to_ creation of the actual device. This would be incredibly useful, and comparisons can be made against the model once the physical thruster is created.

# Anticipated Procedure and Techniques

The following categories are intended to serve as initial predictions for what procedures and techniques will be needed to accomplish this project. USC's Laboratory for Advanced Plasma Dynamics contains legacy code for a multi-scale model for conventional electrospray thrusters. Each of the three scales (nano-, micro-, and centi- to meters) incorporates a different model as outlined in the figure.

![image](https://user-images.githubusercontent.com/92297548/188243711-8a9b1d6e-2422-4277-8999-af26238cc263.png)

## Parallel and Distributed Computing

The existing legacy code includes parallel computing options, which are to be investigated and likely improved upon prior to project completion.

## Data Visualization and Analysis

Previously, data visualization and analysis has been doing through the Paraview software, which has often used .dat or .txt files to create useful images such as these below.

<img width="1439" alt="Plume_5_sep_Conventional_ZoomOut_Array" src="https://user-images.githubusercontent.com/92297548/188244323-e0f4a5a9-0243-492e-bcde-4f1eb80e7732.png">

# Expected Results

We are hopeful that, with outputting data on particle positions are a function of time, we may accurately track the motion of the particles as they exit the thruster. By comparison data on charge density, general energies, and plume characteristics of the AMPS results against more conventional tests, we hope to determine whether such a thruster would operate successfully and remain under the Space Charge Limit.

