# A8 – Gear Box Design

All Downloadables:
#### Assembly

[Gearbox Assembly](<Assem1 Gear Box.SLDASM>)

#### Custom Parts

[Input Shaft](<Input Shaft.SLDPRT>)
[Output Shaft](<Output Shaft.SLDPRT>)
[Housing Base](<Part5.SLDPRT>)
[Housing Cover](<Part8.SLDPRT>)

#### Gears

[18-Tooth Input Pinion](<7880K19_Metal Gear - 20 Degree Pressure Angle.SLDPRT>)
[48-Tooth Output Gear](<7880K24_Metal Gear - 20 Degree Pressure Angle.SLDPRT>)

#### Bearings

[Small Sleeve Bearing](<6391K753_Oil-Embedded 841 Bronze Sleeve Bearing.SLDPRT>)
[Large Sleeve Bearing](<6391K131_Oil-Embedded 841 Bronze Sleeve Bearing.SLDPRT>)

#### Fasteners

[Socket Head Screw](<91251A078_Black-Oxide Alloy Steel Socket Head Screw.SLDPRT>)
[Hex Nut](<90480A005_Zinc-Plated Low-Strength Steel Hex Nuts.SLDPRT>)



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


Gears: Matching pitch and pressure angle provide compatible tooth geometry. The 48-tooth gear and 18-tooth pinion provide the required 2.6667 reduction ratio.
Bearings: Two sleeve bearings support each shaft, with one installed in the base and one in the cover.
Fasteners: Four screws and matching nuts secure the housing while allowing disassembly.
Custom parts: I modeled the shafts and housing around the selected component sizes and the calculated 0.6875 in shaft center distance.

<img width="750" height="807" alt="image" src="https://github.com/user-attachments/assets/3f0365a9-05dd-4d07-8120-68f664c9d837" />

<img width="775" height="805" alt="image" src="https://github.com/user-attachments/assets/c4203a1a-2c0a-486d-b8b2-ee6ee41693eb" />
I calculated the tangential tooth force using the output torque

<img width="682" height="777" alt="image" src="https://github.com/user-attachments/assets/637ab9eb-c790-4e4f-9656-6ae6dc675569" />
Bearing reactions depend on the position of the gear load relative to the two supports. For a support span S and a load F located a distance a from the rear support. These relationships connect the shaft free-body diagrams to bearing pressure and PV.

<img width="607" height="761" alt="image" src="https://github.com/user-attachments/assets/bbe1e5f4-f17d-4e28-8f20-becf0bc1f87b" />
<img width="603" height="468" alt="Screenshot 2026-10-29 005533" src="https://github.com/user-attachments/assets/cf963555-c29c-43c7-9338-91666b6e7407" />
<img width="612" height="762" alt="image" src="https://github.com/user-attachments/assets/350eb868-3c8d-4597-a57b-ed52f55a2d80" />
<img width="661" height="572" alt="image" src="https://github.com/user-attachments/assets/381dda80-5e10-4467-9be1-9e0117d49e2b" />


### Parametric Modeling

I created the shafts using dimensioned circular sketches and extruded features. The shaft diameters and lengths control their geometry and provide the dimensions used in the drawings.

I modeled the housing base around the shaft spacing and purchased components. The base contains a recessed gear cavity, two bearing bores, and four corner supports for the fasteners. The cover matches the base outline and includes corresponding bearing and fastener holes.

### Custom Components

Input shaft 
<img width="1040" height="562" alt="Screenshot 2026-10-29 003417" src="https://github.com/user-attachments/assets/a654d2e3-33ac-475e-84a6-766729983558" />
<img width="995" height="393" alt="Screenshot 2026-10-29 003438" src="https://github.com/user-attachments/assets/3e7dc7f1-eaa4-426c-a46d-e762f53734b2" />
<img width="910" height="616" alt="Screenshot 2026-10-29 003523" src="https://github.com/user-attachments/assets/a10dcf69-fdb9-4586-a4ba-14280d5b15b0" />

Output shaft 
<img width="962" height="622" alt="Screenshot 2026-10-29 003541" src="https://github.com/user-attachments/assets/4a498c24-01f5-443b-9a70-f352faa6ab1a" />
<img width="1152" height="465" alt="Screenshot 2026-10-29 003555" src="https://github.com/user-attachments/assets/ae96da66-5cd6-4fe8-a665-1059b8ee1fce" />

