# FINAL PROJECT
# PART 1
## 1. Research

### A. Spiral Design Process

The Spiral Design Process is an engineering method that focuses on developing a product through multiple stages of designing and improvement. Instead of expecting the first design to be perfect, the process lets designers to identify problems early and use those findings to improve the next version of their design.

The process is usually  divided into four main categories:

- **Planning:** Where designers establish the purpose of the product, its requirements, and the limitations that need to be considered.
- **Risk Analysis:** Possible problems are then identified, ones that could affect the manufacturing process or final product. This includes considering material types and its strength, what dimensions to use, and possible failure points.
- **Engineering:** Create the design using CAD software, manufacture prototypes, and test the components.
- **Evaluation:** Examine the results, determine what worked and what did not, and use that information to plan the next design iteration.

According to [TechTarget](https://www.techtarget.com/news/What-is-the-spiral-model-and-how-is-it-used/858209/)'s description of the Spiral Model, each cycle involves planning, risk analysis, engineering, and evaluation. Each prototype builds on the knowledge gained from the previous one which is what I plan to do throughout the development of my windowsill extender.

### B. FDM Anisotropy

[Fused Deposition Modeling](https://rapidmade.com/isotropic-vs-anisotropic-strength-in-3d-printing/) (FDM) is a 3D printing process in which a thermoplastic filament is heated and deposited layer by layer to create a solid object. Since the object is built from separate layers and deposited strands of material, its mechanical properties can vary depending on the direction in which a force is applied. This is known as **anisotropy**.

FDM parts can be stronger along the direction of the deposited filament than in the direction where forces attempt to separate the layers. This is important because the bonding between layers is not always as strong as the material within an individual deposited strand.

For my project, anisotropy is an important consideration because the C-clamp will experience forces when it is attached to the windowsill or desk. The clamp must resist the weight of the wooden platform and whatever is placed on it. If the clamp is printed in an orientation where the layers are pulled apart by these forces, it could crack or fail.

### C. SLA Shrinkage and Dimensional Accuracy

Stereolithography (SLA) is a 3D printing process that uses light to cure liquid resin into solid layers. SLA is useful for producing detailed parts and features that require relatively high dimensional accuracy. Eve so, resin parts can experience dimensional changes during printing and post processing. After printing, the part must be washed and may undergo additional UV curing. During post curing, the resin continues to form polymer bonds, which can cause a small amount of shrinkage.

Shrinkage is important when designing components that must fit together. For example, if an SLA component is designed to fit inside a slot, even a small dimensional difference could make the fit too tight or too loose. There is no univrsal shrinkage percentage that applies to every SLA resin. The amount depends on the resin, geometry, orientation, and post-curing process. Formlabs explains that its software and material settings account for expected shrinkage, but dimensional accuracy still needs to be considered when designing parts with tight tolerances.

Although I don't plan on using SLA For my project, this [research](https://formlabs.com/blog/understanding-accuracy-precision-tolerance-in-3d-printing/) is still useful because even if i don't incoorprate it into my first prototype, perhaps  would like to later.

### D. Laser Cutter Kerf

[Laser cutting](https://making.stanford.edu/resources/process-guides/laser-cutting/design-laser-cutting) is a manufacturing process that uses a focused laser beam to cut shapes out of sheet material. One important factor to consider is **kerf**, which refers to the width of material removed by the laser during cutting. Kerf affects the final dimensions of a part because the laser removes material along the cutting path. For example, if I design a tab and a slot to have exactly the same width, the finished parts may not fit together as expected. The tab becomes slightly smaller, while the slot becomes slightly larger.

This is particularly important when creating press-fit or interlocking joints. If the kerf is not accounted for, the connection may become too loose or too tight. To compensate for kerf, I can create a small test cut using the same wood and laser settings intended for the final platform. I can then measure the resulting dimensions and adjust the CAD design or cutting offset accordingly.

For my project, I plan to use the laser cutter to manufacture the wooden extension platform. The platform will act as the actual surface on which the plant can sit. I will need to account for the thickness of the wood, the dimensions of the platform, and how it attaches to the C-clamp.

## 2. Problem Definition

Before selecting my final project, I considered several everyday problems that could potentially be solved using the manufacturing processes available in class.

### Problem 1: Limited Windowsill Space

<img width="314" height="433" alt="image" src="https://github.com/user-attachments/assets/975ba7e1-e329-4f60-84bd-f6a46bd19179" />

I have a plant sitting on my windowsill, but it is positioned close to the edge and hangs over the side. I am concerned that it could eventually fall, especially if it gets bumped or if the available surface area is not large enough to support it comfortably.

One possible solution would be to create an extension that attaches to the existing windowsill and provides additional surface area. This would allow the plant to sit farther away from the edge without requiring me to replace the entire windowsill or permanently modify it.

### Problem 2: Limited Desk Space

Another issue I considered was the lack of available space on a desk. When a desk is being used for schoolwork, a computer, notebooks, and other items can quickly take up most of the available surface area. A removable desk extension could provide additional room without requiring a larger desk. Ideally, the attachment would be adjustable so it could fit different desk thicknesses and be removed when it is no longer needed.

### Problem 3: Difficulty Organizing Keys and Small Items

I also considered creating a key holder or small entryway organizer. Keys and other small everyday items can easily become misplaced when they do not have a designated storage location. A possible design would use a laser-cut wooden backing with 3D-printed hooks. A small resin-printed label or decorative insert could also be incorporated. Although this concept was possible, I was less interested in it because I felt the windowsill extender offered a more useful solution to a problem I personally experienced.

## 3. Problem Selection

After considering these ideas, I decided to develop the adjustable windowsill extender.

The main reason I selected this problem was that I already had a plant sitting near the edge of my windowsill, and I wanted to give it more room so it would be less likely to fall. Rather than creating a permanent addition to the windowsill, I wanted to design something that could attach and detach easily.

I also wanted the product to have more than one possible use. This led me to design the attachment around an adjustable C-clamp. Since the opening of the clamp can be adjusted, the same product could potentially attach to the edge of a desk as well as a windowsill.

My proposed solution consists of two components:

1. **C-clamp:** The adjustable mounting component that attaches the product to the windowsill or desk.
2. **Wooden extension platform:** A flat surface manufactured using the laser cutter. This acts as the additional table or shelf.

## 4. Concept Development

### Initial Design : C-Clamp

I began by researching existing C-clamp designs and using them as references for my own model. I wanted the clamp to have a simple shape while still providing enough room for an adjustable screw mechanism. 

<img width="410" height="263" alt="Screenshot 2026-11-12 132115" src="https://github.com/user-attachments/assets/68f7c0e2-e682-42d5-af59-509e9f28bc3c" />

> I created the C-clamp body in SolidWorks by sketching its side profile on the right plane.

<img width="413" height="329" alt="image" src="https://github.com/user-attachments/assets/65cb9c66-9097-4b74-a236-b29ece446b17" />
<img width="346" height="317" alt="image" src="https://github.com/user-attachments/assets/4ded8a79-2547-4801-9da6-e312d8e354f5" />
<img width="191" height="265" alt="image" src="https://github.com/user-attachments/assets/53ae1a6a-3af8-4799-900b-2ea2692c8b5f" />

>  I then extruded the profile by 20 mm using the mid-plane option so the part would remain symmetrical. I added an additional 8 mm extrusion to the bottom section and applied fillets to selected corners.

<img width="437" height="343" alt="image" src="https://github.com/user-attachments/assets/05b9125d-c92e-4f59-9539-8b0e198d0f02" />
<img width="255" height="305" alt="image" src="https://github.com/user-attachments/assets/e3edcfc4-08e7-420a-8d37-e97745e5e697" />
<img width="259" height="287" alt="image" src="https://github.com/user-attachments/assets/ef8ede51-1595-400c-9628-12556c4da395" />

> I used the thread feature in SolidWorks to create the threaded opening for the screw. I then designed the screw separately using a revolved sketch and applied a matching thread specification. I also modeled a handle using a 5 mm diameter circle extruded to 96 mm.

For the first version, I selected an M12 × 1.5 mm thread specification. This was an initial design choice that I would need to verify through testing, since the actual performance of printed threads depends on the printer, material, orientation, and clearances. Once the features were complete, I saved this component as the C-clamp.

### Screw 

After completing the clamp body, I designed the screw that would be used to tighten it against the desk. 

<img width="518" height="171" alt="image" src="https://github.com/user-attachments/assets/a09240e6-7303-494f-b4b3-6255030cd249" />
<img width="406" height="254" alt="image" src="https://github.com/user-attachments/assets/02c3931c-7c3a-467d-8869-7b2919a83d2a" />

> I created a sketch of half of the screw's cross-sectional profile. This allowed me to use the revolve feature to create the full cylindrical shape while keeping it symmetrical around its center axis.


<img width="354" height="207" alt="image" src="https://github.com/user-attachments/assets/9b40c65f-dfe4-4105-bc54-4e7e30c20a32" />

> I followed a similar process to create the threaded portion of the screw. I applied the same thread of M12 × 1.5 mm that I used for the clamp opening so that the two components would match.

### Rod

<img width="390" height="113" alt="image" src="https://github.com/user-attachments/assets/cebb1dc5-0fa5-484d-b171-cc897bc56fd0" />

> The handle was relatively simple to model. I created a circle with a 5 mm diameter and extruded it to a length of 96 mm. This would act as the bar used to turn the screw and tighten the clamp.

<img width="274" height="261" alt="image" src="https://github.com/user-attachments/assets/209588d8-78fe-4a00-8bf7-c862a47692ad" />
<img width="352" height="282" alt="image" src="https://github.com/user-attachments/assets/1371020d-4863-4ba2-8b97-0bdf7b8af2c8" />

<img width="354" height="284" alt="image" src="https://github.com/user-attachments/assets/30930912-6df2-4e48-9ab0-433354f57eec" />

<img width="550" height="341" alt="image" src="https://github.com/user-attachments/assets/777f8282-e739-4116-96ea-912e8011a4c4" />

> I also used the Hole Wizard feature in SolidWorks to create the hole for the handle. I selected the legacy hole option, applied the settings shown in my model, and positioned the hole in the center of the screw head. This allowed the handle to pass through the screw and provide a way to rotate it.

### PrusaSLicer

<img width="305" height="275" alt="image" src="https://github.com/user-attachments/assets/89294662-1558-40fd-be4e-8a48c60a9c98" />
<img width="297" height="134" alt="image" src="https://github.com/user-attachments/assets/2d9155b3-bd67-446f-b1ee-5d2eacf9c903" />

Once I had completed the individual components, I imported them into PrusaSlicer to prepare the prototype for printing. The original model was relatively large, and printing the entire design would have taken longer than necessary for an initial test. Since my main goal at this stage was to see whether the components could fit together and whether the screw mechanism would function, I decided to scale the model down by 50%. This would allow me to test the general design without using as much material or time. However, scaling the model down also reduced the size of features such as the handle, screw, and threads. This meant that the smaller prototype could help me evaluate the overall concept, but it would not necessarily prove that the full-size threaded mechanism would work correctly. 

<img width="193" height="238" alt="Screenshot 2026-11-12 143714" src="https://github.com/user-attachments/assets/a518db45-d453-4479-b471-b33b7aab3b68" />
<img width="302" height="120" alt="image" src="https://github.com/user-attachments/assets/a1f9801b-94da-48bb-8ca3-eb71e9ea9b4f" />

For the print orientation, I positioned the parts so that the holes faced upward wherever possible. I wanted to avoid placing support material inside the holes because removing supports from these areas could damage the surfaces and affect how the components fit together. I also wanted to preserve the thread geometry as much as possible.

### Design considerations 

While my C-clamp printed, I considered two possible ways to connect the components:

Option A – Slide-in connection: The component would slide into place, allowing it to be inserted and removed without needing to screw it on.

<img width="318" height="287" alt="image" src="https://github.com/user-attachments/assets/bf933911-8cb5-43d7-a207-ed76d970ad11" />


Option B – Screw-on connection: The component would attach through a threaded connection, making the assembly more secure if the threads worked correctly.

<img width="344" height="278" alt="image" src="https://github.com/user-attachments/assets/c7e2b262-960a-4c60-9b26-8055b5950ae2" />


### Initial Prototype

After printing the scaled-down version, I was able to examine the individual components and see how they interacted. The prototype helped me identify several design and manufacturing problems that were not as obvious while working in SolidWorks.

<img width="329" height="323" alt="image" src="https://github.com/user-attachments/assets/9a37fac3-3738-47b5-b06e-7e69439a9c3b" />
<img width="294" height="343" alt="image" src="https://github.com/user-attachments/assets/ee4d1e22-73d8-4c61-9d19-2d912cc862c4" />
<img width="254" height="416" alt="image" src="https://github.com/user-attachments/assets/3a4aecee-1142-4e37-9121-2725b0a238f2" />

One issue was that some of the smaller components became unnecessary at the reduced scale. For example, the cap and handle rod did not contribute much to turning the screw on the miniature prototype. The handle rod also snapped because it became too thin after the model was scaled down. This showed me that simply scaling an entire design does not always preserve the functionality of every feature. Some components need to be redesigned with minimum dimensions and strength in mind.

## Problems I Encountered 

### 1. Supports interfering with the ridges on the C-clamp

I added ridges to the C-clamp as part of its design, but because of the orientation I selected, the slicer generated support material underneath them. These supports were difficult to remove cleanly and affected the surface of the part.

To improve this, I could either remove the ridges and use a thicker, smoother surface or experiment with a different print orientation. I would need to compare these options to determine which produces the strongest part while minimizing the amount of support material required.

<img width="313" height="323" alt="image" src="https://github.com/user-attachments/assets/c5bbedc2-a91a-4682-a93d-a956321ab90e" />

### 2. Supports damaging the screw threads

I printed the screw horizontally. This created a problem because support material was generated underneath portions of the threaded surface. On one side, the threads printed relatively cleanly, while the opposite side showed visible damage where the supports had contacted the plastic.

Since the threads need to fit closely with the threaded opening in the clamp, even small imperfections could prevent the screw from turning properly. Removing the supports also risked damaging the thread profile. For a future print, I would experiment with a different orientation or another way of manufacturing the threaded components to reduce support contact on the threads.

<img width="306" height="152" alt="image" src="https://github.com/user-attachments/assets/cfe57060-f1df-430b-95cc-404d0560a76e" />
<img width="263" height="113" alt="image" src="https://github.com/user-attachments/assets/e8f9b580-54b7-4393-9735-27a10492947c" />

### 3. Supports inside the threaded hole

The C-clamp body was also printed horizontally. Because of this orientation, support material was generated inside the threaded hole. Removing the supports was difficult, and the process damaged the inside of the hole. As a result, the screw could not properly engage with the threads.

This was one of the most important problems I identified because the screw mechanism depends on the internal and external threads fitting together. For the next version, I would change the orientation or redesign the threaded connection so that support material would not interfere with the threads.

## Final Product 

<img width="252" height="370" alt="image" src="https://github.com/user-attachments/assets/8be72f1c-3eb1-4ece-9a40-113aef83436e" />

Despite these problems, I was able to attach the clamp to the edge of a desk, which showed that the overall C-shaped design was capable of fitting around the desk edge as intended. However, the screw mechanism did not work as expected. Instead of functioning as a screw that gradually tightened the clamp, it mostly acted as a pushing mechanism. It was able to hold its position against the desk, but it did not tighten smoothly or provide the adjustment I originally wanted. I believe this was caused by the damaged threads and support material left inside the threaded hole. The miniature scale may have also contributed because the reduced thread size and handle dimensions made the components more difficult to use.

Overall, this first prototype was useful because it showed me that the basic clamp shape could work, but the threaded mechanism and print orientation needed improvement. My next step would be to revise the design, pay closer attention to the tolerances between the screw and clamp, and test the threaded components at a more realistic size. I would also consider changing the print orientation to prevent support material from interfering with important features.

## Video Presentation

watch my video [here](https://github.com/user-attachments/assets/76e957aa-b824-449a-95bb-3fd0179d9577) 


# PART 2

## Worksheet

After presenting my initial design, I received feedback from three classmates. Overall, the feedback was positive, and people understood the purpose of the windowsill extender. However, they also pointed out a few areas that could be improved before making the final prototype.

<img width="300" height="283" alt="image" src="https://github.com/user-attachments/assets/f2815178-c5fd-4e90-b4e4-d9966d9ab996" />
<img width="200" height="150" alt="image" src="https://github.com/user-attachments/assets/95befd5c-0745-423c-b75d-1d13b9fddf4e" />


> Kaileigh


<img width="300" height="251" alt="image" src="https://github.com/user-attachments/assets/d9b10dd3-dc00-4a60-8ea6-fff601e19299" />
<img width="200" height="150" alt="image" src="https://github.com/user-attachments/assets/a7a40cb4-a3b2-4e4d-9053-620b5266293f" />

> Austin

<img width="300" height="266" alt="image" src="https://github.com/user-attachments/assets/a7e4f620-3757-436e-9979-3580fa78b994" />
<img width="200" height="150" alt="image" src="https://github.com/user-attachments/assets/8e59829b-3ec0-4228-9b9c-9a7a7d4eada3" />

> Ameer

| Feedback | Summary |
| --- | --- |
| Clarity | Overall easy to understand, one suggestion was to include a picture of the actual windowsill to help show why additional space was needed. |
| Functionality| Concerns about stability, the thickness of the wooden platform, and whether the clamp would be strong enough to support a plant. One suggestion was to use clamps on both sides for additional support. | 
| Creativity | People liked the adjustable screw mechanism because it allows the clamp to fit different surface thicknesses. They also liked the idea of using a clamp to create additional windowsill or desk space. | 
| User Experience | Improve the support underneath the platform and making sure the screw threads fit properly. | 
| Iteration FOcus | Most common suggestions was to improve the strength and stability of the platform, confirm that the clamp fits properly, and make sure the threaded components work as intended. | 

## Refinement

I found the feedback helpful because it pointed out areas I needed to focus on when moving from my first test print to the final design. I agreed that stability was one of the most important things to improve, and in order to do that I needed to get the clamp and its threads to actually fit and work. The first test print helped me identify problems with the printed threads, so now I know what not to do. 

One thing I didn't consider before were FDM clearances and, so that means i need to make adjustments to the dimensions before printing at full size. Instead of adding clamps like someone suggested, I decided I'd rather focus on improving the connection between the existing clamp and the wooden platform. 

### Removed Ridges 

<img width="245" height="257" alt="image" src="https://github.com/user-attachments/assets/813218d0-b688-4d18-a12a-39588c2f9472" />

I removed the ridges from the clamp. This made the design simpler and reduced the need for support material during printing. In the first print, support material had caused problems around the threaded area, making it difficult to remove and it damaged the threads.

### Clearance

<img width="185" height="163" alt="Screenshot 2026-11-18 150423" src="https://github.com/user-attachments/assets/b33595ec-6ff6-40ab-8ec7-3567f556cfbd" />
<img width="131" height="193" alt="image" src="https://github.com/user-attachments/assets/5d830ea6-32d6-417b-955d-0bab58e3dc10" />


Another important adjustment involved the threaded connection. In my initial model, I had used a 12 mm dimension for both the screw and the hole. However, the printed parts did not engage with each other properly. I adjusted the internal thread dimensions, using a 10.5 mm minor diameter for the hole while keeping the screw's nominal diameter at 12 mm. This gave the threaded components a better chance of engaging properly. The final fit still needed to be checked through assembly.

### Extension

<img width="302" height="243" alt="image" src="https://github.com/user-attachments/assets/1abdfb5a-962f-4ea3-8316-de19fc3b9bd8" />
<img width="167" height="283" alt="Screenshot 2026-11-18 144336" src="https://github.com/user-attachments/assets/5ffa62cf-623c-46f2-979b-81b77a67a722" />

I also included the extender platform in this version so that I could evaluate the complete design rather than just the clamps function. To improve the connection between the clamp and the platform, I added a screw and slot. This increased size for it to rest on (slit) and helped secure the platform to the clamp and makes the connection more stable (screws). 

### Upscaled

<img width="542" height="410" alt="Screenshot 2026-11-19 135948" src="https://github.com/user-attachments/assets/bd370996-da33-4526-9054-3807f5f13509" />

Finally, I printed the clamp at its original designed size instead of scaling it down. The first print was useful for identifying problems, but scaling it down also made some features too small to properly evaluate. For the next version, I used the actual dimensions intended for the windowsill.


## Documentation


<img width="396" height="271" alt="Screenshot 2026-11-19 170545" src="https://github.com/user-attachments/assets/cc425946-a26f-4743-a910-8a47aab020af" />
<img width="378" height="271" alt="Screenshot 2026-11-19 170741" src="https://github.com/user-attachments/assets/4cd0ebab-a41e-401b-ac5d-7110d77625e6" />

While the 3D-printed parts were being manufactured, I started designing the wooden platform for my desk extender. I created the design in SolidWorks and then exported it to Inkscape to prepare it for laser cutting.


<img width="206" height="229" alt="Screenshot 2026-11-19 171825" src="https://github.com/user-attachments/assets/99d54aa2-6a29-475c-9bd8-782fd3f41d3a" />
<img width="206" height="270" alt="Screenshot 2026-11-19 172621" src="https://github.com/user-attachments/assets/c4f7a4b6-b844-4733-8a2d-1e54261aa3d9" />
<img width="830" height="397" alt="Screenshot 2026-11-19 191213" src="https://github.com/user-attachments/assets/65178db6-5553-453b-8291-683cf2b6529b" />

Since the laser cutter also has an engraving feature, I decided to add a flower design to the wooden platform. I thought this would be a nice detail because the extender is primarily intended to hold a plant. After finishing the design and engraving, I laser-cut the wooden platform. 

<img width="656" height="403" alt="image" src="https://github.com/user-attachments/assets/5f53ffd1-b6f6-40e5-a24e-8e2ad7d3b50b" />
<img width="656" height="400" alt="image" src="https://github.com/user-attachments/assets/02ddd040-fd1c-40d2-8227-2a32de911dd4" />

Here are the completed results- the wooden platform and the C-clamp!

### Assembly Instructions: 

1. Position the C-clamp around the edge of the windowsill or desk.
<img width="379" height="406" alt="image" src="https://github.com/user-attachments/assets/3748321c-ff36-4196-8933-5c794942efff" />

2. Turn the adjustment screw until the clamp grips the surface securely. Avoid overtightening.
<img width="379" height="406" alt="image" src="https://github.com/user-attachments/assets/97d43141-fbf5-4284-b9eb-fbd93ed0bd52" />

3. Align the wooden extension platform with the clamp.
<img width="334" height="251" alt="image" src="https://github.com/user-attachments/assets/a4b9f483-01ad-43f4-a7d0-8b8c62953615" />

4. Use the screw-and-slot connection to attach the platform to the clamp.
<img width="331" height="353" alt="image" src="https://github.com/user-attachments/assets/f3e46377-a205-4153-a445-137db3810c23" />

5. Place the intended object, such as a potted plant, onto the platform.
<img width="320" height="350" alt="image" src="https://github.com/user-attachments/assets/06280335-485f-4c44-81b4-3e6b52c05aa0" />

## Presentation 

<img width="618" height="343" alt="image" src="https://github.com/user-attachments/assets/1cba2236-b6ac-45da-adc7-cc15e9cc7404" />

## Parametric Design

To make the design more adjustable, I included a parametric feature in my SolidWorks model to control the wooden slot for of the C-clamp.

<img width="393" height="320" alt="image" src="https://github.com/user-attachments/assets/0d985922-1978-4b94-9252-40868fbbe456" />

Instead of manually changing the clamp dimensions each time I want to fit a different surface, I can link the opening dimension in my sketch to this variable. Changing the variable will update the model automatically.

## Final Video
Watch my final video [here](https://photos.google.com/u/1/photo/AF1QipOFWT1vONUCfCuDDbKK7XZtiwO8PggkDi9bkbOG)
Produce a 1–2 minute video summarizing your work.
Include:
The problem and motivation
Your manufactured solution
How both FDM and SLA technologies were utilized
