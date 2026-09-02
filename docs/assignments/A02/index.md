**MEGR 2156 Assignment 2: Truss Stress**

Assignment Objectives
This assignment is meant to provide experience in applying students' engineering knowledge. This is done through designing a truss to support a load with a safety factor while navigating geometric constraints.

Objectives given include:

Creating a planar truss following geometric constraints

Creating free body diagrams for the truss and all joints

Calculating the minimum cross-sectional area of all members with a safety factor

Calculating the minimum cross-sectional area of pins with a safety factor to withstand single shear

Calculating the weight of the pins with given material properties

Creating an accurate CAD model of the truss and pin connections

Applying mass properties to the CAD model to predict the weight of the truss

Fully documenting the design process, calculations, and reasoning in this document

The following are the constraints given for the assignment:

"Design a lightweight planar truss using A500 structural steel (Some software will not have this material, use another type of steel). There are four steps outlined below. Steps 1 through 2 require FBDs as well as calculations to determine the design. The third step requires a CAD model and verification of the analytical calculations in the previous steps.

Design constraints are shown in Figure #1. (See Appendix for deeper explanation).



The cross-sectional area of each element is to be identical.

The pins are to be identical to each other and each element is to have the same cross-sectional geometry."

<img width="1404" height="604" alt="image" src="https://github.com/user-attachments/assets/d58b6a73-6429-441c-976d-b4aa2862d087" />


**Design**

<img width="4032" height="2100" alt="IMG_5202" src="https://github.com/user-attachments/assets/258b6f36-9914-422e-9da7-6a8e830cdb85" />
<img width="5712" height="1858" alt="IMG_5203" src="https://github.com/user-attachments/assets/2b002992-1ff2-4e5a-b830-a3994c968f02" />
<img width="5712" height="4284" alt="IMG_5210" src="https://github.com/user-attachments/assets/51604b77-c684-47d9-98a5-bba7a6ea2ae0" />

For my truss design, I decided to use a simple planar truss that could withstand two 25kN loads downward at joints C and D. I still used the dimensions of a=0.4m and b=0.3m. I created the geometry of the truss using 7 members and calculated the members lengths horizontally and vertically. I drew my free body diagram, found my reactions, and then used the method of joints to solve for all internal forces.

<img width="4284" height="5712" alt="IMG_5211" src="https://github.com/user-attachments/assets/0536118e-0dbd-49a8-a5ac-aa0f16aea9ad" />
<img width="4284" height="5712" alt="IMG_5212" src="https://github.com/user-attachments/assets/6de0b7e2-c1ec-45fd-9c45-3d943bd0a7ca" />
<img width="5704" height="2936" alt="IMG_5213" src="https://github.com/user-attachments/assets/69fa2bc6-e7b6-477a-878e-3070f38289c4" />


**Cross Sectional Area**

After finding all my internal forces. I used the highest internal force to help me calculate the required cross-sectional area for my truss using the safety factor of 3.5 and the yield strength. I used the stress relationship to compare the working stress with the materials allowable yield stress to find the minimum cross-sectional area. My calculation was 422.7mm^2 and I decided to use a 23mm-by-23mm square selection with the area of 529mm^2. 

<img width="4184" height="2875" alt="IMG_5214" src="https://github.com/user-attachments/assets/cb502f20-473f-49ee-9f66-6210b860c2b8" />
<img width="4074" height="4445" alt="IMG_5215" src="https://github.com/user-attachments/assets/1382710d-aaa0-4e38-b560-3d0ddb14a661" />


**Determine the Cross Sectional Area of connecting pins with a yield strength of 170 ksi and density of 0.278 lb/in^3**

I designed connecting pins to prevent the joints from falling using my largest support reaction and the shear loading condition to account for the others. I used the hardened tool steel shear strength of 170 ksi and a factor of safety of 4. I used the shear stress equation to calculate the minimum pin area and diameter. The minimum calculated diameter was 10.42 so I went up to 11 and calculated a weight of .185 for all pins. 

<img width="4280" height="3106" alt="image" src="https://github.com/user-attachments/assets/48e20c30-061e-4b3b-a766-328c97b6c211" />

<img width="3129" height="4691" alt="IMG_5216" src="https://github.com/user-attachments/assets/46aa35eb-0c10-4a3d-9421-60087360520c" />

**Use Solidworks to design the truss**