Housing base
<img width="883" height="612" alt="Screenshot 2026-10-29 010227" src="https://github.com/user-attachments/assets/bc087b71-7b53-4b32-b8a9-7834aa1de831" />
<img width="863" height="492" alt="Screenshot 2026-10-29 010248" src="https://github.com/user-attachments/assets/d9fef832-b1cf-404c-8cea-23348e8b6e5d" />
<img width="767" height="487" alt="Screenshot 2026-10-29 010255" src="https://github.com/user-attachments/assets/15d043b8-5e6a-4614-a76f-824099b376ae" />
<img width="646" height="460" alt="Screenshot 2026-10-29 010301" src="https://github.com/user-attachments/assets/b2b15968-448c-4510-ac3d-860a3068913b" />
<img width="641" height="582" alt="Screenshot 2026-10-29 010308" src="https://github.com/user-attachments/assets/881952b4-8146-4ee5-82eb-2ede66fb39b7" />
<img width="626" height="552" alt="Screenshot 2026-10-29 010313" src="https://github.com/user-attachments/assets/98a12944-3c0e-42d6-8e17-788524f270c2" />


Housing cover 

<img width="1042" height="657" alt="Screenshot 2026-10-29 010541" src="https://github.com/user-attachments/assets/c6f59010-3f80-4a53-b32f-81e0f951431a" />
<img width="1187" height="707" alt="Screenshot 2026-10-29 010551" src="https://github.com/user-attachments/assets/ce8becbd-aaf5-49b9-a7fe-e775e0064976" />
<img width="1027" height="666" alt="Screenshot 2026-10-29 010602" src="https://github.com/user-attachments/assets/855bce10-b9a0-41fb-ae52-8c1c8708ac27" />


### Assembly

I imported the purchased component models into SolidWorks and assembled them with the custom parts.

Concentric mates aligned the gears, shafts, bearings, and fasteners. Coincident and distance mates established their axial positions. I used the calculated center distance to position the shaft axes and aligned the gear tooth faces.

After positioning the internal components, I installed the cover and added the four screws and nuts. The assembly model shows the relationship between the internal components and the two housing pieces.


## Tolerances and Drawings

### Fit Intentions

Different interfaces serve different functions in the gearbox. The gears are intended to remain secured to their shafts, the bearing outside diameters are intended to remain secured within the housing, and the shafts are intended to rotate inside the bearings.

The shaft drawings use selected diameter deviations of +0.0002 to +0.0004 in:

| Shaft | Selected Diameter Limits |

| Input shaft | 0.1252–0.1254 in |
| Output shaft | 0.2502–0.2504 in |

### Drawing Tolerances

I used inch dimensions and the following general tolerance block:

| Decimal Format | General Tolerance |

| X.X | ±0.02 in |
| X.XX | ±0.01 in |
| X.XXX | ±0.005 in |

I created six individual part drawings:

1. Input shaft.
2. Output shaft.
3. Housing base.
4. Housing cover.
5. Small sleeve bearing.
6. Large sleeve bearing.

I also created an assembly drawing with orthographic views, an isometric view, and a bill of materials.

The part drawings communicate overall dimensions, hole sizes, feature locations, and selected tolerances. Center marks and centerlines identify hole centers and cylindrical axes. The isometric views help show the shape of each component.

The assembly drawing communicates how the components fit together, and the bill of materials identifies the parts and quantities.

## Results and Lessons Learned

The CAD assembly combines the selected gears, shafts, sleeve bearings, housing pieces, and fasteners. The 48-tooth output gear and 18-tooth input pinion produce the required 2.6667 reduction ratio.

The two-piece housing provides access to the gears through a removable cover. Purchased component models helped me establish the layout and concentrate my custom modeling on the housing and shafts.

One important lesson was the difference between assembly constraints and physical fits. A concentric mate aligns components in SolidWorks, while tolerances describe the dimensional variation allowed in manufactured parts.

I also learned that calculations must follow the actual geometry. Gear pitch diameters determine shaft spacing, and the axial location of the gear force affects bearing reactions.

Preparing the drawings helped me organize the information needed to communicate the design. Overall dimensions describe the part envelope, location dimensions establish feature positions, and individual tolerances communicate critical size limits.

### Time Spent 

I spent approximately 10 hours on component research, calculations, modeling, assembly, and drawings.

I used McMaster-Carr product information and CAD models for the purchased components. 
I used SolidWorks -used to design gear box and assemble

### Resources

- [18-tooth pinion — McMaster-Carr 7880K19](https://www.mcmaster.com/7880K19/)
- [48-tooth gear — McMaster-Carr 7880K24](https://www.mcmaster.com/7880K24/)
- [Small bearing — McMaster-Carr 6391K753](https://www.mcmaster.com/6391K753/)
- [Large bearing — McMaster-Carr 6391K131](https://www.mcmaster.com/6391K131/)
- [Socket head screw — McMaster-Carr 91251A078](https://www.mcmaster.com/91251A078/)
- [Hex nut — McMaster-Carr 90480A005](https://www.mcmaster.com/90480A005/)



