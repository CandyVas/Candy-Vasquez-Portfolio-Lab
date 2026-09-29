# A6 – [Topic]
 
## Parametrically design

For this project, our goal was to parametrically design a small component that would snap onto the features of an artifact provided in class. I chose a gear motor as my artifact because it looked decently easy to make for a snap-fit design. The gear motor is cube-shaped, with a cylindrical rod protruding out the top. It also has ridges along the 4 corners which could provide the place for a snap fit.

<img width="194" height="204" alt="image" src="https://github.com/user-attachments/assets/02499f40-1988-4368-8300-a29ef0f5682a" />
<img width="210" height="212" alt="image" src="https://github.com/user-attachments/assets/b959d441-9ee1-4d68-8c7a-86c839298fa3" />
<img width="193" height="232" alt="image" src="https://github.com/user-attachments/assets/e9fa1e1a-78a7-42d6-93a4-4bd523932326" />

My initial idea was to design a snap-fit around the cylindrical rod. However, I couldn't figure out how I would accomplish said 'snap'. I then considered designing a complete lid that would fit over the entire motor. This created another problem because of either the cylinder protruding from the top, or the wires coming out bottom.

I decided I'd do a work around with the lid idea and have an opening around the cylindrical rod. This allowed the lid to cover the main body without interfering with the cylinder or wires. Here is the hand sketch of the feature, and my potential idea 

<img width="462" height="316" alt="image" src="https://github.com/user-attachments/assets/cb4ccd62-28f9-4f53-a0e0-ddf8ed4e188f" />

