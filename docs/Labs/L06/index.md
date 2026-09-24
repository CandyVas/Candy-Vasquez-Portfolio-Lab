# A6 – [Topic]

## Objective
(40%) Parametrically design something small that snap fits one of the features of the artifact measured in class. Document the thought and physical process and decisions from measuring the artifact to exporting the stl file. The documentation includes many pictures and images. Capture the design’s use of parameters and constraints.

The object that i ended up grabbing was a gear motor, it seemed to make a design out of. Its a cube with a rod potruding out the top. My intiial idea was to create the snapbased off the cylyndrical rod, however i came to a standstill with the fact that it would need to stop. I then moved to the corners of the cube, which had ridges on the corner. I was thinking an entire lid but one side has the cylinder, and the other has a wire that would interfere with the snap. 

I then thought of a work around, the ideawas to make a cut at the top of my rod so that the cylinder protrudes. so like a cap. Using recources to make this design, i wanted this thing to snap and stick. I used this [website](https://www.hubs.com/knowledge-base/how-design-snap-fit-joints-3d-printing/) to help me brainstorm a design. One big thing is to Taper the design A constant-thickness snap-fit cantilever produces uneven strain, with peaks at the root. 

Typically, a semi-flexible cantilevering hook is deflected slightly as it is inserted into a hole or past a latch plate. As the hook passes the edge of the hole, the cantilever beam returns to its original shape.

I used a calliper to measure the dimensiosn of my motor gear. Read the main scale on the solid beam first to get your whole inches and tenths of an inch (each tick mark equals 0.100 inches). Read the dial to find the extra thousandths of an inch. My first step to measuring were the dimensions of the box, and based ff my caliper i got about 1.3 inches. I decided to confirm this with a regular ruler to make suremy conversions were correct and they were about the same which helped confirmed my readings. I then decided to measure the rest of the box's dimensions. 

1.367 inches (34.72 mm)
.865 in diameter (
.363 in sides (9.22 mm)

i measured the width of the thick where the rudge is on all four corners. luckily they all seemed consistent. 
Since th calliper measures in inches, i figured id keep my solidworks desgn that was as well 

When making my parametric designs, I drew my 2D shape using sketch then added dimensions later. I then use relations so the shape maintains its design intent when resized.

For the internal lid of my gear, since the box itself is 34.72 mm i would need enough clearance for it to fit without bing too tight or loose, so i decided to add a total clearance of just about .2 mm

34.72 mm > 34.92 mm
9.22 mm > 9.42 mm
21.971mm > 22.171
https://www.omc-stepperonline.com/nema-14-bipolar-0-9deg-11ncm-15-58oz-in-0-4a-10v-35x35x28mm-4-wires-14hm11-0404s 

the 34.92 mm still proved to be too small so i increased it to 35.15 mm 

the depth of th ride looked like .078 which looks to be 2 mm.  
i wnt back to my extrusion and reduced the length by half, so i can take into account the length of the snap hook i was going to add on the corners 
 9.42 mm / 2 = 4.71
<img width="590" height="340" alt="image" src="https://github.com/user-attachments/assets/48fea2bc-7dac-46bb-8361-5ec7edd5a410" />

when i initially got my design finalized, i chose the usual gyroid infill to prote strength and 
thanks to the parameters put in place, whe i had to upscale my lid fro, 34 mm to 35, the rest of my deisgn was not ruined. the top lid was made so that it potruded y 1 mm on all sides. and the diameter was centered, so increasing the size didnt make it off center. 

## Analyze


## Decide


## Communicate

