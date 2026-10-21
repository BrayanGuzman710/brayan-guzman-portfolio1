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



I stopped after the third mesh attempt for each bracket design, because the assignment said to only have 3 runs. Although the displacement changes met the 7% value, the peak stresses continued becoming bigger as the mesh became finer. That's why I did not consider the bracket’s peak stress or safety factor converged. The increasing stresses were concentrated near sharp inside corners beside the fixed supports. This suggests a possible stress singularity associated with the geometry or boundary conditions. 

# Outer Loop Comparison

Using the finest mesh for each design, increasing the arm depth reduced the predicted maximum displacement from 7.551 to 4.056 mm. Increasing the hook depth reduced it further to 3.073 mm. Bracket 3 had approximately 59.3% less predicted displacement than Bracket 1, while its rounded mass increased from 0.52 to 0.55 lb. Bracket 3 was the stiffest version tested. But none of my bracket designs met the safety-factor target of 4 or the displacement goal of 0.005 in. The displayed peak stresses also exceeded the material’s yield strength. I therefore treated these linear static results as evidence that the design and model required further investigation, rather than as an accurate prediction of deformation after yielding. Going in deeper into the work would be reviewing the support representation and investigating the stress hot spots. 

## Link Results and Optimization





# Inner Loop Results





