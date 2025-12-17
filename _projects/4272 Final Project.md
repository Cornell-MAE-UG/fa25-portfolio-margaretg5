---
layout: project
title: MAE 4272 Final Project
description: Final Project in MAE 4272
image: /assets/images/blades.png
---
## Wind Turbine Blade Design Project

This project involved the design of a small-scale wind turbine blade intended to outperform a baseline turbine analyzed earlier in the course while meeting strict geometric, structural, and operational constraints. The blade length was limited to less than 6 inches, with a maximum allowable operating speed of 2000 RPM and testing restricted to wind speeds below 10 m/s. The design was optimized for a target operating condition of approximately 800 RPM at a wind speed of 5.95 m/s and evaluated under a realistic wind environment modeled by a Weibull distribution.The primary objective was to increase aerodynamic efficiency and power output relative to the Lab 4 turbine, which previously produced a maximum power of approximately 0.09 W at 6.5 m/s.

### Project Overview

The design process used blade element momentum (BEM) theory to determine an optimal blade geometry. A three-bladed rotor using a NACA 4412 airfoil was selected due to its favorable low-Reynolds-number lift-to-drag characteristics. The final blade radius was 5.9 inches, and the span was discretized to calculate chord length and pitch angle distributions that would maintain near-optimal angles of attack along the blade. MATLAB scripts were used to vary tip-speed ratio and identify a geometry that maximized the power coefficient while remaining structurally sound. Structural analyses confirmed that the blade could withstand bending moments and torque loads at wind speeds up to 8.3 m/s and rotational speeds approaching 1900 RPM without failure. The resulting geometry was modeled in CAD and manufactured via 3D printing.

### Design Process

The design process was driven by blade element momentum (BEM) theory and focused on maintaining near-optimal aerodynamic conditions along the blade span. Key decisions included selecting the NACA 4412 airfoil for its reliable low-Reynolds-number performance and implementing controlled taper and twist to reduce stall near the root and improve lift-to-drag behavior. The blade span was discretized, and MATLAB scripts were used to compute chord length and pitch angle at each radial station for a target operating point of approximately 800 RPM. 

<img src="{{ '/assets/images/matlab.png' | relative_url }}" 
     alt="Matlab"
     width="75%">

Structural checks were then performed to verify that bending moments, torque, and stresses remained within acceptable limits. The finalized geometry was transferred to CAD software and manufactured using 3D printing, acknowledging potential performance impacts from surface roughness.

### Testing Summary

<img src="{{ '/assets/images/blades.png' | relative_url }}" 
     alt="Blades"
     width="100%">

Experimental testing was conducted in the “Big Blue” wind tunnel using a pitot-static tube to measure flow velocity, a tachometer to measure rotational speed, and a torque brake to apply and measure shaft torque. Power was calculated and recorded across wind speeds ranging from approximately 5.9 m/s to 8.3 m/s. The turbine achieved a peak measured power of 0.8335 W at a wind speed of 8.31 m/s and a rotational speed of approximately 1270 RPM, corresponding to a maximum power coefficient of about 5.24%. When weighted across the Weibull distribution, the expected power output at the design speed of 800 RPM was 0.0573 W, with a maximum expected output of 0.0628 W occurring near 908 RPM. Although the experimental results were significantly lower than the predicted 2.18 W from the theoretical model, the final design improved power output by more than 200% compared to the Lab 4 turbine, demonstrating a successful and data-supported design improvement.


### Personal Contribution

This assignment was completed by myself and two group members. While we were all involved with every step of the process, I took the lead on creating our CAD model. Fusion 360 was my CAD software of choice due to its cloud-based file sharing and accessible student license. All dimensions were directly informed by the output of the MATLAB script. The first step was to import a sketch of the NACA 4412 cross section from Airfoil Tools and scale it to the appropriate size of the root-end of our blade. We continued to add cross sections scaled and rotated according to their position on the length of the blade. The leading edges of the cross sections were connected together by a 3D line sketch. The same was done for the trailing edges. Using the loft feature with the 3D sketches as rails, we made the body of our blade solid. At the root-end, the properly sized hub connection piece was added along with a fillet to attach the connection piece to our blade more securely. The final part of our design process was to export our design as a .stl file for printing.


<img src="{{ '/assets/images/cadcover.png' | relative_url }}" 
     alt="CAD Model"
     width="120%">

