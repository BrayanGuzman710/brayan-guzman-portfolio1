Motor Mount

Downloads for SolidWorks Parts and Drawings:
### Downloadable Files

- [Download the SolidWorks Part](Motor%20Mount.SLDPRT)
- [Download the SolidWorks Drawing](Motor%20Mount%20Drawing.SLDDRW)
- [View the Engineering Drawing PDF](Motor%20Mount%20Drawing.pdf)


# Motor Mount Design

## Table of Contents

1. [Project Overview](#project-overview)
2. [Engineering Analysis](#engineering-analysis)
3. [Design and CAD Process](#design-and-cad-process)
4. [Final Design and Results](#final-design-and-results)
5. [Mistakes and Lessons Learned](#mistakes-and-lessons-learned)
6. [Files and Resources](#files-and-resources)

---

## Project Overview

The purpose of this project was to design a motor mount for a brushed 24 V DC gear motor. The mount had to attach the motor to rigid wall A and withstand a 300 N force applied to the motor shaft. The design was analyzed using beam-bending stress and deflection equations.

The primary design requirements were:

* Applied force: 300 N
* Factor of safety: 3
* Maximum allowable deflection: 0.30 mm
* Motor shaft diameter: approximately 6 mm
* Motor mounting holes: four M3 holes on a 22 mm bolt circle
* Permitted materials: ABS, PETG, or PLA
* Clearance holes were required for the motor shaft and mounting bolts
* Features were required to reduce deflection
* The model was required to use parametric dimensions

I selected ABS because it was available in the SolidWorks material library and was one of the materials permitted by the assignment. The SolidWorks library listed an elastic modulus of 2000 MPa, tensile strength of 30 MPa, and density of 1020 kg/m³.

<img width="983" height="757" alt="Screenshot 2026-09-16 124448" src="https://github.com/user-attachments/assets/0fd4170b-bdfc-48f9-892f-e5bf0116948e" />


## Engineering Analysis

The mount was divided into two primary structural features. Feature 1 supports the motor, while Feature 2 connects the mount to the rigid wall. Both of my features were approximated as cantilever beams like the assignment states. 

<img width="4284" height="5712" alt="IMG_5356" src="https://github.com/user-attachments/assets/d180ada6-0512-4316-9cc1-d84a9a94aa7b" />


### Feature 1: Motor Attachment

Feature 1 is the horizontal plate that supports the motor. The applied shaft force creates bending stress and deflection in this plate.

<img width="3417" height="2061" alt="IMG_5358" src="https://github.com/user-attachments/assets/afcc9df7-5448-47a8-b741-0077087e00f7" />
<img width="4142" height="2134" alt="IMG_5361 (1)" src="https://github.com/user-attachments/assets/eb400dfd-0e06-4e2d-a1c3-57cd1c870293" />
<img width="3789" height="2365" alt="IMG_5362" src="https://github.com/user-attachments/assets/2e349b4d-74d7-4a90-9df9-82fda11f05cf" />


### Feature 2: Wall Attachment

Feature 2 is the vertical plate that connects the motor mount to rigid wall A. The wall was assumed to support the mount through four bolts.

<img width="4005" height="3917" alt="IMG_5363" src="https://github.com/user-attachments/assets/5918b38b-9eed-4f11-9974-391ab498297f" />

## Design and CAD Process

### Initial Concept

I began by sketching an L-shaped bracket with a horizontal motor plate and a vertical wall plate. The motor is mounted on the horizontal surface, and the vertical plate is fastened to the rigid wall. Two triangular gussets were added to reinforce the corner and reduce bending and deflection.

<img width="1012" height="680" alt="Screenshot 2026-09-16 115730" src="https://github.com/user-attachments/assets/b7c60f78-0e3c-42c0-88a4-714a15213d38" />


### Base and Wall Plates

The horizontal base was modeled as a 50 mm by 50 mm rectangle and extruded to a thickness of 14 mm. The vertical wall plate was designed with a width of 50 mm, a height of 60 mm, and a thickness of 16 mm.


### Motor-Mounting Holes

A 7 mm clearance hole was placed at the center of the horizontal plate for the approximately 6 mm motor shaft.

Four 3.4 mm clearance holes were added for the M3 motor screws. These holes were equally spaced on a 22 mm bolt circle, meaning each hole center was 11 mm from the shaft center.


### Wall-Mounting Holes

Four 5.5 mm clearance holes were added to the vertical plate for the wall bolts. The left and right hole centers were positioned 10 mm from the side edges. The upper and lower hole centers were positioned 12 mm from the top and bottom edges.

<img width="852" height="727" alt="Screenshot 2026-09-16 121106" src="https://github.com/user-attachments/assets/0d39110d-df0c-4ee7-bd1a-37503b86234e" />


### Gussets

Two triangular gussets were added to minimize deflection at the connection between the base and wall plates. Each gusset had 30 mm horizontal and vertical legs and was 6 mm thick.

One gusset was modeled first and then mirrored across the center plane to create the second gusset. These supports increase stiffness by transferring load between the horizontal and vertical plates. I had trouble when trying to create these gussets because I couldn't get the right angle and view to make perfect triangles to match the part. 

<img width="728" height="567" alt="Screenshot 2026-09-16 125231" src="https://github.com/user-attachments/assets/f252d72c-a1ee-4c42-90a5-51cb6fad1ed7" />


### Parametric Modeling

The important dimensions were added directly to the SolidWorks sketches. This allows the plate sizes, thicknesses, hole locations, and gusset dimensions to be changed without rebuilding the entire model.

The main features were renamed in the FeatureManager tree to keep the model organized:

* Motor Base
* Wall Plate
* Motor Holes
* Wall Holes
* Gussets

### Engineering Drawing

I created a A3 engineering drawing with front, top, right-side, and isometric views. The drawing includes the overall dimensions, plate thicknesses, hole diameters, hole locations, gusset dimensions, material, units, and scale.

<img width="1152" height="730" alt="Screenshot 2026-09-17 005442" src="https://github.com/user-attachments/assets/376ec4c4-0e15-440b-8308-8c7d4c7c5b51" />

## Final Design and Results

The final motor mount includes a horizontal motor plate, vertical wall plate, motor clearance holes, four wall-bolt holes, and two triangular reinforcement gussets.

This was my first drawing of my motor mount when thinking about it. 
<img width="2553" height="2933" alt="IMG_5364" src="https://github.com/user-attachments/assets/5d3e3d66-2f69-4ca4-9296-2912c043ef62" />

<img width="728" height="567" alt="Screenshot 2026-09-16 125231" src="https://github.com/user-attachments/assets/6aac8e0f-5114-42ff-ad8c-a07a0ae0df62" />


## Mistakes and Lessons Learned

### Mistakes and Corrections

I had a problem occur when I attempted to extrude the first gusset. SolidWorks produced a zero-thickness geometry error because the gusset only contacted the existing geometry along an edge. I corrected the extrusion direction and adjusted the feature, so the gusset appeared in the correct location. Another problem occurred when I attempted to mirror the gusset as a feature. SolidWorks stated that only merging features could be patterned because the model contained separate solid bodies. I corrected this by mirroring the gusset as a body instead of as a feature. I also attempted to use the Combine command, but SolidWorks could not create one body because it said the bodies did not have enough overlapping volume. 

### Lessons Learned

1. I learned that touching an edge is not always enough for SolidWorks to merge two solid features. The features need proper shared or overlapping geometry.

2. I learned how extrusion direction affects whether a gusset connects correctly to the rest of a bracket.

3. I learned the difference between mirroring a feature and mirroring a solid body.

4. I learned how parametric dimensions make it easier to modify hole patterns and plate dimensions.

### Project Time

The project took approximately 6 hours. I mostly took the most time in SolidWorks fighting errors and sometimes going the wrong way in my project. I went from the beginning of the calculations through completion of the CAD model and engineering drawing.


##  Resources

### Resources

* Motor specifications (https://www.omc-stepperonline.com/brushed-24v-dc-gear-motor-3-6kg-cm-46rpm-w-99-5-1-planetary-gearbox-pa28-28245800-g100)
* SolidWorks- Used to design and model my motor mount. Also used to create an engineering print or design. 
* MEGR 2156 lecture notes — beam-bending stress and deflection equations



