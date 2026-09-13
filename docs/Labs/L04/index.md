# A4 – [Topic]

## Parameter
During our lab we learned about the different parameters and benchmark tests that evaluate the capabilities of a specific 3D printer. They include... 
+ Overhang angle test
+ Pull strength test
+ Tolerance gauge test
+ Dimension calibration test

The test that I decided to go with was the tolerance gauge test. Based on the *Process and Machine Capability Drives Design Rules* a gauge test must have a  minimum hole size of at least .2 mm and go up small differences to determine it's accurascy.

Since we were already working on limited time, I decided to keep this project fairly small to reduce the printing time. My goal was to create a gauge with holes that were close together in size so I could determine the printer's ability to make small changes and i gave my design a tolerance range of 0.05 mm to 0.10 mm.

## Document Design

<img width="484" height="314" alt="Screenshot 2026-09-10 143224" src="https://github.com/user-attachments/assets/63277687-6728-4817-938a-1c6b116099fa" />
I began by creating the main body for the gauges, then I added five holes, each with a slightly different diameter. The holes range from 5.05 mm, 5.10mm, 5.20mm, 5.30 mm, and 5.40 mm. The holes are all spaced 10 mm apart from one another so that there is an equal amounts of material between each hole. 

<img width="398" height="314" alt="Screenshot 2026-09-10 143356" src="https://github.com/user-attachments/assets/49bdf453-37cf-4dd1-a63f-db762760dd21" />

I then extruded the main body by 10 mm, which was also the height of the box. I included all of the pin holes in one sketch so that they would be created simultaneously rather than having to individually extruded cuts for every hole.

<img width="461" height="235" alt="Screenshot 2026-09-10 143416" src="https://github.com/user-attachments/assets/8b3d47a9-0176-42cb-bb43-9da45effc335" />

The design was built on the Front Plane for the convenience of printing. Since this design lays flat on the printing surface, there was no reason to overcomplicate the printing orientation. Keeping it flat also meant that I wouldn't need supports.

From that same plane, I started another sketch and made a pin that was simply 5 mm in diameter. I made this based on the largest pin hole as a safety measure for the design. If I were to make the pin exactly 5.05 mm, there was a chance that it wouldn't even fit through the hole or could potentially get stuck. There was also a possibility that the pin could fuse with the surrounding material while printing because of the heat.

<img width="530" height="266" alt="Screenshot 2026-09-10 143443" src="https://github.com/user-attachments/assets/a1b096c8-c2c6-450d-90c4-258b4e463aba" />
<img width="571" height="280" alt="Screenshot 2026-09-10 143734" src="https://github.com/user-attachments/assets/8295dd36-8ec7-420d-a1b1-62b98b225f21" />

The pin was extruded to a length of 15 mm, which is longer than the 10 mm width of the box. I did this so that the pin wouldn't get stuck inside the box while measuring. Having a longer rod also made it easier to grab and pull out when testing the different holes.

<img width="593" height="340" alt="Screenshot 2026-09-10 143816" src="https://github.com/user-attachments/assets/86106456-8520-45a6-ac8a-3d8fbddfaf8b" />

Finally, for the convenience of the user and for aesthetic purposes, I extruded the measurement sizes onto the box so that it would be easy to tell which hole was which.

<img width="590" height="269" alt="Screenshot 2026-09-10 144539" src="https://github.com/user-attachments/assets/331cb5b2-df31-40c4-858e-8000c67aa074" />

I then exported the design as an STL file to prepare it for printing.

## Preprocessor 

Immediately when importing it into PrusaSlicer, this is the page I was met with. I was pleasantly surprised with the scaling of my object. I purposefully built it with small measurements so that, in case I mistakenly overestimated how big an inch was, I wouldn't have to scale it down and potentially mess up my pin holes because of the scaling done in PrusaSlicer.

When selected, it had the same measurements that I created in CAD. It was also oriented correctly from the flat plane, so there was no need for any alterations in terms of scale or orientation.

