# A7 – [Linkage Mechanisms]

## Objective
Design, 3D print, and document a working linkage or mechanism that performs a defined motion or task. You may use purchased hardware such as screws, bolts, pins or springs. All other functional parts must be your own design and must be 3D printed.


## Research

### [Planar Transforming Coiling Linkage](https://link.springer.com/article/10.1186/s40648-025-00289-3)
(Published: 11 February 2025)

> HOW IT WORKS

It is a planar linkage mechanism that uses a series of four bar linkages to create a coiling and uncoiling motion, unlike the traditional scissor linkage that expands and contracts linearly. The coiling linkage transforms between a compact coil to an extended one. The mechanism has one degree of freedom, meaning that one input motion controls the overall configuration of the linkage.

> HOW IT COULD BE USED

+ Aerospace: The compact form can help store deployable supports and spacecraft items to be stored in a small volume and then expandedd.
+ Architecture: The mechanism could be used for deployable structures that need easy transportation since it can transition from a compact storage and a larger structure.

<img width="158" height="190" alt="40648_2025_289_Fig10_HTML" src="https://github.com/user-attachments/assets/19cb99de-bd42-4806-88a1-6375f5835bba" />

> planar linkage mechanism



### [Sarrus-Derived Single-DoF Embracing Gripper](https://link.springer.com/article/10.1007/s40430-025-05388-1) 
(Published: 30 January 2025)

> HOW IT WORKS