I researched different types of snap-fit joints and found that a cantilever-style snap fit would be appropriate for a small 3D-printed component. I used this [website](https://www.hubs.com/knowledge-base/how-design-snap-fit-joints-3d-printing/). One big idea that I took from it was the use of tapering, because with constant thickness, a snap-fit cantilever can experience higher stress which can cause breakage

### Measuring
Before creating the CAD model, I measured the gear motor. I used a dial caliper to measure the dimensions of the artifact. Since the caliper was displaying measurements in inches, I initially recorded my measurements in inches and then converted them to millimeters.

For the larger dimensions, I also used a regular ruler as a secondary check. This was useful because it allowed me to make sure that my caliper readings and unit conversions were reasonable.

<img width="197" height="204" alt="image" src="https://github.com/user-attachments/assets/7b790439-971d-414b-828b-3653e9e656dd" />
<img width="201" height="228" alt="image" src="https://github.com/user-attachments/assets/de8686bb-2062-4065-82b3-367edf96007e" />
<img width="180" height="211" alt="image" src="https://github.com/user-attachments/assets/0dae88ae-1c4a-45ce-9228-a775995a45c3" />

The primary measurements I recorded were...

+ Main body width: 1.367 in = 34.72 mm

+ Cylindrical rod diameter: 0.865 in = 21.97 mm

+ Distance from the top of the motor to the ridge: 0.363 in = 9.22 mm

I also measured the extruded ridge found on all 4 corners of the cube. Although it was a smaller feature and more difficult to measure because of the size of the caliper.

+ Ridge thickness:  0.078 in = 1.98 mm


For the beginning of my lid design, I used the measured motor body dimension of 34.72 mm. I then added a small amount of clearance so that the printed lid would not be exactly the same size as the measured artifact. I used this [website](https://rapidprototypingsolutions.se/en/knowledge-bank/order-3d-printing-with-the-correct-tolerances-for-fitment/) to determine what clearance would be best suited for a press fit since we are designing parts that must fit together. I decided to do this to the rest of my measurements and ended up with a overall clearance of .2 mm

34.72 mm > 34.92 mm

9.22 mm > 9.42 mm

21.97 mm > 22.17

<img width="458" height="295" alt="Screenshot 2026-09-24 113813" src="https://github.com/user-attachments/assets/99cce09c-e069-4302-87e8-07177adbceb3" />

> Using my measured dimensions + clearance, I made a square with identical dimensions. So my CAD had dimensions of 34.92 mm x 34.92 mm

<img width="590" height="340" alt="image" src="https://github.com/user-attachments/assets/48fea2bc-7dac-46bb-8361-5ec7edd5a410" /> 

> Once the basic square shape was created, I extruded it to create the main body of the lid. I used the height from the top of the motor to the ridge as reference. The measured value was 9.22 mm, so I used half the height for the lid extrusion.

The reason for using a smaller height was that I did not want the lid to extend farther down the motor than necessary. The goal was to eventually create hooks that grab onto the ridges.

<img width="596" height="331" alt="Screenshot 2026-09-24 115307" src="https://github.com/user-attachments/assets/7f4f99a7-b2c7-485d-84d5-ba45a13106fe" />

> The next step was to hollow out the inside of the lid. I used the Shell feature in SolidWorks and selected a thickness of 1 mm. I shelled the part outward so that the external dimensions of my original cube would remain controlled by the parameters I had already established.

<img width="557" height="347" alt="Screenshot 2026-09-24 115924" src="https://github.com/user-attachments/assets/3e5a38c5-dcee-4dd3-8923-575affd8e728" />

> The gear motor did not have perfectly sharp corners. Instead, the corners were rounded. Therefore, I added fillets to the corners of the lid. I selected a 4.5 mm fillet radius.

<img width="685" height="386" alt="image" src="https://github.com/user-attachments/assets/4557610c-f71d-4be8-90d7-bec043060205" />
<img width="362" height="347" alt="Screenshot 2026-09-24 120540" src="https://github.com/user-attachments/assets/971dd771-846d-4ede-8199-775799e7711c" />

> One of the main problems I needed to solve was the rod protruding from the top of the motor. A solid lid would interfere with this feature, so I created a cutout in the center of the lid. The measured diameter of the rod was 21.97 mm. I initially increased this to 22.17 mm to provide clearance around the rod.

Rather than placing the circle manually, I used parameters and sketch relations to make sure the circle was centered relative to the square body. This was important to the parametric design because if I later changed the size of the lid, the circle would remain centered automatically.

<img width="407" height="313" alt="Screenshot 2026-09-24 134036" src="https://github.com/user-attachments/assets/325a4c5f-226a-4ba1-88e2-cf54a4b44901" />

> After creating the main lid, I needed a way for it to stay attached to the motor. This was where the snap-fitcomes in handy. A typical snap-fit works by having a flexible hook to deflect while it is being inserted. Once the hook passes the edge of a feature, it returns toward its original position and locks the two parts together.

I remembered that SolidWorks includes a built in Snap Hook feature, so I decided to experiment with using it rather than manually creating the entire snap mechanism. The Snap Hook feature was useful because it provided a starting point for creating the flexible hook geometry and helped account for the flexure required for the snap. 

However I came across a problem- the snap hook feature would not work against a fillet corner. Because of this, I changed my design strategy. Instead of placing one snap hook on each corner, I decided to put two snap hooks on a singular corner. Although this was not as symmetrical as my original idea, it allowed me to use the existing SolidWorks feature while still creating an attachment mechanism.

 <img width="304" height="290" alt="Screenshot 2026-09-24 134201" src="https://github.com/user-attachments/assets/897adbeb-73d3-4e05-9b1b-17c7c05fccb2" />
<img width="379" height="242" alt="Screenshot 2026-09-24 134610" src="https://github.com/user-attachments/assets/ca5ce9f9-80c7-4472-ad66-d0bc190405df" />
<img width="360" height="326" alt="image" src="https://github.com/user-attachments/assets/ea45fa5c-f7fb-45c9-939a-9e1ab0201e9b" />

> I also used parameters when creating the area that supports the snap hooks. I extended the base supporting the snap hooks by 1 mm on each side. This dimension was intentionally controlled rather than being based on an arbitrary sketch size.

The purpose of this was to maintain consistent spacing if the overall size of the lid changed. For example, if I increased the size of the square body, the snap-hook support would continue to maintain the same 1 mm relationship to the surrounding geometry.

## Documentation

After completing my design in SolidWorks, I exported my model as an STL file and imported it into PrusaSlicer. I then prepared the model for 3D printing by choosing its orientation, adjusting the infill and perimeter settings, checking the estimated dimensions, and generating the G-code needed by the printer.

<img width="212" height="161" alt="image" src="https://github.com/user-attachments/assets/1af914b6-6f82-406a-bfb8-22d6232a8185" />

When I first imported the file, I immediately noticed a problem with the orientation. The model was positioned on its side rather than sitting flat on the print bed.

<img width="745" height="239" alt="Screenshot 2026-09-24 135518" src="https://github.com/user-attachments/assets/6068a5cc-fe06-4061-bda8-014aba24c28f" />

If I printed it in this orientation, a large portion of the model would have been unsupported. This would have needed additional support material and would have made the print more complicated than necessary. To fix this, I used the rotation controls in PrusaSlicer and changed the rotation around the x axis by 90 degrees. This allowed the flat back surface of the lid to sit directly against the print plate. I decided this for the reduced support material, better stability, and a better print efficiency.

In the image above you will see that my final dimensions of the sliced print were

X: 38.92 mm
Y: 38.92 mm
Z: 15.68 mm

The 38.92 mm dimensions make sense when compared to my CAD model. The main lid dimension was 34.92 mm, but I intentionally extended the top structure by 1 mm on each side to provide room for the snap-hook structure.

<img width="620" height="167" alt="Screenshot 2026-09-28 202930" src="https://github.com/user-attachments/assets/38abdc7d-6e79-4775-ba35-1a3a7aba7e95" />


As for the wall thickness of my print, I chose to increase it to 4. Increasing the number of perimeters creates thicker, more continuous outer walls which is useful for my snap-fit because the hooks need to withstand the forces created during bending. A wall that was too thin could make the lid weak or cause it to deform when the snap hooks are engaged. Since the part is relatively small, adding some additional wall thickness also helped make the printed prototype more durable. 

As for the layer height, I kept the default of 0.2 mm, simply because I did not initially consider changing the layer height to be necessary for this particular print. The print did, however, use a total of 78 layers. 

<img width="517" height="164" alt="image" src="https://github.com/user-attachments/assets/a8181643-d891-4229-b668-ad5b056e4a51" />

By now we know the purpose of infill is to provide internal structure without making the entire object completely solid. I chose 15% because the lid does not need to be completely solid to function. A higher infill percentage would increase the strength, but flexibility was more important for this design. As for the pattern, I selected gyroid because it provides good strength in multiple directions while keeping the infill relatively lightweight.

After the slicer settings were finalized, I generated the G-code and transferred it to PC-09 using a USB drive. I used PC-09, which had PLA material. I used PLA because it was the available material for this printer and was what i set my settings in PrusaSlicer.
The part was then placed on the print bed and the printing process began.

<img width="209" height="268" alt="image" src="https://github.com/user-attachments/assets/46c9704f-4c52-4b51-b1ce-26b32264e06b" />

I also recorded a short [video](https://github.com/user-attachments/assets/eee2761e-d7f4-44a7-b0ea-b27dc032e045) during this process as documentation of the transition from the digital CAD model to the physical object.


<img width="174" height="222" alt="image" src="https://github.com/user-attachments/assets/12e71945-07a5-4094-a5a0-df622225fc94" />

> Here is the print fully printed

Unfortunately, the first print did not fit correctly.

When I attempted to place the lid onto the gear motor, I discovered that the internal dimensions were too small. The lid would begin to slide onto the motor but would not fully sit.

<img width="209" height="270" alt="image" src="https://github.com/user-attachments/assets/e53a98f5-b4b3-4341-9142-bc850d00b3e7" />
<img width="220" height="270" alt="image" src="https://github.com/user-attachments/assets/3048f52a-d8fd-471e-80ca-fac825cf8135" />

This was disappointing because the print did not allow me to properly test the rest of the design. I could not determine whether the snap hooks were correctly positioned or whether the center opening had the correct dimensions. So therefore I returned to my SolidWorks model and modified the main internal dimension.


My original design had been based around the measured 34.72 mm motor dimension. I initially increased this to 34.92 mm to provide clearance. However, the physical print showed that this amount of clearance was not sufficient. I therefore changed it to 35.50 mm. This was a large increase compared to my original 0.2 mm clearance. I made this decision because I wanted the next prototype to provide enough room to actually fit over the motor rather than having to repeatedly print a part that was slightly too small and increasing the dimension by tiny increments each time. If the new version turned out to be too loose, I could then work backward and reduce the dimension.

Luckily when altering my design, because I had created relationships and parameters in SolidWorks, I did not need to completely redesign the lid. When I increased the main dimension, the other features remained properly related to the overall design. For example, the top portion of the lid was designed to extend 1 mm beyond the main body on each side. The center opening was also constrained to remain centered. If I had simply drawn every feature independently, changing the overall size could have caused the other features to become misaligned. 

### Updated Design 
After changing the dimension to 35.50 mm, I exported the updated STL and prepared it for another print. The updated model maintained the same general design

<img width="787" height="265" alt="Screenshot 2026-09-28 202705" src="https://github.com/user-attachments/assets/c070e9e0-4ff4-4df8-b554-acb6d6f2b476" />

X: 39.5 mm
Y: 39.5 mm
Z: 15.68 mm

As for my second attempt it turned out to be successful, although difficult to pull apart. 

<img width="208" height="247" alt="image" src="https://github.com/user-attachments/assets/1b9d6fa5-65a9-416e-8e3b-a7ca3c6c0eac" />
<img width="195" height="229" alt="image" src="https://github.com/user-attachments/assets/31b618ac-18c4-4dd6-8803-9d62a35d3cdb" />


## Lessons Learned

One of my biggest lessons was that measurements taken from a physical object are not exact enough to use staright into CAD. I measured the motor body at 34.72 mm and initially added only about 0.2 mm of clearance. However, the first printed part still did not fit. This showed me that I needed to account for measurement uncertainty as well as the tolerances of the 3D printer itself. 

Another lesson is the concept of clearance, especially pertaining to this project. Obviously the printed lid could not be exactly the same dimensions as the artifact, so for the initial design, I used 0.2 mm of additional clearance. And although i followed a guide, it still wasn't enough. This was one of the most important changes during the project. It showed that the measured dimension and the CAD dimension were not necessarily going to produce the same physical fit. 

Another lesson was The most useful feature of my CAD design was the use of parameters and constraints. When I increased the lid size from 34.92 mm to 35.50 mm, I did not have to rebuild the entire model. The center opening remained centered, and the snap-hook support remained related to the rest of the design. This made the redesign much faster and showed the practical value of parametric modeling.

And finally, snap-fit was one of the more complicated parts of the project because it needed to be flexible enough to bend while also being strong enough to hold the lid in place. This influenced my decision to use four perimeters and 15% gyroid infill. The outer walls and snap-hook geometry needed enough strength to survive repeated flexing.

## Time Took 

This project took me 6 hours 

## Recources

[PrusaSlicer](https://www.prusa3d.com/p/prusaslicer/) 

[ProtoLabs Network](https://www.hubs.com/knowledge-base/how-does-part-orientation-affect-3d-print/)

UNC Charlotte Rapid Prototyping 

[Protolabs Network](https://www.hubs.com/knowledge-base/how-design-snap-fit-joints-3d-printing/)

[Rapid Prototyping Solutions](https://rapidprototypingsolutions.se/en/knowledge-bank/order-3d-printing-with-the-correct-tolerances-for-fitment/)

