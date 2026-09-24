# A5 Bracket Design

SolidWorks Part and Drawing:




Objectives:
Conduct stress analysis to determine appropriate dimensions for structural features.

Generate free body diagrams (FBDs) to visualize forces and constraints for each feature.\

Identify and document known and unknown variables, assumptions, and algebraic models for stress calculations.

Perform stiffness analysis to establish minimum required dimensions based on deflection constraints.

Compare stress and stiffness analyses to ensure structural integrity and compliance with given constraints.

Create detailed multiview sketches illustrating dimensions derived from both stress and stiffness analyses.

Reflect on and document key engineering lessons learned throughout the process.

## Table of Contents

- [Design Inputs and Assumptions](#design-inputs-and-assumptions)
- [Stress and Stiffness Analysis](#stress-and-stiffness-analysis)
- [Sketches and CAD Model](#sketches-and-cad-model)
- [Lessons Learned](#lessons-learned)

## Design Inputs and Calculations 

I designed a bracket to retain the specified rigid T-beam and hold a polyester strap. I used **600 lbf per strap leg**, 6061-T6 aluminum, and a safety factor of 4. I sized features A–E using stress and stiffness calculations, then modeled the selected dimensions in SolidWorks.  

<img width="4284" height="5712" alt="IMG_5497" src="https://github.com/user-attachments/assets/f56f0815-5cfe-4543-892e-2c5a7118cac9" />

The nominal T-beam width is a + 2b = 0.498 + 2(0.9992) = 2.4964 in. I chose a 2.55 in opening between the bracket walls, leaving 0.0536 in of nominal width clearance. The 1.55 in clear wall height exceeds the nominal T-beam dimension c by 0.051 in.

**Analysis assumptions:** The strap load is distributed along the 1.00 in round arm. I modeled the round arm as a cantilever, the center stem as carrying the transferred load, the crossbar as supported by the two sides, and the two walls and lips as separate load paths. I neglected direct-shear failure and shear deflection, as instructed.

<img width="4284" height="5712" alt="IMG_5498" src="https://github.com/user-attachments/assets/2b30420a-0815-4165-bfac-15762958441e" />
<img width="4284" height="5712" alt="IMG_5499" src="https://github.com/user-attachments/assets/825180a9-20c8-4011-a171-57df0a29eb1a" />
<img width="4284" height="5712" alt="IMG_5500" src="https://github.com/user-attachments/assets/919de3cf-3021-47b8-be17-500bb9950807" />
<img width="4284" height="5712" alt="IMG_5501" src="https://github.com/user-attachments/assets/f2fd8a53-fab9-48b1-9064-fca959c68c95" />
<img width="4284" height="5712" alt="IMG_5502" src="https://github.com/user-attachments/assets/45278698-07ba-4134-b31d-9e474cd01dec" />
<img width="4284" height="5712" alt="IMG_5503" src="https://github.com/user-attachments/assets/19c7dd48-3845-4b2a-b248-9754fb583979" />

I analyzed the load path from A,B,C,D, and E. For each feature, my notebook shows the known values, unknown dimension, assumptions, free-body diagram (FBD), algebraic equation, substitution, and the result.

##Sketches and CAD Model
This is my hand-drawn front, top, and side multiview sketch using the minimum dimensions obtained from stress analysis.

<img width="4284" height="5712" alt="IMG_5504" src="https://github.com/user-attachments/assets/9145d819-b909-4b68-9eaf-5cb5316d2939" />

This is my hand-drawn front, top, and side multiview sketch using the minimum dimensions obtained from stiffness analysis.
<img width="4284" height="5712" alt="IMG_5505" src="https://github.com/user-attachments/assets/280773ec-6835-4326-a658-3c0de9301f41" />

This was my SolidWorks print
<img width="1127" height="833" alt="Screenshot 2026-09-23 233011" src="https://github.com/user-attachments/assets/ec97f451-fd82-49bf-8178-287da25901a1" />

<img width="813" height="565" alt="Screenshot 2026-09-22 231356" src="https://github.com/user-attachments/assets/da71fea2-84ae-41bb-b76c-fb3e2ebe106d" />

<img width="787" height="605" alt="Screenshot 2026-09-22 232832" src="https://github.com/user-attachments/assets/07fd9827-276c-463b-a472-26dfad5970ed" />

<img width="857" height="816" alt="Screenshot 2026-09-23 171358" src="https://github.com/user-attachments/assets/b202174f-76d0-419a-a16e-1bca2b270cf8" />

<img width="497" height="433" alt="Screenshot 2026-09-23 231254" src="https://github.com/user-attachments/assets/fd864b07-8bc4-44ec-8208-0c2ac4f4444c" />

<img width="646" height="622" alt="Screenshot 2026-09-23 231329" src="https://github.com/user-attachments/assets/4f8ccd8b-7dfd-462b-9abe-f2401fa5ae85" />


## 2157 Students Only
<img width="450" height="610" alt="Screenshot 2026-09-24 002917" src="https://github.com/user-attachments/assets/8816865c-5d3c-4fb1-afae-15e67811f5c4" />
<img width="410" height="495" alt="Screenshot 2026-09-24 003018" src="https://github.com/user-attachments/assets/b8fabfe8-92d5-4994-803b-c74ceefebcbe" />
<img width="4284" height="5712" alt="IMG_5506" src="https://github.com/user-attachments/assets/9970c966-551c-49dc-9aa7-85de6ffb753e" />
## MEGR 2157: Linkage and Fits

### Link design

I designed a two-hole aluminum 6061-T6 link to connect bracket feature A to a nominal 1.000-inch shaft. I assumed that the link carries both 600 lbf strap loads, giving an axial load of 1,200 lbf. The holes are centered along the link.


I used a safety factor of 4 and a yield strength of 40,000 psi. The allowable nominal stress is 40,000 / 4 = 10,000 ps`, so the required net area at a hole is 1,200 / 10,000 = 0.1200 in.

I selected a plate width of **1.50 in**, thickness of **0.25 in**, and hole-center spacing of **2.00 in**. The larger hole controls the net area. Using its maximum example diameter of 1.0006 in:

The estimated deflection is below the **0.005-inch limit**. For rounded ends with a radius of 0.75 in, the proposed overall link length is approximately **3.50 in**.

**Reference:** *Machinery’s Handbook*, 31st ed., “ANSI/ASME Standard Limits and Fits,” pp. 650–660: [fit descriptions](https://online.flippingbook.com/view/954192180/714/), [running and sliding fit table](https://online.flippingbook.com/view/954192180/718-719/), and [force-fit table](https://online.flippingbook.com/view/954192180/728-729/).



## Lessons learned and Resources

I learned that a dimensioned sketch can still put a feature in the wrong location. My lower stem was 0.90 in wide but was aligned to the center mark by its left edge. I corrected its position before extruding. I also checked the round arm’s extrusion direction in the front view to make sure it extended left from the stem. In the Multiview drawing, I changed the displayed diameter precision so the Ø0.875 in design value was clear. This assignment took me 7 hours to complete.

Resources:
SolidWorks- used to design part and create print of part
GitHub- used to input all data and create a information page
Google Docs- used to input all information
Machinery's Handbook