This is a linkage that was designed to replicate human hand motion, derived from the classic [Sarrus mechanism](https://www.researchgate.net/figure/A-Sarrus-mechanism-illustrated-in-its-three-different-positions_fig12_277385942). It uses only one degree of freedom, so instead of independently controlling every link, the motion of the linkage coordinates the movement of the entire gripper. It Employs a multi-bar crank-slider finger configuration modeled after human hand movements.

> HOW IT COULD BE USED

Robotics: A gripper like this could pick up and manipulate objects on an automated production line.

Logistics: It could be used on high density orders since it has a large gripping range, which allows the arms to handle varying package sizes.

<img width="260" height="190" alt="40430_2025_5388_Fig3_HTML" src="https://github.com/user-attachments/assets/b418f6a1-31e9-4daf-be8e-149322132637" />

> DoF Embracing Gripper


## Design

For my linkage project, I decided to design a scissor-style lifting mechanism. I chose this type of linkage because scissor mechanisms were one of the examples discussed in class, which gave me a starting point when I began researching different types of linkages. 

After researching scissor mechanisms further, I looked at existing 3D-printable designs and found several examples of scissor lifts. These designs helped me understand how the links, pivot points, and platforms could be arranged. I decided to use the basic concept of a scissor lift while designing my own components and dimensions in CAD rather than directly copying an existing model.

The purpose of my mechanism is to raise and lower an upper platform using the movement of crossed links. The scissor configuration allows the upper platform to remain relatively level while moving vertically. I chose this design because it provided a clear example of how a linkage can convert movement at its joints into useful vertical motion while remaining compact.

<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/c8a61991-f935-4dcf-9786-336b610d7f0c" />

My goal was to create a mechanism that could raise and lower the upper platform while keeping the design small enough to print efficiently. Because the assignment required functional components to be 3D printed, I designed the individual components as separate CAD bodies and assembled them after printing.

### Design

<img width="474" height="196" alt="image" src="https://github.com/user-attachments/assets/a5187f6c-495b-40c1-b6a0-05abdefb43f4" />
<img width="722" height="315" alt="image" src="https://github.com/user-attachments/assets/75e39cd7-68c8-4047-a0f8-cf01d9524d8d" />
<img width="422" height="239" alt="image" src="https://github.com/user-attachments/assets/e18e2178-0f9e-4871-a194-83cea1b6d7e5" />

> I began by designing the upper and lower platforms, which are essentially the same design. I selected the dimensions as a compromise between functionality, size, and print time. Making the platforms larger would have increased the amount of material and printing time without providing a significant benefit to the mechanism.

The platform includes a slot that allows the linkage to move as the mechanism raises and lowers. The dimensions were selected so that the linkage could move through its range of motion without interfering with the platform.

<img width="463" height="152" alt="Screenshot 2026-10-01 151137" src="https://github.com/user-attachments/assets/fb6a3ef9-e9cc-478d-9fa0-07be0da28fb2" />
<img width="545" height="192" alt="image" src="https://github.com/user-attachments/assets/465a9212-5ef3-41a8-b1e1-ee579d8c8cc0" />

> The next component I designed was the scissor linkage itself. The links were designed to cross at a central pivot, allowing them to rotate relative to each other as the mechanism moves. The end features were designed with circular openings so that the rods could act as rotational interfaces. The links needed enough freedom to rotate while remaining connected to the platforms.

The links needed enough freedom to rotate while still remaining connected to the platforms. I therefore had to consider both the geometry of the linkage and the tolerances of the printed components.

<img width="191" height="173" alt="image" src="https://github.com/user-attachments/assets/af6dec38-2aa4-4b79-92b0-5666133ab381" />

> I then designed the center button that connects the crossed links. The opening for this component was designed as a tight fit. I wanted the center pivot to remain in place during operation rather than falling out while the mechanism was being lifted or lowered.

One of the most important design considerations was the tolerance between the printed moving parts. I used the this [website](https://markforged.com/resources/learn/design-for-additive-manufacturing-plastics-composites/3d-printing-strategies-for-composites/composites-3d-printing-design-tips) as a reference for decide the appropriate clearance. Their guide recommends a 0.00–0.05 mm diametral difference for a press fit which i followed. So for the center pivot, I designed the opening to be 5.00 mm, with the goal of creating a very tight/press fit to prevent the button from falling out while the mechanism moved.


<img width="457" height="188" alt="image" src="https://github.com/user-attachments/assets/8835247a-96f7-4c9e-bfe2-fc1b34a4ac86" />

> For the pivot rods, I originally used a 5.00 mm opening but changed the rod diameter from 5.00 mm to 4.65 mm. The final rods were 4.65 mm in diameter and 56 mm long. This was larger than the recommended range from the previous website, but I chose this clearance because I was primarily thinking about allowing the rod to rotate inside the mechanism. However, I did not think enough for the fact that the same rod also needed to remain held by the outside of the linkage. This caused some of the rods to slip out during assembly.

### Compontents

+ Platforms-	Supports the mechanism with upper and lower mounting	(2)
+ Scissor links-	Convert joint movement into vertical lifting motion	(4)
+ Center pivot-	Connects the links at their central pivot	(2)
+ Pivot rods-	Allow the links to rotate at the joints (4)

### Decisions 
1. I chose the scissor configuration because it produces a clear vertical lifting motion while using relatively few components. It also provided a direct connection between my project and the linkage examples discussed in class. Scissor mechanisms are commonly used when a compact mechanism needs to produce significant vertical movement. SOme alternative linkage mechanisms i couldve went with was a Four-bar linkage or a  sliding mechanism.

2. I chose to print the pins and pivot components because it allowed me to control all of the dimensions directly in CAD. I also wanted the finished mechanism to demonstrate that the functional components could be manufactured through 3D printing. The downside was that printed pins have less dimensional consistency and strength than purchased metal hardware.  

3. Changing some tolerences. I changed the rods to 4.65 mm because I wanted the rods to rotate freely inside the openings rather than binding. However, after printing and assembling the mechanism, I discovered that I had created too much clearance. The rods could rotate easily, but some could also move laterally enough to escape from the linkage. This was one of the most important design lessons from the project. The alternative could've been to Keep the original 5.00 mm diameter or to use a slightly smaller diameter.


## 3D Print

<img width="383" height="257" alt="image" src="https://github.com/user-attachments/assets/7ee18ea0-b2b4-4b7c-944b-fa746d784142" />

When importing my design into PrusaSlicer, some of the components appeared vertically oriented. I rotated these components by 90 degrees so that they would print horizontally. This was particularly important for the rods because their orientation affects both print time and the strength of the finished part.

 <img width="477" height="286" alt="Screenshot 2026-10-01 153317" src="https://github.com/user-attachments/assets/7b246aa5-8c51-4152-949c-2062034d411c" />

I initially tried to use automatic supports for the circular rods. However, PrusaSlicer did not generate the support I expected, and the rods were not adequately supported.

<img width="380" height="400" alt="IMG_2275" src="https://github.com/user-attachments/assets/b4bf8133-fda2-4bd6-ba70-e20f0563dda5" />

I encountered a problem about an hour into the print. When I checked on the printer, the main components were printing successfully, but the rods had detached from the print bed and were missing. This made me realize that I needed to reconsider both the orientation of the rods and how their supports were being generated.

I wanted an orientation that considered both print time and part strength. I remembered from a previous lab that parts should not always be printed in the same orientation as their final use because the direction of the layers can affect the strength of the finished part.

<img width="300" height="200" alt="IMG_2278" src="https://github.com/user-attachments/assets/0ed6766f-2751-46e3-874e-23474db1c65f" />

I was hesitant to use this orientation because the rods could potentially become unstable during printing. If the rods fell over during the print, I would have had to restart the print and lose additional time and material. I therefore decided against this orientation.

<img width="400" height="230" alt="Screenshot 2026-10-01 170956" src="https://github.com/user-attachments/assets/af4bd72c-37b1-4d6d-a396-1a1fcf19e718" />

I eventually found the support-enforcer feature in PrusaSlicer. Instead of relying on automatic supports, I selected the rods and manually added support underneath them. After testing the available options, I chose a slab-style support because it provided support along the length of the thin rods without creating a large amount of unnecessary material.

The slab support added 11 minutes of printing time compared to the 45 minutes for the larger support structures I had considered. This was a reasonable tradeoff because the rods received the support they needed without significantly increasing the total print time.

<img width="200" height="194" alt="image" src="https://github.com/user-attachments/assets/5f70b3b5-74c0-4672-8ded-3e9f19c689ba" />
<img width="400" height="180" alt="Screenshot 2026-10-01 172700" src="https://github.com/user-attachments/assets/9b1fb764-d14e-4e89-8c0c-7412a8fbfad9" />

<img width="200" height="183" alt="Screenshot 2026-10-01 173301" src="https://github.com/user-attachments/assets/df766a1e-ffac-4180-bd55-70e31dad0ee2" />

> Manual support added to the rods in PrusaSlicer.

<img width="180" height="200" alt="IMG_2283" src="https://github.com/user-attachments/assets/fb006968-2ac0-4c40-9898-c4a51c1eed7d" />
<img width="180" height="200" alt="IMG_2285" src="https://github.com/user-attachments/assets/4871769c-5bca-40d2-a1e2-a10b4b43039f" />
<img width="180" height="200" alt="IMG_2292" src="https://github.com/user-attachments/assets/ceb68e3a-c9e7-463a-b802-147b9314d97e" />

> Successfully printed rods.

### Assembly 

After printing, I encountered another problem with the supports inside the platform slot. The support material was difficult to remove and left ridges inside the slot. These ridges interfered with the movement of the rods and reduced the mobility of the mechanism.

I initially tried removing the material manually with a knife, but this began to scuff and damage the printed part. I eventually found a method online that recommended soaking the material in water to soften it, which made the remaining support material easier to remove.

<img width="180" height="200" alt="IMG_2296" src="https://github.com/user-attachments/assets/2038b8e6-45b1-4399-945e-a2a5ec19e7f4" />
<img width="180" height="200" alt="IMG_2333" src="https://github.com/user-attachments/assets/3a1256fd-2d9e-4034-acd3-6faf815ab253" />
<img width="180" height="200" alt="IMG_2330" src="https://github.com/user-attachments/assets/58bbb3ca-8742-44e3-8eb6-4a0e252be895" />


After cleaning the parts, I assembled the platforms, links, rods, and center pivot.

<img width="180" height="200" alt="IMG_2335" src="https://github.com/user-attachments/assets/0787db24-f061-4cd0-b965-e0be0c72afb2" />
<img width="181" height="206" alt="IMG_2339" src="https://github.com/user-attachments/assets/3d07f627-fed4-4e25-93f3-a355bf066402" />

The mechanism was able to move through the intended scissor motion, although the rod tolerance caused some assembly problems. Some rods remained in place while others slipped out. This inconsistency demonstrated that the 4.65 mm rod diameter was too small for the 5.00 mm openings.

___ 

## Lessons Learned

### Time
The project took about 6 hours from start to finish. I spent about 1 hour researching linkage designs, about 30 minutes designing the components in SolidWorks, 2 hours printing, and 1 hour removing supports and assembling the mechanism, with the remaining time spent on slicing and documenting. The project took longer than I originally expected because I had to reprint the rods after the first orientation failed. The additional troubleshooting and post-processing took more time than I initially anticipated.

### Biggest Mistake
My biggest mistake was using too much clearance between the rods and the linkage openings. I designed the rods to be 4.65 mm diameter while the openings were 5.00 mm, creating 0.35 mm of diametral clearance. I originally thought this would make the rods rotate freely, but I did not consider that the rods also needed to remain captured inside the linkage. After assembling the mechanism, I discovered that some rods could slip out, which showed me that the clearance needed to be smaller. If I redesigned the mechanism, I would use a rod around 4.85–4.90 mm for a 5.00 mm opening, depending on the printer and material being used. I would also print a small tolerance test before committing to the complete print.

### Tolerances
My first-print clearances worked partially, but they were not ideal for every interface. The center pivot was intentionally designed as a tight fit and successfully stayed in place, while the 4.65 mm rods rotated freely but had too much lateral movement in the 5.00 mm openings. The resulting 0.35 mm diametral clearance was larger than the 0.10–0.20 mm free-fit range. Next time i would reduce the rod clearance to about 0.10–0.15 mm diametral clearance, giving a rod diameter of 4.85–4.90 mm for a 5.00 mm opening. I would also print a small tolerance test before committing to the final print. This would allow me to verify the fit on the actual printer and material instead of relying only on a general tolerance guideline.

## Appendix 

[Sarrus-Derived Single-DoF Embracing Gripper](https://link.springer.com/article/10.1007/s40430-025-05388-1)

[Sarrus mechanism](https://www.researchgate.net/figure/A-Sarrus-mechanism-illustrated-in-its-three-different-positions_fig12_277385942)

[Planar Transforming Coiling Linkage](https://link.springer.com/article/10.1186/s40648-025-00289-3)

[Markforged](https://markforged.com/resources/learn/design-for-additive-manufacturing-plastics-composites/3d-printing-strategies-for-composites/composites-3d-printing-design-tips)
