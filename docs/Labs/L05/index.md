# A5 – [Topic]


## Objective 

We were given a list of options of potential snip fit designs we could create in a CAD program. I decided to go with the ball joint example. This was dsigned first and froemnt before continuing on with the poject, so i noticed that my ball-and-socket design does not align with the modeling portion of this project. Especially since the desugn requires supports, i decided to go with a ball and joint, because i imagined making another style would be difficult to built with support.  So instead of having dedicated cantilever dimenions, i figured I'd make them up for the modeling aspect of my website.

## Modeling

I decided that my snap-fit project will be made of PLA the 3d printing material, After [researching](https://www.makeitfrom.com/material-properties/Polylactic-Acid-PLA-Polylactide) the common Young's Modulus and yield strength of PLA (aka  Common Polylactic acid), I got Young's Modulus to be 3.5 GPa (3,500 MPa) and a yield/tensile strength of about 50 MPa. From there, i made sure to use a Safety factor of 3.5. As for the transverse load, we were tasked between a load of .25 lbf - 5 lbf.  The axial load of the clip should be in between 5 lbf - 10 lbf.

For my knowns i have

  + Safety Factor: N = 3.5
    
  + PLA young modulus: E = 3.5 GPa = 3500 MPa
    
  + PLA tensile strength: σy = 50 MPa

  + transverse load between .25 lbf - 5 lbf

  + axial load between 5 lbf - 10 lbf

To start this design, initially we should choose the width and base of the flexure. Since i am a visual learner,i decided to go into solidworks first and foremost to decide the lengths id be dealing with. I wanted something proportional

  +  Base: b = 10 mm

  +  thickness: t = 2 mm
  
We are meant to solve for thr length of the flexure using the beam equation for cantilever beam with a concentrated load at the free end. The equation appropriate for this was found in the lecture slides. Since a cantilever is fixed at one ejd, and the load is concentrated at the very end, i used the second equation in this graph. 

<img width="545" height="293" alt="Screenshot 2026-09-15 211140" src="https://github.com/user-attachments/assets/1e844484-1be6-4052-8d09-bf5e5480d4a3" />

Generate a separate FBD of each component.



That way, i can choose the dimensions of my snap-fit, since it will depend on the flexing using the chosen load. If i did this correctly, then the axial load of the clip should be in between 5 lbf - 10 lbf.

Using my answer from above, I decided to choose the initial width of __ and a base of __ of the flexure. 

I then solved for the length of the flexure using the beam equation for cantilever beam with a concentrated load at the free end.

Here I have provided a separate FBD of each component.

The required axial load is between 5 and 10 lbf. The worst-case value of 10 lbf will be used.



However when reading back the assignment- one of the requirements say "Make sure the stress is less than the strength of material and SF". When adding my stresses, i got 15.56 MPa which is greater than the allowable 14.29 MPa. So if the 5-lbf transverse load and 10-lbf axial load occur at the same critical section, my sizes for the flexure would not meet the 3.5 safety-factor requirement. However indivisially, they pass just fine. *Lesson learned and what i could do to fix that*


## Parametrically design

When creating my CAD file, I used a parametric approach so that the model could be modified during the design process. Instead of manually changing every dimension whenever the size of the part changed, I created relationships between the dimensions which allowed the dimensions to update automatically when one of the primary dimensions was changed.

For example, In the picture below you will see how I initially made the main dimensions equal to one another to achieve the cube shape. I then created linked dimensions between Sketch 1 and Sketch 2, so that when the primary dimension in Sketch 1 is changed, the corresponding dimension in Sketch 2 changes proportionally. This helped keep the two sides of the snap-fit consistent and prevented the geometry from becoming distorted during iterations.

<img width="392" height="288" alt="Screenshot 2026-09-17 141804" src="https://github.com/user-attachments/assets/782961f8-f528-416f-a676-fddce9b83f81" />

> i started off w a cube. I made the parameters so they are al the same length- i assigned it into my eq manager. I also set it so that if ine length gets altered, i did oneside "sketch 1 /2" so that if i change sketch 1, it will scale down equally

<img width="494" height="317" alt="Screenshot 2026-09-17 141827" src="https://github.com/user-attachments/assets/1affd6ca-6bac-4cdf-801e-0c56b93f00f7" />
<img width="409" height="287" alt="Screenshot 2026-09-17 141908" src="https://github.com/user-attachments/assets/246659ec-7bcf-4266-9d3d-affd1055937d" />
<img width="425" height="284" alt="Screenshot 2026-09-17 141959" src="https://github.com/user-attachments/assets/48698a25-d877-4cc0-b0bf-adbe817b3faf" />
> the lengths of my cube were all 6.6, so when making my fillet to round the edges the radius was also set to 6.5 to make a perfect sphere

<img width="332" height="322" alt="Screenshot 2026-09-17 142232" src="https://github.com/user-attachments/assets/e9947e56-eddc-41e4-b65d-d353d8cf68a8" />
<img width="387" height="276" alt="Screenshot 2026-09-17 142349" src="https://github.com/user-attachments/assets/54c424c3-f672-4597-9fc6-6527ea2a3917" />

> here is a demonstration of how i included contraints into my design. If i ever decide to change the width of my rectangle, the midpoint will stay consistent and centered witht he midline.  

<img width="321" height="294" alt="Screenshot 2026-09-17 142526" src="https://github.com/user-attachments/assets/fefa5c58-3c53-4631-b979-4a803cbbb092" />
> just like before, i fillet the sides to be a perfect radius.

<img width="272" height="226" alt="Screenshot 2026-09-17 143405" src="https://github.com/user-attachments/assets/dcad8b9f-564c-4263-b995-8f3679bc5162" />
> i copies the ball section and displaced it 25 mm from the original. this was gonna be used as my base for the body.

<img width="594" height="338" alt="Screenshot 2026-09-17 143743" src="https://github.com/user-attachments/assets/629be9c4-6014-4659-8404-72b8bb2b7b59" />
> i offset the orb by a size of 2 mm.This was previously discussed as the minumum size for 3d printing leeway.

<img width="550" height="272" alt="Screenshot 2026-09-17 145419" src="https://github.com/user-attachments/assets/9ff48e22-6d1d-4f34-87e2-52574f60e095" />
<img width="518" height="281" alt="Screenshot 2026-09-17 145531" src="https://github.com/user-attachments/assets/48015d0d-4891-436d-8119-0da9de8e237d" />
> i am setting up the body

<img width="751" height="283" alt="Screenshot 2026-09-17 145646" src="https://github.com/user-attachments/assets/167d5b3a-d683-464f-9232-221d3b573b38" />
<img width="498" height="263" alt="Screenshot 2026-09-17 145821" src="https://github.com/user-attachments/assets/4570f5ce-66d9-4c5f-9d2d-ddcd457ad38e" />

> once again i amusing the displacement tehcnique, taking that same orb and displacing it 25 mm again, into the holder, to create that opening.

<img width="442" height="246" alt="Screenshot 2026-09-17 150156" src="https://github.com/user-attachments/assets/a882400b-7e93-4878-867a-9eda68c5c9fa" />
> although diffcult tp nptice, i chamfered the sides as reccomended on the assignment. We were given the hint to avoid any sharp inside corners as it will avoid stress concentrations.


<img width="264" height="294" alt="Screenshot 2026-09-17 150705" src="https://github.com/user-attachments/assets/2c7fd443-0f57-45ea-ab74-9f62286fbf28" />
<img width="479" height="277" alt="Screenshot 2026-09-17 150744" src="https://github.com/user-attachments/assets/4ed520db-50d6-41a7-a54b-338d95e060c6" />
<img width="363" height="215" alt="Screenshot 2026-09-17 151027" src="https://github.com/user-attachments/assets/38593ae2-df4c-40ef-b6e7-7ed28f8bdcbc" />

> sinc the ball is supposed to snap in place there is deflection involved. i decided to add slits on the side to account for that. this was done by makig a rectangle, assigning parameters, etruding piece, fillet the sides, and finally extrude cut

<img width="389" height="263" alt="Screenshot 2026-09-17 151830" src="https://github.com/user-attachments/assets/1a63dc17-e04a-4998-b63d-0a73a36e76f5" />

> finally i added a cyllinder to hold the clasper. I was careful to not let it exceed the sup, becayse if it did it would get in the way of the snap in part. I ensured this by making the part see though so i ca tell har far the piece was going. 

<img width="363" height="327" alt="Screenshot 2026-09-17 152032" src="https://github.com/user-attachments/assets/042c0932-84b1-4de8-93d1-cb9d521f2dc5" />
<img width="360" height="272" alt="Screenshot 2026-09-17 152109" src="https://github.com/user-attachments/assets/be8162ca-19ca-431c-98b0-45ebb2030d31" />


<img width="429" height="264" alt="Screenshot 2026-09-17 152259" src="https://github.com/user-attachments/assets/2792b6b4-ead4-41df-8782-89215cab1302" />
<img width="356" height="298" alt="Screenshot 2026-09-17 152356" src="https://github.com/user-attachments/assets/a193cb05-cc4d-42a6-9a5f-6ade071433df" />

> Finally, with the design done it was translated one final time bakc into place and it fit.

## 3D printing

A [source](https://www.hubs.com/knowledge-base/how-does-part-orientation-affect-3d-print/)  that discusses how build orientation affects the strength of an FDM printed part. 

## Test

