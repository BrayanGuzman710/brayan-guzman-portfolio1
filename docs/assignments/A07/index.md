# A7 FEA on Bracket

Objectives:
Use Finite Element Analysis (FEA) to improve the bracket design from previous assignments.
Ensure high stiffness, strength, and lightweight optimization through iterative design.
Conduct multiple FEA simulations, refining geometry based on results.
Perform static stress analysis, including constraints, loading, and meshing selection.
Interpret data by identifying max stress, displacement, and safety factors.
Optimize the design by modifying geometry to enhance performance.
Document the entire process with images, calculations, and insights.
Reflect on key engineering lessons learned and time spent.


SolidWorks Links:

### Bracket Designs

- [Download Bracket Design 1](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A07/A5%20Bracket%20Design.SLDPRT)
- [Download Bracket Design 2](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A07/A5%20Bracket%20Design%202.SLDPRT)
- [Download Bracket Design 3](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A07/A5%20Bracket%20Design%203.SLDPRT)

- 
### Link Designs — MEGR 2157

- [Download Link Design 1](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A07/A6%20Link%20Design%20%281%29%20FEA.SLDPRT)
- [Download Link Design 2](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A07/A6%20Link%20Design%20%282%29%20FEA.SLDPRT)
- [Download Link Design 3](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A07/A6%20Link%20Design%20%283%29%20FEA.SLDPRT)


## Table of Contents

