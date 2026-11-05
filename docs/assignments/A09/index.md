 # Assignment 8: Pulley System

 Description:

Design a pulley system to transfer power between two parallel axes separated by a center distance of 4–6 inches. The system must meet the following requirements:

Pulley Diameter: Both pulleys shall have a diameter of 3 inches.

Rotational Speed: Select an operating speed between 1000–2000 rpm.

Belt Tension (Static): Select a belt tension between 4–6 lbf under stationary conditions.

Material: Pulleys may be made from aluminum, ABS, or steel, and may include a groove and shaft diameter of your choosing (within reasonable manufacturing limits).

Safety Factor: The design must satisfy a minimum safety factor of 3

Assume the belt is made from polyurethane rubber, with a yield strength of 3.25 MPa (471 psi) at 20% strain, based on: Wanga, Chena, Wua, Zhangb, Suna, “Strain-induced Structural and Dynamic Changes in Segmented Polyurethane Elastomers.”


## Table of Contents

1. [Introduction](#introduction)
2. [Belt Design](#belt-design)
3. [Shaft Design](#shaft-design)
4. [Journal Bearing Design](#journal-bearing-design)
5. [Frame Design](#frame-design)
6. [Lessons Learned](#lessons-learned)
7. [Resources](#resources)

## Introduction

I designed a two-pulley belt-drive system using engineering calculations to determine the required belt, shaft, journal bearings, and supporting frame.

The system consists of two 3-inch-diameter pulleys separated by a center distance of 5 inches. I selected an operating speed of 1,500 rpm and an initial static belt tension of 5 lbf.

My goal was to develop a pulley system that meets the design requirements while maintaining a minimum safety factor of 3. I used free-body diagrams, symbolic equations, material properties, and stress calculations to evaluate the components.

### Design Parameters

<img width="897" height="702" alt="image" src="https://github.com/user-attachments/assets/1deb8f4d-be16-45b4-97b7-c0fda687a0e7" />
<img width="897" height="560" alt="image" src="https://github.com/user-attachments/assets/84993381-978d-45b6-905e-dfb77132de30" />

## Belt Design

### Engineering Analysis

I began by calculating the tight-side and loose-side forces acting on the belt. Using an assumed coefficient of friction of 1 and a wrap angle of 180 degrees.

<img width="631" height="717" alt="image" src="https://github.com/user-attachments/assets/1b26176c-7c6e-4808-ab9a-50746a83df62" />

<img width="630" height="512" alt="Screenshot 2026-11-04 223830" src="https://github.com/user-attachments/assets/55cbfc1a-7c25-4cbf-9bd1-8a1ab21437e2" />

I used the maximum belt tension to determine the minimum cross-sectional area and belt diameter.

### Belt Selection

The calculated minimum belt diameter was 0.2788 inches. I selected a nominal 5/16-inch polyurethane round belt because its diameter exceeds the calculated minimum.

<img width="630" height="617" alt="image" src="https://github.com/user-attachments/assets/44100496-803f-4b1a-a97f-8e826a98d853" />

The nominal tensile stress was approximately 125 psi, giving a preliminary safety factor of 3.77 based on the assumed polyurethane yield strength.

<img width="631" height="617" alt="image" src="https://github.com/user-attachments/assets/3fc9f4a4-de92-4c23-932e-2b3f01bb4850" />

I also calculated the belt circumference using the pulley diameter and center distance. The nominal pitch length was 19.4248 inches. When accounting approximately for the round belt diameter, the installed centerline length was 20.4065 inches.

<img width="630" height="302" alt="image" src="https://github.com/user-attachments/assets/f34dd1b8-e4b0-47d3-9536-1e4da17a42ed" />

The proposed belt is McMaster-Carr part 9462T58. The final ordering circumference and belt material ratings must be verified against the manufacturer's specifications.

## Shaft Design

### Engineering Analysis

<img width="635" height="687" alt="image" src="https://github.com/user-attachments/assets/9d485fd6-0f91-4ecb-bfd4-4e0872a9dd74" />

For the shaft design, I selected AISI 1060 hardened steel. I used the difference between the belt tensions to calculate the maximum transmitted torque under the assumed limiting no-slip condition.

The calculated torque was 13.7574 lbf-in.

<img width="630" height="667" alt="image" src="https://github.com/user-attachments/assets/2721e8cc-0eb3-4159-ad52-94d6ad0bad99" />


I first determined the minimum shaft diameter using torsional shear stress and a safety factor of 3. The calculated minimum diameter was approximately 0.1594 inches based on an assumed tensile yield strength of 90,000 psi.

<img width="630" height="647" alt="image" src="https://github.com/user-attachments/assets/9cf89ef0-8063-40ff-a8f1-5d230c89edb7" />

I selected a standard 1/4-inch shaft for the preliminary design.

### Combined Stress Analysis

I also evaluated the shaft under combined bending and torsion.

Using a proposed 3-inch bearing span and a centered pulley, I calculated:

- Bearing reaction A: 5 lbf
- Bearing reaction B: 5 lbf
- Maximum bending moment: 7.5 lbf-in
- Maximum bending stress: 4,889 psi
- Torsional shear stress: 4,485 psi
- Equivalent von Mises stress: 9,184 psi
- Preliminary combined static safety factor: 9.80

These results support the 1/4-inch shaft for the assumed loading and material properties.

<img width="450" height="567" alt="image" src="https://github.com/user-attachments/assets/8a874204-8ba5-46e5-9919-4700a40a6806" />

## Journal Bearing Design

### Engineering Analysis

I evaluated oil-impregnated sintered bronze as the journal bearing material because of its self-lubricating properties and compatibility with rotating steel shafts.

Each bearing was assumed to support a radial load of 5 lbf. I used a 1/4-inch shaft diameter and a proposed bearing length of 1/2 inch.

<img width="450" height="560" alt="image" src="https://github.com/user-attachments/assets/335b8218-6deb-4e9b-a38c-c77e27458627" />


I compared the calculated operating values with published ratings for oil-impregnated bronze bearings.

The preliminary material comparison showed that the pressure, velocity, and PV requirements could be satisfied with the bronze bearing.

## Frame Design

### Design Description

For the supporting frame, I selected 6061-T6 aluminum because it is lightweight, strong, and relatively easy to machine.

<img width="452" height="560" alt="image" src="https://github.com/user-attachments/assets/e8eca2d5-d9c9-4eb8-876c-6093d3ea0ae7" />

I developed a preliminary hand sketch showing the pulley arrangement, shaft positions, and supporting frame.

<img width="451" height="446" alt="image" src="https://github.com/user-attachments/assets/f23f41b0-f8ce-40a0-bd71-b7d50befd6b4" />


## Lessons Learned

Throughout this assignment, I learned how the design of a pulley system involves several connected engineering decisions. The belt tension affects the shaft torque, shaft bending loads, bearing reactions, and frame design.

One important lesson was that selecting a belt requires more than checking its diameter. I also had to consider the required belt circumference, friction, material properties, and installation conditions.

For the shaft, I learned why both bending and torsional stresses should be considered. Although the minimum diameter calculated from torsion was relatively small, the combined stress analysis provided a more complete evaluation.

The journal bearing calculations helped me understand the importance of pressure, surface velocity, and PV ratings when selecting a bearing material.

The frame analysis also demonstrated how assumptions about the support conditions and load distribution influence bending stress and safety factor.

If I continued developing this design, I would verify the manufacturer specifications for the belt and bearings, improve the frame load model, and evaluate the effects of fatigue, deflection, and vibration.

Overall, this assignment helped me understand how to use engineering calculations to make design decisions and evaluate a complete mechanical system.

This assignment took me about 5 hours.


## Resources: 

[McMaster-Carr - Proposed Round Belt](https://www.mcmaster.com/9462T58)

[McMaster-Carr - Sleeve Bearings](https://www.mcmaster.com/products/sleeve-bearings/)

Machinery's Handbook - Bearing Material and Design Reference
