# A5 – [Topic]


## Objective 

We were given a list of options for potential snap-fit designs that we could create in a CAD program. I decided to go with the ball-and-joint example. This was designed first and foremost before continuing on with the project, so I noticed that my ball-and-socket design does not perfectly align with the modeling portion of this project. Especially since the design requires supports, I decided to go with a ball and joint because I imagined making another style would be more difficult to build with supports. So instead of having dedicated cantilever dimensions from the beginning, I decided to make up my own dimensions for the modeling aspect of my website and then use the engineering equations to see if my dimensions would work.

## Modeling

I decided that my snap-fit project will be made of PLA the 3d printing material, After [researching](https://www.makeitfrom.com/material-properties/Polylactic-Acid-PLA-Polylactide) the common Young's Modulus and yield strength of PLA (aka  Common Polylactic acid), I got Young's Modulus to be 3.5 GPa (3,500 MPa) and a yield/tensile strength of about 50 MPa. From there, I made sure to use a Safety factor of 3.5. As for the transverse load, we were tasked between a load of .25 lbf - 5 lbf.  The axial load of the clip should be in between 5 lbf - 10 lbf.

For my knowns I have

  + Safety Factor: N = 3.5
    
  + PLA young modulus: E = 3.5 GPa = 3500 MPa
    
  + PLA tensile strength: σy = 50 MPa

  + transverse load between .25 lbf - 5 lbf

  + axial load between 5 lbf - 10 lbf

To start this design, initially we should choose the width and thickness of the flexure.

  +  Base: b = 10 mm

  +  thickness: t = 2 mm
  
We were meant to solve for the length of the flexure using the beam equation for a cantilever beam with a concentrated load at the free end. The appropriate equation was found in the lecture slides. Since a cantilever is fixed at one end and the load is concentrated at the very end, I used the equation for a cantilever beam with a point load at the free end.

<img width="545" height="293" alt="Screenshot 2026-09-15 211140" src="https://github.com/user-attachments/assets/1e844484-1be6-4052-8d09-bf5e5480d4a3" />

I implemented that equation into my calculations below. I then solved for the length of the flexure using the beam equation for a cantilever beam with a concentrated load at the free end.

Here I have provided a separate FBD of each component. These diagrams show the forces and reactions acting on the flexure, base, and ball-and-joint components.

The required axial load is between 5 and 10 lbf. I decided to use the worst-case value of 10 lbf for my calculations. For the transverse load, I used 5 lbf, which is the highest value allowed by the assignment. I wanted to make sure the flexure could withstand the maximum axial force, so designing for the highest load gives me a more conservative design and helps make sure the part will not fail if the full 10 lbf is applied. I used the same reasoning for the transverse load and selected 5 lbf

<img width="351" height="353" alt="image" src="https://github.com/user-attachments/assets/e53d7256-165d-4707-9e19-254529a9435c" />

However, when reading back through the assignment, one of the requirements said, "Make sure the stress is less than the strength of material and SF." When adding my bending and axial stresses together, I got 15.56 MPa, which is greater than the allowable stress of 14.29 MPa.

This means that if the 5-lbf transverse load and 10-lbf axial load occur at the same section at the same time, my flexure dimensions would not meet the 3.5 safety-factor requirement. Individually they pass just fine, but when they are combined, they slightly exceed the allowable stress.


## Parametrically design

When creating my CAD file, I used a parametric approach so that the model could be modified during the design process. Instead of manually changing every dimension whenever the size of the part changed, I created relationships between the dimensions. This allowed the dimensions to update automatically when one of the primary dimensions was changed.

For example, in the picture below, you will see how I initially made the main dimensions equal to one another to achieve the cube shape. I then created linked dimensions between Sketch 1 and Sketch 2 so that when the primary dimension in Sketch 1 is changed, the corresponding dimension in Sketch 2 changes proportionally. This helped keep the two sides of the snap-fit consistent and prevented the geometry from becoming distorted during iterations.


<img width="392" height="288" alt="Screenshot 2026-09-17 141804" src="https://github.com/user-attachments/assets/782961f8-f528-416f-a676-fddce9b83f81" />

> I started off with a cube. I made the parameters all the same length and assigned them into my Equation Manager. I also set it up so that if one length gets altered, the other related dimensions will change as well. I used Sketch 1 and Sketch 2 so that if I changed the main dimension in Sketch 1, the other side would scale down equally.

<img width="494" height="317" alt="Screenshot 2026-09-17 141827" src="https://github.com/user-attachments/assets/1affd6ca-6bac-4cdf-801e-0c56b93f00f7" />
<img width="409" height="287" alt="Screenshot 2026-09-17 141908" src="https://github.com/user-attachments/assets/246659ec-7bcf-4266-9d3d-affd1055937d" />
<img width="425" height="284" alt="Screenshot 2026-09-17 141959" src="https://github.com/user-attachments/assets/48698a25-d877-4cc0-b0bf-adbe817b3faf" />

> The lengths of my cube were all 6.5 mm. When making my fillet to round the edges, I set the radius to approximately 6.5 mm to create a rounded shape that would become the ball.


<img width="332" height="322" alt="Screenshot 2026-09-17 142232" src="https://github.com/user-attachments/assets/e9947e56-eddc-41e4-b65d-d353d8cf68a8" />
<img width="387" height="276" alt="Screenshot 2026-09-17 142349" src="https://github.com/user-attachments/assets/54c424c3-f672-4597-9fc6-6527ea2a3917" />

> Here is a demonstration of how I included constraints in my design. If I ever decide to change the width of my rectangle, the midpoint will stay consistent and centered with the midline. This was important because I wanted the geometry to stay centered even if I changed the dimensions later.

<img width="321" height="294" alt="Screenshot 2026-09-17 142526" src="https://github.com/user-attachments/assets/fefa5c58-3c53-4631-b979-4a803cbbb092" />

> Just like before, I filleted the sides to create a consistent radius and make the shape more spherical.

<img width="272" height="226" alt="Screenshot 2026-09-17 143405" src="https://github.com/user-attachments/assets/dcad8b9f-564c-4263-b995-8f3679bc5162" />

> I then copied the ball section and displaced it 25 mm from the original. This was going to be used as the base for the body.

<img width="594" height="338" alt="Screenshot 2026-09-17 143743" src="https://github.com/user-attachments/assets/629be9c4-6014-4659-8404-72b8bb2b7b59" />

> I offset the orb by a size of 2 mm. This was based on the minimum amount of clearance I had previously discussed for 3D printing. The purpose of this offset was to give the ball enough room to move inside the joint instead of creating an interference fit.

<img width="550" height="272" alt="Screenshot 2026-09-17 145419" src="https://github.com/user-attachments/assets/9ff48e22-6d1d-4f34-87e2-52574f60e095" />
<img width="518" height="281" alt="Screenshot 2026-09-17 145531" src="https://github.com/user-attachments/assets/48015d0d-4891-436d-8119-0da9de8e237d" />

> I then started setting up the body of the joint.

<img width="751" height="283" alt="Screenshot 2026-09-17 145646" src="https://github.com/user-attachments/assets/167d5b3a-d683-464f-9232-221d3b573b38" />
<img width="498" height="263" alt="Screenshot 2026-09-17 145821" src="https://github.com/user-attachments/assets/4570f5ce-66d9-4c5f-9d2d-ddcd457ad38e" />

> Once again, I used the displacement technique, taking that same orb and displacing it 25 mm again into the holder to create the opening where the ball would eventually sit.

<img width="442" height="246" alt="Screenshot 2026-09-17 150156" src="https://github.com/user-attachments/assets/a882400b-7e93-4878-867a-9eda68c5c9fa" />

>Although it is difficult to notice, I chamfered the sides as recommended in the assignment. We were given the hint to avoid sharp inside corners because doing so can help avoid stress concentrations. The chamfer also helps make the transition into the opening smoother.


<img width="264" height="294" alt="Screenshot 2026-09-17 150705" src="https://github.com/user-attachments/assets/2c7fd443-0f57-45ea-ab74-9f62286fbf28" />
<img width="479" height="277" alt="Screenshot 2026-09-17 150744" src="https://github.com/user-attachments/assets/4ed520db-50d6-41a7-a54b-338d95e060c6" />
<img width="363" height="215" alt="Screenshot 2026-09-17 151027" src="https://github.com/user-attachments/assets/38593ae2-df4c-40ef-b6e7-7ed28f8bdcbc" />

> Since the ball is supposed to snap into place, there needs to be some deflection involved. I decided to add slits on the sides to allow the joint to flex. I created these by making a rectangle, extruding the piece, filleting the sides, and finally using an extrude cut. These cuts allow the sides of the joint to move slightly outward when the ball is inserted.

<img width="389" height="263" alt="Screenshot 2026-09-17 151830" src="https://github.com/user-attachments/assets/1a63dc17-e04a-4998-b63d-0a73a36e76f5" />

> Finally, I added a cylinder to hold the clasper. I was careful not to let it exceed the support area because if it did, it could get in the way of the snap-in part. I ensured this by making the part see-through so I could tell how far the piece was going and make sure it would not interfere with the other components. 

<img width="363" height="327" alt="Screenshot 2026-09-17 152032" src="https://github.com/user-attachments/assets/042c0932-84b1-4de8-93d1-cb9d521f2dc5" />
<img width="360" height="272" alt="Screenshot 2026-09-17 152109" src="https://github.com/user-attachments/assets/be8162ca-19ca-431c-98b0-45ebb2030d31" />


<img width="429" height="264" alt="Screenshot 2026-09-17 152259" src="https://github.com/user-attachments/assets/2792b6b4-ead4-41df-8782-89215cab1302" />
<img width="356" height="298" alt="Screenshot 2026-09-17 152356" src="https://github.com/user-attachments/assets/a193cb05-cc4d-42a6-9a5f-6ade071433df" />

> Finally, with the design completed, it was translated one final time back into place, and it fit together correctly in the CAD model.

## 3D printing & Testing
Now that the CAD model had been designed, it was time to print. Immediately after importing it into PrusaSlicer, this is what I was met with. Luckily, with the dimensions I chose, the design was a reasonable size, so there was no need for scaling. Another bonus was that it was already laying on its side, so there was no need to change the orientation.

<img width="204" height="146" alt="image" src="https://github.com/user-attachments/assets/db8f699e-8082-44f5-834e-3b543b6e2520" />

Therefore, I went straight to the print settings. Wall thickness contributes significantly to the structural strength of a snap-fit, especially around the socket and other load-bearing areas. Because of this, I used stronger outer perimeters along with 40% gyroid infill. Combining stronger outer walls with 40% infill increased the strength of the part without making the entire interior solid, which was a good balance for this project.

The last step was adding supports. I used the automatic support feature provided by PrusaSlicer.


<img width="680" height="174" alt="Screenshot 2026-09-17 153551" src="https://github.com/user-attachments/assets/2f3ede97-e660-4b91-84ac-eccfe71b0b4d" />
<img width="662" height="268" alt="Screenshot 2026-09-17 153546" src="https://github.com/user-attachments/assets/aa319a98-66e0-4ac5-87f2-7d4900e9fc59" />
<img width="559" height="287" alt="Screenshot 2026-09-17 171349" src="https://github.com/user-attachments/assets/68e1f88b-8d62-42f8-8a3e-af9ba2184362" />

After I was happy with the settings, I sliced my design and looked through the estimated printing time. You can also notice the orientation of the printed lines in the preview. The orientation of these lines was especially important because the direction of the layers affects the strength of an FDM printed part.

<img width="401" height="232" alt="image" src="https://github.com/user-attachments/assets/b72b35ce-b87b-4092-952d-9ad7906e26d5" />
<img width="243" height="167" alt="Screenshot 2026-09-17 171758" src="https://github.com/user-attachments/assets/fd538bcd-21be-414f-8a4c-60fe70f6047e" />

I used this [source](https://www.hubs.com/knowledge-base/how-does-part-orientation-affect-3d-print/) to determine my build orientation and how it would affect the strength of my snap-fit. The strength of 3D print depends on the direction in which they are printed, and the article explains that FDM parts are much stronger within the XY plane than in the Z direction because the bond between printed layers is weaker than the material within the layers. 

This helped me decide on my orientation because I designed the snap-fit as a ball-and-joint and printed it sideways rather than standing it vertically. The primary reason for my build orientation was strength. If the ball-and-joint had been printed in the direction of the pulling force, the layers could have been more vulnerable to separating when the two pieces were pulled apart. By printing it sideways, I oriented the stronger in-plane material paths to better resist the applied load. My chosen orientation lines up with the research for a part under bending or pulling loads. 


I also chose to lay the ball-and-joint sideways on the build plate because the ball is round (duh), so placing it sideways allowed the geometry to be supported by the build plate instead of trying to balance it with a large unsupported portion. Laying it sideways also helped reduce the amount of support material needed because support material increases printing time, material usage, and post-processing.


<img width="307" height="244" alt="image" src="https://github.com/user-attachments/assets/02382b4f-8728-4e36-bd10-72315fd3a209" />

I chose to use supports only where it was necessary to balance the sphere for printing. Because the ball has curved surfaces, some areas can be difficult for an FDM printer to build without support.

I kept it plain and simple and used the automatic support feature provided by PrusaSlicer. My goal was to let the slicer identify the areas that needed support rather than manually placing supports everywhere.

<img width="191" height="139" alt="image" src="https://github.com/user-attachments/assets/1e0d8e1a-2eba-4f07-93b3-4a19f3e15716" />
<img width="161" height="154" alt="image" src="https://github.com/user-attachments/assets/6660fa3e-b2d7-42d7-b5af-c6c5b8cf25d6" />

Removing the supports proved to be difficult, and I had to get pliers involved. Especially around the opening-side parts, I would not have been able to remove the supports without tools.

This was foreshadowing what was to come with my design because I was afraid the part would not separate. It wouldn't even move inside each other. After further observing my part, I also noticed that the back was poorly printed, so I am not sure whether that was caused by a printer error, the orientation, or human error during the setup.


<img width="320" height="316" alt="image" src="https://github.com/user-attachments/assets/20051d4b-3e84-4f9a-bc56-db3f094ffad2" />
<img width="326" height="300" alt="image" src="https://github.com/user-attachments/assets/b5a13f7e-3d98-4033-975c-fd2ac41c8ecd" />


### Mistakes 
One of the main mistakes was assuming that PrusaSlicer was going to add the supports for me automatically. My first attempt at printing was a major fail because I did not add supports, and it ended up as a tangled mess of melted plastic. After that disappointing first try, I had to reconsider how the curved ball would be supported during printing. A sphere does not have a large flat surface, so its orientation affects both stability and the amount of support required. This showed me that I need to check the support settings before starting the print instead of assuming the slicer will automatically do everything correctly.

<img width="466" height="349" alt="image" src="https://github.com/user-attachments/assets/805b61ef-b79d-479b-bcb7-b38285563b64" />

Another mistake I encountered was that the ball and joint were printed inside each other without enough clearance between the two. Because there was not enough separation between the mating surfaces, the PLA from the two parts fused together during printing. As a result, the ball could not move freely inside the joint, which prevented the snap-fit from functioning properly. This was a major lesson for me because the CAD model looked like the two pieces fit together correctly, but the actual printer could not reproduce the clearance the way I expected. In the future, I would increase the clearance between the mating surfaces and also consider printing the ball and joint separately. Printing them separately would prevent them from accidentally fusing together and would allow me to test the fit before combining them into one print.

On a better note, one thing I learned was that the direction of FDM parts and layers matters when designing a load-bearing part. The orientation should be selected based on the expected load. For my ball-and-joint snap-fit, printing the part sideways meant that the pulling force would not simply try to separate the layers from one another.

I also learned that the CAD model and the physical print are not always going to behave exactly the same way. In CAD, the ball and joint looked like they fit together, but when they were actually printed, the parts fused because the clearance was not large enough. 

Another lesson I learned was the importance of checking the slicer preview before printing. My first print failed because I did not properly set up the supports. Looking at the sliced preview more carefully would have helped me catch the problem before wasting material and time. 

The project took me about 6 hours from start to finish.

## Recources 

[PrusaSlicer](https://www.prusa3d.com/p/prusaslicer/) – Used to slice the CAD model

[ProtoLabs Network](https://www.hubs.com/knowledge-base/how-does-part-orientation-affect-3d-print/) - Helped me determine the build orientation of my part

UNC Charlotte Rapid Prototyping Lab – FDM printer and PLA used to manufacture the part.

[MakeItFrom](https://www.makeitfrom.com/material-properties/Polylactic-Acid-PLA-Polylactide) - PLA young modulus and tensile strength. 