<img width="623" height="206" alt="image" src="https://github.com/user-attachments/assets/b921d6dd-b06e-4f3f-829d-4a7e1e66fe45" />

For this design, I decided to be a little more adventurous and change the vertical shell parameters to 3. This was because I didn't alter this in my last design, and I was curious to see what it would contribute to the design. I also thought this would be a positive addition because it would make my gauge tester stronger structurally and hopefully prevent it from flexing while I was testing the holes. The same thought process went into changing the default infill to 25% and changing the pattern to gyroid. I wanted the gauge to have some additional strength while still keeping the print time reasonable.



<img width="664" height="185" alt="Screenshot 2026-09-10 144826" src="https://github.com/user-attachments/assets/acd029b3-7132-4ee3-b7c7-f8b0357e0319" />
<img width="791" height="186" alt="Screenshot 2026-09-10 144836" src="https://github.com/user-attachments/assets/debf4e4b-ba60-4095-a3a1-18d8dbdb84af" />

After making these design choices, I sliced my part, which resulted in this screen.

<img width="617" height="197" alt="image" src="https://github.com/user-attachments/assets/ce6feb1f-7016-4c4a-aead-88585df0288f" />

I was given an estimated time of about 30 minutes, which was a little shocking at first. However, after looking at the cross-section, I realized that gyroid is a pretty intricate design compared to the grid infill that I'm used to. I decided to compare it to a 25% grid infill to see if the time would be any faster. Not to anyone's surprise, it was slightly faster, but not by a whole lot.

Since the difference wasn't very significant and the gyroid was not only stronger but also cooler, I decided to keep it for the final print.

<img width="491" height="358" alt="image" src="https://github.com/user-attachments/assets/6c5e10a9-7d2c-4ef6-9eb9-a31eb4a170aa" />
<img width="578" height="192" alt="image" src="https://github.com/user-attachments/assets/96ca30b5-0d4f-437b-bf76-ed45684a0854" />

From there i exported my original gyroid infilled gauge tester as a G-code file to get ready to physically print it. 

###Predictions

Now that I finally had my design finalized and knew what size holes and pin I was going to use, I predict that the middle hole would fit the best. Since there are 5 holes total, I expect one end to be really loose and the other end to be too tight. Since my pin is 5 mm, I figured that the fit would slowly become looser as the diameter increased.

For example...
+ 5.05 mm will not fit
+ 5.10 mm will have a tight fit
+ 5.20 mm will be perfect 
+ 5.30 mm will be a loose fit
+ 5.40 mm will be extremely loose 

## Print Artifact 


<img width="282" height="194" alt="Screenshot 2026-09-13 142152" src="https://github.com/user-attachments/assets/f2884a7d-1fbd-4aa1-970f-7d82f6b03715" />

> Once I was ready to print, I used the printer belonging to PC-07 because it uses PLA as its printing material, which was the material I selected for my G-code.

