# A8 – Gear Box Design

Description:
Design a gearbox which can be assembled and disassembled. The spur gears have a gear ratio of 24:9 and are listed in the resource section. The output gear torque and speed are to be 1.25 in-lbf and 1100 rpm relative. The input (pinion,power-transmission) and output (gear, short shaft) shaft diameters are .125 and .25 inches respectively and each have a length of 1 inch. Use the appropriate equations in the Machinery’s Handbook for empirical units. The critical features of the gearbox include the shafts, and the journal bearings.

Assumptions: 

Assume appropriate strength of shafts, use Machinery’s Handbook.
The gear train is ideal.
The moment of the radial force from the gear train is small enough to be ignored.
Note:

The shafts are press fit through the hubs of the gears.
Make sure there is enough clearance between the gears and the gearbox.
Use a running sliding fit for the size of the hole for the shafts.


## Table of Contents

1. [Project Overview](#project-overview)
2. [Engineering Analysis](#engineering-analysis)
3. [Component Selection](#component-selection)
4. [Modeling and Assembly](#modeling-and-assembly)
5. [Tolerances and Drawings](#tolerances-and-drawings)
6. [Results and Lessons Learned](#results-and-lessons-learned)
7. [Files and Resources](#files-and-resources)

## Project Overview

For this project, I designed a compact spur gearbox in SolidWorks with a required reduction ratio of 24:9. The specified output conditions were 1.25 lbf·in of torque at 1100 rpm.

My design uses an 18-tooth input pinion and a 48-tooth output gear mounted on separate shafts. Four bronze sleeve bearings support the shafts inside a two-piece housing. A removable cover and four screw-and-nut pairs allow access to the internal components.

The project combined engineering calculations, component selection, parametric modeling, assembly, and technical drawings.

<img width="566" height="595" alt="image" src="https://github.com/user-attachments/assets/c7725875-d1e3-47de-b266-f64096d54a2f" />
<img width="607" height="678" alt="Screenshot 2026-10-29 004412" src="https://github.com/user-attachments/assets/654a5118-cf61-421b-84ed-79ce0b331fd6" />
<img width="845" height="726" alt="Screenshot 2026-10-29 004349" src="https://github.com/user-attachments/assets/252d38c6-b19a-412c-b7b1-ca164e415d06" />

## Engineering Analysis

I selected the gear tooth counts to match the required reduction ratio:

<img width="880" height="761" alt="image" src="https://github.com/user-attachments/assets/bf1dc109-a5f2-4d92-afb4-4f6e2624daf7" />

Using the specified output speed, I calculated the required input speed:

<img width="912" height="637" alt="image" src="https://github.com/user-attachments/assets/3f403178-9ea0-4e46-be89-798045e8bd0c" />

The gear arrangement reduces speed while increasing ideal output torque.

<img width="857" height="672" alt="image" src="https://github.com/user-attachments/assets/aec6aeca-461c-4b42-8911-3a390309c00a" />

<img width="802" height="810" alt="image" src="https://github.com/user-attachments/assets/bfb63a56-069e-429b-8815-0741a8266533" />

<img width="820" height="656" alt="image" src="https://github.com/user-attachments/assets/1765eb2d-4186-4471-8b87-89ead327c433" />

I modeled a 0.125 in diameter input shaft and a 0.250 in diameter output shaft. Both shafts have a nominal length of 1.000 in. The input shaft experiences the larger torsional shear stress because of its smaller diameter.

## Component Selection

I used McMaster-Carr gears, sleeve bearings, screws, and nuts with custom shafts and housing components modeled in SolidWorks.

### Purchased Components

| Component | Part Number | Quantity | Specifications |
|---|---|---:|---|
| Input pinion | [7880K19](https://www.mcmaster.com/7880K19/) | 1 | Brass spur gear, 18 teeth, 48 diametral pitch, 20° pressure angle, nominal 1/8 in shaft size |
| Output gear | [7880K24](https://www.mcmaster.com/7880K24/) | 1 | Brass spur gear, 48 teeth, 48 diametral pitch, 20° pressure angle, nominal 1/4 in shaft size |
| Small sleeve bearing | [6391K753](https://www.mcmaster.com/6391K753/) | 2 | Oil-embedded 841 bronze, for 1/8 in shaft, nominal 3/16 in housing bore, 1/4 in long |
| Large sleeve bearing | [6391K131](https://www.mcmaster.com/6391K131/) | 2 | Oil-embedded 841 bronze, for 1/4 in shaft, nominal 3/8 in housing bore, 1/4 in long |
| Socket head screw | [91251A078](https://www.mcmaster.com/91251A078/) | 4 | #4-40 thread, 1¼ in long, black-oxide alloy steel |
| Hex nut | [90480A005](https://www.mcmaster.com/90480A005/) | 4 | #4-40 thread, zinc-plated steel, 1/4 in width across flats |


I selected gears with matching pitch and pressure angle so their tooth geometry is compatible. The 18-tooth and 48-tooth combination provides the specified reduction ratio.

The oil-embedded 841 bronze sleeve bearings support the two shaft sizes. Each bearing is 0.250 in long, with one bearing at each end of each shaft.

<img width="750" height="807" alt="image" src="https://github.com/user-attachments/assets/3f0365a9-05dd-4d07-8120-68f664c9d837" />

<img width="775" height="805" alt="image" src="https://github.com/user-attachments/assets/c4203a1a-2c0a-486d-b8b2-ee6ee41693eb" />
I calculated the tangential tooth force using the output torque

<img width="682" height="777" alt="image" src="https://github.com/user-attachments/assets/637ab9eb-c790-4e4f-9656-6ae6dc675569" />
Bearing reactions depend on the position of the gear load relative to the two supports. For a support span S and a load F located a distance a from the rear support. These relationships connect the shaft free-body diagrams to bearing pressure and PV.

<img width="607" height="761" alt="image" src="https://github.com/user-attachments/assets/bbe1e5f4-f17d-4e28-8f20-becf0bc1f87b" />
<img width="603" height="468" alt="Screenshot 2026-10-29 005533" src="https://github.com/user-attachments/assets/cf963555-c29c-43c7-9338-91666b6e7407" />
<img width="612" height="762" alt="image" src="https://github.com/user-attachments/assets/350eb868-3c8d-4597-a57b-ed52f55a2d80" />
<img width="661" height="572" alt="image" src="https://github.com/user-attachments/assets/381dda80-5e10-4467-9be1-9e0117d49e2b" />



<img width="750" height="807" alt="image" src="https://github.com/user-attachments/assets/3f0365a9-05dd-4d07-8120-68f664c9d837" />

