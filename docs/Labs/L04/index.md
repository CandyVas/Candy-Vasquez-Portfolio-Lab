# A4 – [Topic]

## Parameter
During our lab we learned about the different parameters, benchmark tests 
+ Overhang angle test
+ Pull strength test
+ Tolerance gauge test
+ Dimension calibration test

The one i decided to go with was the tolerance gauge test. Based on the Process and Machine Capability Drives Design Rules a gauge tets must have a hole minimum of .2 mm. Since we were alread working on limited time, i decided to keep this project fairly small to reduce print time. Meaning, my designs gauges will be arounf the .2 mm range. My tolerance stood within a .05mm to .1 mm range.


Before you print, predict the result. Write down what you expect the limit to be. This prediction is part of your documentation and is graded under Preprocessor.

## Document Design
choose your build parameters in PrusaSlicer deliberately, and document why. Infill, build orientation, supports, and scale should all trace back to what your test is trying to measure. A poor choice here can invalidate the test.

<img width="484" height="314" alt="Screenshot 2026-09-10 143224" src="https://github.com/user-attachments/assets/63277687-6728-4817-938a-1c6b116099fa" />
hr ar my hols all mov in qual inrimnts. thy rang from 5.05 mm, 5.10mm, 5.20mm, 5.30 mm, and 5.40 mm. all spaces 10 mm from eachother for the sake of approximately equal width between all the holes so they stay stable.  

<img width="398" height="314" alt="Screenshot 2026-09-10 143356" src="https://github.com/user-attachments/assets/49bdf453-37cf-4dd1-a63f-db762760dd21" />
I then extruded it by the very same 10 mm that is the height of the box. whih rsultd in this as my extrusion. I made sure to include the pin holes in the same sketch layer so there was no need to indivisually perform extruded cuts for them all 

<img width="461" height="235" alt="Screenshot 2026-09-10 143416" src="https://github.com/user-attachments/assets/8b3d47a9-0176-42cb-bb43-9da45effc335" />

The design was built on the front plane fr th eonvenience of printing. Since this design lays flat on the surface, there is no need to overcomplicate the printing. And from that same plane i started another sketch and made a pin of simply 5mm. I made this inside the largest pin hole for the safety measure of this design. If i were to make it in 5.05 theres a chance it wouldnt have even fit or come out, or wvwn worse, fuse when printing because of the temperature. 

<img width="530" height="266" alt="Screenshot 2026-09-10 143443" src="https://github.com/user-attachments/assets/a1b096c8-c2c6-450d-90c4-258b4e463aba" />
<img width="571" height="280" alt="Screenshot 2026-09-10 143734" src="https://github.com/user-attachments/assets/8295dd36-8ec7-420d-a1b1-62b98b225f21" />
The pin is extruded to be a length of 15mm, much longer than the width of the box (10mm). This was designed so that the pin would not get stuck inside the box when measuring, and a longer rod would make it easier to pull out. 
<img width="593" height="340" alt="Screenshot 2026-09-10 143816" src="https://github.com/user-attachments/assets/86106456-8520-45a6-ac8a-3d8fbddfaf8b" />

Finally, for convenicen of th users and aesthetic purposes, i extruded the measurement sizes meant to measure each hole 

<img width="590" height="269" alt="Screenshot 2026-09-10 144539" src="https://github.com/user-attachments/assets/331cb5b2-df31-40c4-858e-8000c67aa074" />

it was then exported as an stl file to prepare it for the printing design. 

## Preprocessor 

Immeditley when importing it into PrusaSlicer, this si the page i was met with. I ws pleasantly surprised with the scaling of my object, i purposefully built it with small measurements so that in case i mistakenly overestimeted how big an inch was, i wouldnt have to scale it down and get my pin holes wrong due to the scaling that went down in Prusa, seperate to the deisgn earlier via CAD. WHen selected, it has the same measurements when created in cad, oriented correctly from the flat plane, so there was no need for alterations in terms of scale. 

<img width="623" height="206" alt="image" src="https://github.com/user-attachments/assets/b921d6dd-b06e-4f3f-829d-4a7e1e66fe45" />

For this design i decide to be adventourous and change the vertical shell peramtiers by 3. This was because i didnt alter this in my last design and i was curious what it contribute to a design. Also i think this was a positive installation as it will make my gauge tester stronger structurally.  The same thought process went into changing the default infill to 25%, and the pattern to be gyroid. 

<img width="664" height="185" alt="Screenshot 2026-09-10 144826" src="https://github.com/user-attachments/assets/acd029b3-7132-4ee3-b7c7-f8b0357e0319" />
<img width="791" height="186" alt="Screenshot 2026-09-10 144836" src="https://github.com/user-attachments/assets/debf4e4b-ba60-4095-a3a1-18d8dbdb84af" />

After these design choices, i sliced my part which resulted in this screen

## Print Artifact 

## Lessons Learned

## Resources 

