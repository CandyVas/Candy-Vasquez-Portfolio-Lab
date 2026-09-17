# A5 – [Topic]


## Objective 
Parametrically design an assembly of two constituents which snap fit together.
Use parameters in CAD
Use constraints in CAD
Print the two components. On of the components needs to have support material.
Test the snap fit.
Iterate if needed.

The design i decided to go with was a snap on fit, more specifically 
## Modeling
When modeling the components ___ 
I decided that my snap-fit project will be made of PLA the 3d printing material, 

After [researching](https://www.makeitfrom.com/material-properties/Polylactic-Acid-PLA-Polylactide) the common Young's Modulus and yield strength of PLA (aka  Common Polylactic acid), I got Young's Modulus to be 3.5 GPa (3,500 MPa) and a yield/tensile strength of about 50 MPa. From there, i made sure to use a Safety factor of 3.5. As for the transverse load, we were tasked between a load of .25 lbf - 5 lbf.  The axial load of the clip should be in between 5 lbf - 10 lbf.

For my knowns i have

  + Safety Factor: N = 3.5
    
  + PLA young modulus: E = 3.5 GPa = 3500 MPa
    
  + PLA tensile strength: σy = 50 MPa

  + transverse load between .25 lbf - 5 lbf

  + axial load between 5 lbf - 10 lbf

To start this design, initially we should choose the width and base of the flexure. Since i am a visual learner,i decided to go into solidworks first and foremost to decide the lengths id be dealing with. I wanted something proportional

  +  Base: b = .5 in

  +  Width: h = .3 in
  
Solve  the length of the flexure using the beam equation for cantilever beam with a concentrated load at the free end.

since the desugn requirements requires supports, i decided to go with a ball and joint, because i imagined making another style would be difficult to built with support. 

since they are asking for the stress to be lower than the safety factor, i ended up choosing a load of 5 lbf 

The equation appropriate for this was found in the lecture slides. Since a cantilever is fixed at one ejd, and the load is concentrated at the very end, i used the second equation in this graph. 

<img width="545" height="293" alt="Screenshot 2026-09-15 211140" src="https://github.com/user-attachments/assets/1e844484-1be6-4052-8d09-bf5e5480d4a3" />

Generate a separate FBD of each component.



That way, i can choose the dimensions of my snap-fit, since it will depend on the flexing using the chosen load. If i did this correctly, then the axial load of the clip should be in between 5 lbf - 10 lbf.

Using my answer from above, I decided to choose the initial width of __ and a base of __ of the flexure. 

I then solved for the length of the flexure using the beam equation for cantilever beam with a concentrated load at the free end.

Here I have provided a separate FBD of each component.

Make sure the stress is less than the strength of material and SF. Admittedly i dont understand this 

>Determine the bending stress of the flexure component using appropriate force. Make sure the stress is less than the strength of material and SF.
>Determine the axial stress of the flexure with an appropriate load.
>Determine the average shear stress of the flexure protrusion.

## Parametrically design


## 3D printing

A [source](https://www.hubs.com/knowledge-base/how-does-part-orientation-affect-3d-print/)  that discusses how build orientation affects the strength of an FDM printed part. 

Based on what you find, does your chosen orientation for the flexure line up with what the research recommends for a part under bending load? Explain your answer in a short paragraph in your Research section.



## Test

