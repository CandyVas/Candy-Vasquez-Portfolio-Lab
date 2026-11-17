# Final Project – [Manufactured Prototype]

## 1. Research

### A. Spiral Design Process

The Spiral Design Process is an engineering approach that focuses on developing a product through multiple stages of designing and improvement. Instead of expecting the first design to be perfect, the process lets designers to identify problems early and use those findings to improve the next version of their design.

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

There are several ways to reduce the effects of anisotropy:

- Select a print orientation that keeps the main forces from pulling the layers apart.
- Add fillets to reduce stress around corners.
- Increase the number of walls or perimeters to strengthen the outside of the part.
- Use an appropriate infill and pattern.

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

>I also used the Hole Wizard feature in SolidWorks to create the hole for the handle. I selected the legacy hole option, applied the settings shown in my model, and positioned the hole in the center of the screw head. This allowed the handle to pass through the screw and provide a way to rotate it.

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


## Planned Final Assembly

For the next design iteration, I plan to manufacture the wooden platform using the laser cutter. The platform will provide the additional surface area for the plant and will be attached to the C-clamp assembly.

I also plan to create a small SLA-printed spacer or insert to improve the fit between the platform and the clamp. The purpose of this component will be to reduce looseness and improve alignment without making the resin part responsible for supporting the main load.

The final design will combine the flexibility of FDM printing, the surface area and appearance of laser-cut wood, and the detail of SLA printing.

### Threaded Connection

In the first prototype, support material damaged both the external screw threads and the internal threaded hole. For the next version, I plan to test the thread fit separately before printing the entire clamp. I will also experiment with print orientation to reduce support contact with the threads.

### Clamp Fit and Adjustment

The clamp needs to accommodate the thickness of the windowsill or desk. I will need to measure the actual surface thickness before finalizing the opening dimensions.

I also need to verify that turning the screw creates inward movement and applies pressure against the surface. The clamp should not simply slide into position or remain attached because of a tight physical fit.

### Handle Strength

The handle rod snapped on the miniature prototype because scaling the design down made the feature too thin. In the next version, I will avoid scaling down small functional components without checking their minimum dimensions. I will also consider increasing the handle diameter or changing its design.

### Wooden Platform and SLA Insert

The laser-cut wooden platform will need to be checked for dimensions, flatness, and fit with the clamp assembly. I will make a small kerf test before cutting the final platform. The SLA insert will also need a fit test to determine whether it is too tight or too loose. I will make adjustments to its dimensions based on the actual printed result.

### Load and Stability Testing

Once the assembly is complete, I will test whether the platform can support the intended plant without slipping, rotating, or bending. I will begin with a small load and increase it gradually while observing the clamp and platform. I will also check whether the platform moves when a load is placed near its outer edge. This is important because the additional distance from the clamp creates a bending moment that could cause the platform to rotate or sag.

## Video Presentation


https://github.com/user-attachments/assets/76e957aa-b824-449a-95bb-3fd0179d9577



