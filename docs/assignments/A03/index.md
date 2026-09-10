A3: Parametric and FEA

# A3 – Parametric Design and FEA

## Table of Contents

1. [Introduction](#introduction)
2. [Analyze – Hand Calculations](#analyze--hand-calculations)
3. [Decide – Parametric SolidWorks Model](#decide--parametric-solidworks-model)
4. [Parameter Changes](#parameter-changes)
5. [FEA Setup](#fea-setup)
6. [FEA Stress Results](#fea-stress-results)
7. [FEA Displacement Results](#fea-displacement-results)
8. [Analytical vs. FEA Comparison](#analytical-vs-fea-comparison)
9. [Lessons Learned](#lessons-learned)


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

After doing all my hand calculations on my aluminum bar. I created my bar in SolidWorks and used the global variables for the load, modulus of elasticity, max deflection, width, and bar thickness. I also used equations to calculate the cross-sectional area and the bar length. This was almost like checking my work over again. It made the model parametric, meaning that changing any inputs would automatically change the length. 

<img width="935" height="422" alt="Screenshot 2026-09-09 175632" src="https://github.com/user-attachments/assets/bc8cba43-a066-496b-94ed-a2bde84ffe3c" />