WAtch the video of it beig printed [here](https://github.com/user-attachments/assets/3427958a-d2df-4641-a2cd-e4be76187d06) 
https://github.com/user-attachments/assets/3427958a-d2df-4641-a2cd-e4be76187d06 

<img width="213" height="249" alt="image" src="https://github.com/user-attachments/assets/eca0199b-d513-41c1-944f-32109e5da41f" />
<img width="197" height="143" alt="image" src="https://github.com/user-attachments/assets/8661704d-88e5-444c-9f25-1b9d5ad77462" />

> The print successfully completed and was removed from the printing plate.


<img width="558" height="285" alt="image" src="https://github.com/user-attachments/assets/bf6a869b-8163-4f6e-ab44-9bc478887916" />
<img width="491" height="262" alt="image" src="https://github.com/user-attachments/assets/904e6568-f72c-4451-aa23-3a185c10688f" />

After removing the gauge from the print plate, I decided to go a step further and measure the dimensions of the holes using a caliper. This proved to be somewhat difficult because the increments between some of the holes were extremely small.

Even though the differences were not drastic, the caliper showed that there were small dimensional changes between the holes. Because the increments were so small, even moving the caliper slightly could change the measurement. This demonstrated one of the challenges of measuring small tolerances manually.

<img width="296" height="261" alt="image" src="https://github.com/user-attachments/assets/51b56170-4387-4479-a293-c5a229f9087f" />
<img width="296" height="261" alt="image" src="https://github.com/user-attachments/assets/19c2aff3-d428-43fb-a826-9bf54654044b" />
<img width="296" height="261" alt="image" src="https://github.com/user-attachments/assets/47fd92e7-2afe-4fb2-a8cf-1b866245484e" />
<img width="296" height="261" alt="image" src="https://github.com/user-attachments/assets/daab1c88-d5eb-4ec6-990e-b4a9d288adc7" />
<img width="296" height="261" alt="image" src="https://github.com/user-attachments/assets/fda47568-620e-44b6-9595-e310cb893c39" />

<img width="296" height="261" alt="image" src="https://github.com/user-attachments/assets/fb19ff59-74c8-46cd-8da1-71e8fa22610a" />

I then tested the 5 mm pin against each of the holes in my design. When comparing the pin to the holes, the results were somewhat different from my original prediction. The 5.05 mm hole was too small for the pin, as expected. The 5.40 mm hole was also too large, allowing the pin to pass through very easily. However, the 5.30 mm hole was also loose enough that the pin could slip completely through. This was slightly different from my original prediction, since I expected the 5.30 mm hole to be loose but not loose enough to pass through completely. 

The middle hole (5.20 mm) was a perfect fit right out the printer and moved just like how I predicted. However, after tinkering with the part too much and inserting and removing the pin, now it has an inconsistent fit. Sometimes the pin would remain in the hole, while in others it would slip through more easily.

## Lessons Learned

### different outcome 
The outcome was mostly the same as what I originally thought. I predicted that the 5.05 mm hole would be too small, the 5.20 mm hole would be the best fit, and the 5.40 mm hole would be extremely loose. After testing it though, my biggest surprise was the 5.30 mm hole being loose enough for the pin to slip through. But after further research on tolerance using this [website](https://www.sovol3d.com/blogs/news/fdm-3d-printing-tolerances-clearances-how-to-design-parts-that-fit) I understood my results more since they discusses different types of fits, such as press fits and sliding fits, and also mentions PLA as a good material for this type of project, which happened to be the material that I used. 

### compare result
I would say that the printer exceeded the documented FDM specification. The class design rules list a minimum tolerance of 0.2 mm, while my gauge was able to show differences between holes using increments as small as 0.05 mm. The 5.20 mm hole also gave me a good fit with my 5 mm pin, showing that the printer was able to produce a functional fit at a smaller clearance than the documented specification. 

### 4 lessons 
+ Test more tolerances: I would use more holes with smaller increments around the successful range, such as 5.15 mm, 5.20 mm, 5.25 mm, and 5.30 mm.
Use multiple pins: I would test multiple pin sizes instead of only using a 5 mm pin. This would give me a better understanding of the actual clearance between the pin and holes.
+ Improve the lettering: The letters identifying the hole sizes ended up somewhat blended together. I think the spacing was too close or the letters were too small for the printer to reproduce properly . Even though they did not print perfectly, they were still useful for identifying which hole was which.
+ After researching FDM tolerances more, I wish I would have experimented with multiple pins instead of only using one 5 mm pin. Having several pins with slightly different diameters would allow me to test the gauge from both directions.
+ Limit repeated testing: Repeatedly moving the pin through the same hole changed the friction and made the fit less consistent. I would try to limit this or use multiple test pieces.

### Time took
The print itself took approximately 36 minutes, according to PrusaSlicer. The full project took 4 hours. 

## Resources 

[SOLOV](https://www.sovol3d.com/blogs/news/fdm-3d-printing-tolerances-clearances-how-to-design-parts-that-fit)
Design Rules for 3D Printing PDF
