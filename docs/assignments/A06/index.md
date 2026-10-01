### A6 Bracket Drawing

Documentation:
The documentation’s intent is to capture your work and learning process from the time you read through the assignment all the way until you turn in your work. Your work may include but not limited to your thoughts, your insights, your mistakes, your drawings, your calculations etc.

Document the process which includes many pictures with an overview of images.
Make sure to post a picture of the parametric table in CAD.
Detail any mistakes throughout the process.
Actual time it took from start to finish.
Have a Lessons Learned section

## Download Files

## Bracket Files

- [View Bracket Drawing PDF](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/blob/main/docs/assignments/A06/A6%20Bracket%20Design%20Drawing.pdf)
- [Download Bracket Drawing PDF](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A06/A6%20Bracket%20Design%20Drawing.pdf)
- [Download Bracket SolidWorks Part](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A06/A5%20Bracket%20Design.SLDPRT)
- [Download Bracket SolidWorks Drawing](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A06/A6%20Bracket%20Design%20Drawing.SLDDRW)

## Link Files

- [View Link Drawing PDF](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/blob/main/docs/assignments/A06/A6%20Link%20Design.pdf)
- [Download Link Drawing PDF](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A06/A6%20Link%20Design.pdf)
- [Download Link SolidWorks Part](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A06/A6%20Link%20Design.SLDPRT)
- [Download Link SolidWorks Drawing](https://github.com/BrayanGuzman710/brayan-guzman-portfolio1/raw/refs/heads/main/docs/assignments/A06/A6%20Link%20Design.SLDDRW)

<img width="797" height="667" alt="Screenshot 2026-09-29 231803" src="https://github.com/user-attachments/assets/674c84f0-b8c1-46e3-b166-f92e3de5dc60" />
<img width="610" height="757" alt="Screenshot 2026-10-01 012739" src="https://github.com/user-attachments/assets/eb93fbed-8a77-48bc-940c-b30f7e8cd9a0" />


- [Parametric Bracket Design](#parametric-bracket-design)
- [Bracket Drawing and Tolerances](#bracket-drawing-and-tolerances)
- [2157 Link Design and Drawing](#2157-link-design-and-drawing)
- [Lessons Learned and Time Spent](#lessons-learned-and-time-spent)
- [Resources and Downloads](#resources-and-downloads)

## Parametric Drawing
For this assignment, I developed a parametric SolidWorks model of my bracket using the dimensions selected during the previous strength and stiffness analysis. I created a multiview engineering drawing and added tolerances to communicate how the bracket should be manufactured and assembled.
I organized the bracket dimensions as named global variables instead of leaving them as separate unnamed dimensions. I connected the sketch dimensions and extrusion depths to these variables.
<img width="937" height="995" alt="Screenshot 2026-10-01 010635" src="https://github.com/user-attachments/assets/efca194f-55ee-4453-a279-0f958c5177d4" />
<img width="4284" height="5712" alt="IMG_5497" src="https://github.com/user-attachments/assets/8d1a051b-9b9a-4c79-8749-9bd9cff2bf06" />
<img width="4284" height="5712" alt="IMG_5506" src="https://github.com/user-attachments/assets/6d598b11-695d-4321-a28c-f7192bd725d5" />


The selected dimensions came from my previous bracket design work. The bar diameter is additionally controlled by a bending-strength equation inside SolidWorks.
I retained my selected diameter of 0.875 in by adding approximately 0.026 in of diameter allowance above the original calculated minimum.
<img width="800" height="126" alt="image" src="https://github.com/user-attachments/assets/472b2ab7-f92f-4e45-a45c-68ea93c8cbce" />
The allowance calculation uses the original reference values, so it stays constant when the current moment changes. The bar sketch dimension references "Bar Diameter". This means the analytical equation controls the actual geometry instead of only appearing as a separate calculation.
I temporarily changed the bar moment from original value to a random one. The bar diameter changed from original diameter to the random after rebuilding. This made sure my equations were working. 

## Bracket Drawing and Tolerances
I arranged the drawing in third-angle projection, with the top view above the front view and the right-side view to the right. I included an isometric view to help explain the overall shape.
<img width="1005" height="762" alt="Screenshot 2026-10-01 014004" src="https://github.com/user-attachments/assets/be5ebc66-e1d0-4be7-ae11-4a4e671bdbe2" />
I made sure to make a tolerance block so it was easily visible.
ALL DIMENSIONS IN INCHES
X.X +,- 0.02
X.XX +,- 0.01
X.XXX +,- 0.005
Inside width between the supports 2.550
Horizontal opening between the lip tips 1.550
Vertical clearance beneath the lips 1.550

## 2157 Link and Drawing
<img width="862" height="641" alt="Screenshot 2026-10-01 015034" src="https://github.com/user-attachments/assets/161edfdb-0fd7-49e1-b1a9-f3456cf78e97" />

I selected a link width of 1.50 in, a hole-center spacing of 2.00 in, and a thickness of 0.25 in. These dimensions define the link body and the locations of its two connections.
<img width="4284" height="5712" alt="IMG_5506 (1)" src="https://github.com/user-attachments/assets/b98f2c5c-e10c-4ad5-8e13-186976d8a88b" />
I linked the bracket using these formulas
"Bracket Bar Diameter" = "Bar Diameter"
"Bracket Hole Diameter" = "Bracket Bar Diameter"+0.001in
With a bracket bar diameter of 0.875 in, the nominal mating hole diameter is 0.876 in. For the second connection, I selected a nominal shaft diameter of 1.000 in and a hole diameter of 0.9995 in to create nominal interference for a pressed connection. A nominal diameter difference does not guarantee the fit by itself. The hole and shaft tolerances must also maintain the intended clearance. 
<img width="927" height="993" alt="Screenshot 2026-10-01 004752" src="https://github.com/user-attachments/assets/01025e1f-c06c-4680-a1cb-3c537bac8e21" />
For the bracket-side connection, my proposed callouts are:
Bracket bar: diameter 0.875 +0.0000/−0.0005 in
Link hole: diameter 0.876 +0.0005/−0.0000 in
I included the link’s Multiview drawing, body dimensions, thickness, hole sizes, and hole-center spacing. My interface note identifies the bracket-side hole: THE BRACKET-SIDE HOLE MATES WITH THE BRACKET BAR. ITS NOMINAL DIAMETER IS LINKED TO THE BRACKET. BAR DIAMETER THROUGH THE SHARED PARAMETER FILE.

## Lessons Learned
I learned that naming a dimension as a global variable is only part of parametric design. A fixed number can be reused throughout a model, but it does not automatically respond to a changed load. One problem I encountered was entering engineering units and mathematical operators into the equation table. I used the keyboard asterisk for multiplication. I also encountered a warning because the equation referenced variable names that did not match the names in my table. I corrected the references to "Min Bar Diameter" and "Diameter Allow".

Applying the tightest tolerance to every dimension would increase manufacturing and inspection effort. It could require additional machining, more precise equipment, and rejection of parts whose variation does not affect their function. I therefore selected tolerances according to each feature’s purpose.

This assignment took me 8 hours. 