- [FEA Setup](#fea-setup)
- [Bracket Results and Design Optimization](#bracket-results-and-design-optimization)
- [Link Results and Design Optimization — MEGR 2157](#link-results-and-design-optimization-megr-2157)
- [Lessons Learned and Time Spent](#lessons-learned-and-time-spent)

- ## FEA Setup

For my FEA setup I used SOLIDWORKS Simulation to perform static stress analyses on my bracket and link. I used the assigned 6061-T6 aluminum material for every design. Its yield strength in the material library was 275 MPa.

<img width="942" height="728" alt="Screenshot 2026-10-20 224250" src="https://github.com/user-attachments/assets/d7d2ae5c-7919-4da3-a9db-336b63c2f940" />

The workflow for the assignment included two loops I used:

Inner loop validation: I kept the geometry, material, fixtures, and loading unchanged while refining the mesh. I compared the safety factor, maximum von Mises stress, and maximum resultant displacement between successive meshes.
Outer loop design optimization: After completing the mesh comparison, I changed the geometry to improve the design and repeated the analysis.
I calculated the percentage change using the newer, finer-mesh result as the reference:

Percentage change = finer result − previous result ÷ finer result times (100)

I stopped refining when the results changed by less than 7%, or after the third mesh attempt, as the assignment said

# Bracket Results and loading

I fixed the two inside horizontal support ledges of the bracket hooks. I applied a total force of 1,200 lbf to the cylindrical bar surface in the horizontal loading direction. This represented the combined loading of two assumed 600 lbf strap forces. I also retained the same fixtures and force for all three bracket designs so that way I could compare the effect of geometry changes.

<img width="1908" height="832" alt="Screenshot 2026-10-18 223408" src="https://github.com/user-attachments/assets/041c3423-d061-4ab0-a06f-c1efa16add13" />

# Link constraints and loading

I fixed the cylindrical surface inside the upper hole. I applied a 1,200 lbf downward force to the cylindrical surface inside the lower hole, parallel to the line joining the hole centers. This setup represented a simplified tensile loading case. Fixing the entire upper-hole surface and distributing the load over the lower-hole surface simplified the pin connections. 

<img width="1177" height="777" alt="Screenshot 2026-10-20 231850" src="https://github.com/user-attachments/assets/863a2c3a-fe72-42ca-a6f2-fbe01f572e2b" />

# Mesh settings

For my mesh I used a solid mesh with the blended curvature-based mesher. The mesh used 16 Jacobian checking points, a minimum of eight elements around a circle, and an element growth ratio of 1.4. All of the meshes had zero distorted elements. 

<img width="682" height="446" alt="image" src="https://github.com/user-attachments/assets/8dad6d1e-43f9-49ef-a906-2056ad1b23c0" />

## Bracket Results and Design Optimization

I used three different bracket designs to evaluate them using the same loading and material. 

<img width="682" height="746" alt="image" src="https://github.com/user-attachments/assets/c61a4d3b-73ed-40e5-bb10-6a3e8835fbb7" />

MY first change added material to the arms to increase stiffness. The second change increased the hook depth to match the arms and removed the depth step between these features.

# Inner Loop

<img width="682" height="736" alt="image" src="https://github.com/user-attachments/assets/409a640e-b695-4bde-be19-db335a08bf35" />

<img width="677" height="737" alt="image" src="https://github.com/user-attachments/assets/c26ddae6-2016-4871-a772-f36934d86407" />

<img width="685" height="776" alt="image" src="https://github.com/user-attachments/assets/8fba62c8-f361-4206-af2e-b75dbadf555a" />

<img width="678" height="782" alt="Screenshot 2026-10-21 184852" src="https://github.com/user-attachments/assets/b77f2c7b-a82c-4382-be33-2eee2c0b6c30" />

<img width="677" height="737" alt="image" src="https://github.com/user-attachments/assets/c8c0bad5-da71-4b79-9689-7e6b2227e399" />

<img width="687" height="712" alt="image" src="https://github.com/user-attachments/assets/a62e8ed5-5e03-4cf2-b02c-655aa6929ce3" />

<img width="681" height="717" alt="image" src="https://github.com/user-attachments/assets/4a5ebd80-9ecc-4ee1-8d95-17938faa36be" />

<img width="682" height="757" alt="image" src="https://github.com/user-attachments/assets/4d3eafa8-6723-4620-8f07-09148dd2fbb5" />

<img width="677" height="747" alt="image" src="https://github.com/user-attachments/assets/a9df996c-8dcf-47aa-b2ae-445dd7197e0b" />




# Max Stress and Displacement locations

For all three bracket designs:

- The maximum stress occurred at an inside hook corner near a fixed support.

  <img width="761" height="572" alt="image" src="https://github.com/user-attachments/assets/6045e6f5-c2d7-45ea-a1df-ca00c1ee6ff2" />


- The maximum displacement occurred near the bottom edge of the loaded cylindrical bar.

<img width="657" height="545" alt="image" src="https://github.com/user-attachments/assets/04906619-9582-4d5b-8e35-8a2210d24286" />


- The minimum safety factor occurred in the maximum-stress region near the hook support.

<img width="871" height="546" alt="image" src="https://github.com/user-attachments/assets/6937cb20-2fb0-4370-b1b3-fee7044468d6" />


# Mesh Convergence

<img width="871" height="655" alt="image" src="https://github.com/user-attachments/assets/54f11d83-361b-4390-8ba0-85536587dafc" />

I stopped after the third mesh attempt for each bracket design, because the assignment said to only have 3 runs. Although the displacement changes met the 7% value, the peak stresses continued becoming bigger as the mesh became finer. That's why I did not consider the bracket’s peak stress or safety factor converged. The increasing stresses were concentrated near sharp inside corners beside the fixed supports. This suggests a possible stress singularity associated with the geometry or boundary conditions. 

# Outer Loop Comparison

Using the finest mesh for each design, increasing the arm depth reduced the predicted maximum displacement from 7.551 to 4.056 mm. Increasing the hook depth reduced it further to 3.073 mm. Bracket 3 had approximately 59.3% less predicted displacement than Bracket 1, while its rounded mass increased from 0.52 to 0.55 lb. Bracket 3 was the stiffest version tested. But none of my bracket designs met the safety-factor target of 4 or the displacement goal of 0.005 in. The displayed peak stresses also exceeded the material’s yield strength. I therefore treated these linear static results as evidence that the design and model required further investigation, rather than as an accurate prediction of deformation after yielding. Going in deeper into the work would be reviewing the support representation and investigating the stress hot spots. 

## Link Results and Optimization

# Geometry Changes

I repeated the same analysis and optimization process for the link. I retained the hole sizes, hole spacing, outside profile, material, fixtures, and force while changing the plate thickness.

<img width="872" height="575" alt="image" src="https://github.com/user-attachments/assets/5a3098aa-9809-4b30-977a-961e65c62014" />

# Inner Loop Results

<img width="677" height="812" alt="image" src="https://github.com/user-attachments/assets/d7cb4b61-b394-405a-b7d7-bed6c79c2bb6" />

<img width="680" height="787" alt="image" src="https://github.com/user-attachments/assets/d6d84d30-f9b6-4271-a8d2-5fb30a918bc7" />

<img width="680" height="710" alt="image" src="https://github.com/user-attachments/assets/b13125bd-2ded-44fd-9232-7213e583c1bd" />

<img width="677" height="732" alt="image" src="https://github.com/user-attachments/assets/57f18d72-ec12-4dac-8344-b95b0903e02b" />

<img width="677" height="717" alt="image" src="https://github.com/user-attachments/assets/c710791d-b644-476b-956c-cfa12735636b" />

<img width="682" height="797" alt="image" src="https://github.com/user-attachments/assets/6f2dfd6a-e070-4c75-886d-e379c904d2da" />


# Max Stress and Displacement Locations 

For all three link designs:

The maximum stress occurred along the side of the lower, loaded hole.

<img width="1055" height="737" alt="image" src="https://github.com/user-attachments/assets/1534911e-5140-4526-8bd2-2fb9c4baf527" />

The maximum displacement occurred at the lower end of the link near the bottom rim of the loaded hole.

<img width="921" height="752" alt="image" src="https://github.com/user-attachments/assets/71b0a9df-7c4c-4e0a-95ac-1f8d65cb8cf2" />

The minimum safety factor occurred in the high-stress region beside the lower hole.

<img width="1566" height="686" alt="Screenshot 2026-10-21 225940" src="https://github.com/user-attachments/assets/ae3447f5-e558-4211-9095-f5aa580c417a" />

The corresponding yield-based safety factors also changed by less than 7%. Each link design met the convergence criterion after the second mesh, so I did not complete a third mesh as it was unnecessary under the assignment’s stopping rule. I used the medium-mesh results for the final design comparisons.

# Mesh Convergence

<img width="687" height="547" alt="image" src="https://github.com/user-attachments/assets/51b311fb-ee6c-49bd-85ef-7edc27ac13ac" />

# Outer Loop Comparison

Link 1 had a minimum safety factor of 2.6305, which was below the target of 4. Increasing the thickness to 0.40 in reduced maximum stress from 104.5 to 64.87 MPa and maximum displacement from 0.05109 to 0.03209 mm. Link 2 reached a reported FOS of 4.2, but required more material. For Link 3, I reduced thickness to 0.39 in. Maximum stress increased to 66.85 MPa, and maximum displacement increased to 0.03291 mm. Its minimum FOS remained above the target at 4.11341.

Because the profile and material stayed unchanged, reducing thickness from 0.40 to 0.39 in reduced the modeled volume and mass by 2.5%. Both masses displayed as 0.13 lb because the mass-properties display rounded to two decimal places.

I selected Link 3 as the preferred version among the three tested designs because it used less material than Link 2 while retaining a modeled FOS above 4. Its displacement of 0.03291 mm, approximately 0.00130 in, was below the 0.005 in goal.


## Lessons Learned and Time Spent

I learned that completing a simulation does not automatically establish that its results are independent of mesh size. In the bracket studies, the maximum displacement changed by less than 7% between the last two meshes, while maximum stress continued increasing a lot. I needed to evaluate convergence separately for each result. I also learned that adding material changes both structural response and mass. Increasing the bracket arm and hook depths reduced predicted displacement but increased mass. For the link, increasing thickness allowed the modeled safety factor to exceed 4. I then reduced the thickness slightly to save material while retaining the target safety factor.

I spent around 9 hours to complete this assignment what took me the most was processing and inputting the information. 

# Resources 

SolidWorks- Creating Model and Simulation
Gifthub- Uploading all info into webpage

