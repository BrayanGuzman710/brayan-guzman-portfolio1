A3: Parametric and FEA

# A3 – Parametric Design and FEA

## Table of Contents

1. [Introduction](#introduction)
2. [Analyze – Hand Calculations](#analyze--hand-calculations)
3. [Decide – Parametric SolidWorks Model](#decide--parametric-solidworks-model)
4. [FEA Setup](#fea-setup)
5. [FEA Stress Results](#fea-stress-results)
6. [FEA Displacement Results](#fea-displacement-results)
7. [Analytical vs. FEA Comparison](#analytical-vs-fea-comparison)
8. [Lessons Learned](#lessons-learned)
9. [Parameter Changes](#parameter-changes)

## Introduction

Description:
You are to design a bar which has a circular cross section where the values of the criteria given for the material, maximum deflection, and load. Determine the bar’s minimum geometry (ie.. length, diameter, and weight) through parametric design while under direct tension. Then verify the geometry through finite element analysis.

<img width="458" height="55" alt="image" src="https://github.com/user-attachments/assets/ac99f514-3ef1-4959-923d-bb37ddc930ed" />


Figure #1. Sketch of  bar with a distributed load.

 <img width="1832" height="850" alt="Screenshot 2026-09-09 174626" src="https://github.com/user-attachments/assets/35d635dd-3f2c-47d1-a2a9-bd3821c2ec3b" />

<img width="958" height="421" alt="Screenshot 2026-09-09 175409" src="https://github.com/user-attachments/assets/c3f6ac81-685f-40c6-bf14-6e5986447519" />

This assignment's purpose was to learn how Parametric CAD modeling and FEA can be used for an engineering design. I chose to design an aluminum bar under an axial tensile load. I first calculated the given dimensions by hand then made my parametric model in SolidWorks. After I used SolidWorks to create a simulation of what would really happen to my bar under the load. I compared the FEA results with my hand calculations. 

## Analysis/ Hand Calculations

<img width="4065" height="3554" alt="IMG_5256" src="https://github.com/user-attachments/assets/1d468f70-4401-4c69-a284-ba49fe61e11f" />

<img width="3021" height="2195" alt="IMG_5249" src="https://github.com/user-attachments/assets/088c08a0-f39d-4d2b-bdf8-6b137dac85fd" />

Based on my hand calculations my bar needs a cross-sectional area of 0.125in^2 and a length of 28.125in to be able to meet the max deflection.

## Parametric SolidWorks Design

<img width="958" height="421" alt="Screenshot 2026-09-09 175409" src="https://github.com/user-attachments/assets/2363ba71-5287-4b2b-8a7c-7e07fac5b35e" />

After doing all my hand calculations on my aluminum bar. I created my bar in SolidWorks and used the global variables for the load, modulus of elasticity, max deflection, width, and bar thickness. I also used equations to calculate the cross-sectional area and the bar length. This was almost like checking my work over again. It made the model parametric, meaning that changing any inputs would automatically change the length. I used the Aluminum 6061 T6 because it was the one with the closest values to mine.

<img width="956" height="386" alt="Screenshot 2026-09-09 180108" src="https://github.com/user-attachments/assets/79c54414-55c5-488d-8396-efe3acde3b66" />

<img width="935" height="422" alt="Screenshot 2026-09-09 175632" src="https://github.com/user-attachments/assets/bc8cba43-a066-496b-94ed-a2bde84ffe3c" />

## FEA Setup

<img width="1292" height="465" alt="Screenshot 2026-09-09 181148" src="https://github.com/user-attachments/assets/5e0c0ece-fb7c-4c9d-bb7b-9370c1a3b7c9" />

For my FEA setup, I created a static study using SolidWorks Simulation. I assigned 6061 T6 Aluminum to my bar. The left end face was fixed, and a 400lbf tensile force was applied to the opposite end face. 
After applying the material, fixture, and load, I used a element mesh. The mesh divided the bar into small elements that SolidWorks uses to calculate stress, strain, and displacement. 

<img width="1511" height="606" alt="Screenshot 2026-09-09 181321" src="https://github.com/user-attachments/assets/db2443d5-c3d0-4d8e-adcc-0bca4cb7b3f8" />

## FEA Stress Results

<img width="1917" height="1016" alt="Screenshot 2026-09-09 181620" src="https://github.com/user-attachments/assets/9f362cd8-d607-4c98-846c-8870614e074f" />

The SolidWorks Simulation showed a maximum Von Mises stress of 25.44 MPa. The yield strength of the 6061 T6 Aluminum was 275 MPa. The max stress was below the materials yield strength.

<img width="3651" height="1075" alt="IMG_5253" src="https://github.com/user-attachments/assets/04639283-835c-4798-a13a-116790effb61" />

Using the max FEA stress my bar is not predicted to yield under the load. 

## FEA Displacement Results

<img width="1917" height="1011" alt="Screenshot 2026-09-09 182528" src="https://github.com/user-attachments/assets/07f25878-7106-4ce7-9582-e4b2b3c4527a" />
<img width="3651" height="1075" alt="IMG_5253" src="https://github.com/user-attachments/assets/04639283-835c-4798-a13a-116790effb61" />

The max displacement predicted by SolidWorks was 0.2195mm or 0.00864 in. This was below the max allowable displacement of 0.009 in. The design satisfies the displacement requirement. 

## Analysis VS FEA

<img width="4020" height="914" alt="IMG_5252" src="https://github.com/user-attachments/assets/a41bcfd8-2b7f-40d0-abb3-b0c4c6e1846b" />

My hand calculation had a displacement of 0.009 in, while the SolidWorks simulation was 0.00864 in. The percent difference was 4%. Both results were really close. I would trust my calculation because the geometry and loading matches the axial deformation. The FEA was useful to check over my work and verifying I was very close. 

## Pin Hole Stress

<img width="3662" height="2278" alt="IMG_5254" src="https://github.com/user-attachments/assets/332a2217-8c79-48aa-b01b-306ff75a2c0b" />

## Lessons Learned 

The biggest thing I learned from this assignment was how parametric modeling can make design changes very easy. Instead of manually calculating and adjusting dimensions, SolidWorks is capable of doing that for you. I also learned that the boundary conditions were important when making the FEA. I had an issue whrn trying to generate it and it said that my model was unstable. I later figured out that it was because I had the wrong fixture in my model. I had to make my entire left face fixed so that the force would be applied correctly on the other end. 

## 2157 Students Assignment

<img width="4249" height="1417" alt="IMG_5251" src="https://github.com/user-attachments/assets/9a5cfecf-285b-4480-9fd8-e577e5b982ed" />
<img width="918" height="395" alt="Screenshot 2026-09-09 200932" src="https://github.com/user-attachments/assets/45f57a42-8de4-4e1a-a6c9-5bcc8560c73b" />
<img width="941" height="447" alt="Screenshot 2026-09-09 201012" src="https://github.com/user-attachments/assets/2d17a8b0-b62e-42be-86af-5c1f9307adb3" />
<img width="936" height="430" alt="Screenshot 2026-09-09 201258" src="https://github.com/user-attachments/assets/d1b8c6b1-fc36-4cdc-93ba-0015ec62e081" />
<img width="932" height="427" alt="Screenshot 2026-09-09 201435" src="https://github.com/user-attachments/assets/3d869b51-a8de-4b80-829c-2aa09872bbfa" />
<img width="936" height="420" alt="Screenshot 2026-09-09 201553" src="https://github.com/user-attachments/assets/b203489c-40a5-4ac1-b7fe-a14869c2feb1" />


To test the parametric model. I changed one parameter at a time and put it back before changing the next. Before making the changes I also predicted whether the length would increase or decrease. 

This assignment took me about 5 hours. 
