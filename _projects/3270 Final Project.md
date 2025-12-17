---
layout: project
title: MAE 3270 Final Project
description: Final Project in MAE 3270
image: /assets/images/assets/images/image 6.jpg
---
# Improved Torque Wrench Design and Analysis  

## Images of CAD Model With Dimensions  

Note: Bit is cut off where it would be interacting with the socket for analysis purposes  

<img src="{{ '/assets/images/CAD Model with Dimensions.jpg' | relative_url }}" 
     alt="CAD Model"
     width="120%">

## Material of Choice and Important Characteristics  


AISI S7 Tool Steel Tempered at 650 degrees C  


| Youngs Modulus  | Yield strength | Fracture Toughness | Fracture Strength (10^6 Cycles) |
| ----------- | ----------- | ----------- | ----------- |
| 329*10^6 psi| 154 ksi     | 30 ksi      | 60 ksi      |  

<br>

## FEM Loads and Boundary Conditions  

Setup to analyze a 600 in-lb torque on torque wrench with 0.4" of 0.5" bit inside of the socket at the end  

<img src="{{ '/assets/images/Section3.jpg' | relative_url }}" 
     alt="CAD Model"
     width="120%"> 

## FEM Normal Strain Contours  

Strain in the direction of the strain gauge. Strain gauge location probed  

<img src="{{ '/assets/images/Image4.jpg' | relative_url }}" 
     alt="CAD Model"
     width="120%"> 

## FEM Maximum Principal Stress  

Maximum principal stress. Analyzed location on the body probed  

<img src="{{ '/assets/images/Image5.jpg' | relative_url }}" 
     alt="CAD Model"
     width="120%"> 
   

## FEM Results Summary  

|Maximum Normal Stress (on wrench body)   | Maximum normal stress (On bit, due to stress concentration at boundary condition)        | Load Point Deflection   | Strain at strain gauge location      |
| ----------- | ----------- | ----------- | ----------- | 
| 33043 psi | 1.9E5 psi |0.387 in | 1214 microStrain |  

<br>

#### Load Point Deflection:  

<img src="{{ '/assets/images/Image 6.jpg' | relative_url }}" 
     alt="CAD Model"
     width="120%"> 

## Torque Wrench Sensitivity  

Using the strains from the FEM analysis at the strain gauge locations gives a sensitivity of 1.21mV/V, which surpasses the design requirement of 1mV/V by 21%  

## Strain Gauge Selection  


Using a half bridge strain gauge with dimensions of 0.126 x 0.122in, which is a common form factor for general purpose strain gauges at the sensitivity needed. These dimensions fit easily onto the torque wrench so they are able to be used for this application.  
