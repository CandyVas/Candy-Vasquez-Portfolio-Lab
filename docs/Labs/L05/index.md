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

After [researching](https://www.makeitfrom.com/material-properties/Polylactic-Acid-PLA-Polylactide) the common Young's Modulus and yield strength of PLA (aka  Common Polylactic acid), I got Young's Modulus to be 3.5 GPa (3,500 MPa) and a yield/tensile strength of about 50 MPa. From there, i made sure to use a Safety factor of 3.5. As for the transverse load, we were tasked between a load of .25 lbf - 5 lbf. 

since i am a visual learner,i decided to go into solidworks first and foremost to decide the lengths id be dealing with. I wanted something proportional,  
Initially chose the width and base of the flexure.

+ 80 mm
+ 40 mm
+ 20 mm
+ 
Solve  the length of the flexure using the beam equation for cantilever beam with a concentrated load at the free end.
Generate a separate FBD of each component.

That way, i can choose the dimensions of my snap-fit, since it will depend on the flexing using the chosen load. If i did this correctly, then the axial load of the clip should be in between 5 lbf - 10 lbf.

Using my answer from above, I decided to choose the initial width of __ and a base of __ of the flexure. 

I then solved for the length of the flexure using the beam equation for cantilever beam with a concentrated load at the free end.

Here I have provided a separate FBD of each component.

Make sure the stress is less than the strength of material and SF.

>Determine the bending stress of the flexure component using appropriate force. Make sure the stress is less than the strength of material and SF.
>Determine the axial stress of the flexure with an appropriate load.
>Determine the average shear stress of the flexure protrusion.

## Parametrically design


## 3D printing

A [source](https://www.hubs.com/knowledge-base/how-does-part-orientation-affect-3d-print/)  that discusses how build orientation affects the strength of an FDM printed part. 

Based on what you find, does your chosen orientation for the flexure line up with what the research recommends for a part under bending load? Explain your answer in a short paragraph in your Research section.



## Test

