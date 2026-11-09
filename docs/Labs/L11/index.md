# L11 – SLA Snap Fit

## Objective


## Snap Fit Research

A snap fit joint is a way to connect two or more parts and it works by using a flexible feature on one part, such as a hook or clip, that bends while being pushed into another part. Once it passes, it returns to its original position and locks into place. Depending on the design, the two parts can either be taken apart or stay permanently connected. The amount of force needed to connect or separate them depends on the shape, size, and flexibility of the snap fit.

For my project, I focused on a cantilever snap fit since it was the one i was most familiar with. This type of design uses a flexible arm with a hook at the end so when the parts are pushed together, the arm bends to allow the hook to pass the edge of the other part and connect. 

<img width="197" height="241" alt="image" src="https://github.com/user-attachments/assets/01ae782d-e9ae-42f9-9d78-c88f468c1b2f" />

In the design guide "Snap-Fit Joints for Plastics" it shows an example of a box with four cantilever hooks. The hooks are meant to keep the box secure, but still allow it to be removed when needed. This is a good example of how cantilever snap-fits can be used in everyday products where parts need to stay connected but may also need to be removed.

One important part of this design is the thickness of the flexible arm. If the arm is too thick, it will be harder to bend and will require more force to assemble. If it is too thin, it may become weak and break. The design guide explains that reducing the arm thickness toward the hook can help spread the bending across the arm instead of placing too much stress in one area. This is also shown in the image above which what is represented by "h" and "h/2"


<img width="326" height="212" alt="image" src="https://github.com/user-attachments/assets/41e290bb-439e-415e-b55f-4a1425f0790e" />
<img width="391" height="215" alt="image" src="https://github.com/user-attachments/assets/3890cebc-d602-4c3f-a021-58e2a60f9d76" />

The root of the cantilever is one of the most important areas because this is where the arm experiences the most bending. If the corner is too sharp, stress can build up in that area and increase the chance of the arm cracking or breaking. To help prevent this a rounded corner (or a fillet) can be added where the arm connects to the main body. On that same note however, the radius can not be too large because making this area too thick can create other problems like uneven material thickness and internal stress. For this reason, the design needs a balance between having a smooth connection and avoiding areas that are much thicker than the rest of the part. 


<img width="529" height="236" alt="image" src="https://github.com/user-attachments/assets/6926da0a-3d30-45a9-9873-ffd67c8441ab" />
<img width="501" height="346" alt="image" src="https://github.com/user-attachments/assets/aaf3261c-9253-4521-8ed1-898869a0ebf1" />

Deflection is the amount that the cantilever arm bends when the two parts are pushed together. The undercut is the amount of overlap between the hook and the part it catches onto. The hook needs to bend far enough to pass the edge of the other part, but not to the point where it gets damaged.

The amount of bending a snap fit can handle depends on the material and its ability to stretch without breaking. A material that is more flexible can usually handle more deflection than a material that is stiff or brittle. The design guide also shows different cross section designs for a cantilever snap joint hook designs. For my design, I decided to focus on Column A because it was the most relevant to the type of design I wanted to create.

Since I was using SLA resin, I also had to consider that the material may not bend as easily as some other plastics commonly used for snap fit parts. This meant that I needed to be careful with my design and do some extra research.

## CAD

The type of snap fit I wanted to design was a cantilever snap fit. My goal was to create a small box with a removable lid that could lock into place using hooks on the sides. Using [Protolabs Network](https://www.hubs.com/knowledge-base/how-design-parts-sla-3d-printing/) I followed design specifications recommended for SLA printing, including the minimal thickness and heights for a design to function. 

<img width="222" height="168" alt="image" src="https://github.com/user-attachments/assets/bb6fe514-6863-43f2-9e06-17ca8397de33" />

### Lid

I started by creating a sketch on the top plane. I drew a centered square measuring 60 mm by 60 mm and extruded it by 2.5 mm to create the base of the lid.

<img width="270" height="245" alt="image" src="https://github.com/user-attachments/assets/df703c7b-adf0-488d-8172-4c358bfe5029" />
<img width="566" height="310" alt="image" src="https://github.com/user-attachments/assets/03e0345c-8fe8-455f-9023-f70154d563ca" />

I used the centerline feature to ensure that my hook extrusions would be centered from the lid box. I made it a box that was 5 mm by 2.5mm, extruding it outwards by 15 mm then used the mirror feature to do the same on the other side. 

<img width="444" height="317" alt="image" src="https://github.com/user-attachments/assets/d408e033-422e-4fe6-84bd-cec0f62a1ebc" />
<img width="467" height="278" alt="image" src="https://github.com/user-attachments/assets/ffe259c4-6ad1-4701-bf67-d83fff73d93c" />

Next, I worked on the hooks. I created a 1.5 mm line and shaped it into a triangle to form the hook. The triangular shape was intended to help the hook catch onto the box and prevent the lid from coming off easily.

<img width="244" height="204" alt="image" src="https://github.com/user-attachments/assets/f30680c9-ddc8-4994-bc83-daae557afe9e" />

After creating the first hook, I repeated the same process on the opposite side by mirroring the feature. I then extruded the hooks to give them the shape needed to engage with the box.

<img width="487" height="191" alt="image" src="https://github.com/user-attachments/assets/fcc648e7-25f7-4f3a-b1c0-ea719c82f69b" />

Finally, I added fillets where the hooks connect to the lid. I did this to create smoother corners and reduce stress in the areas where the hooks would bend during assembly.

### Box

Next, I selected the top face and used the shell feature with a thickness of 2.5 mm. This hollowed out the inside of the box while keeping the walls at a consistent thickness.

<img width="443" height="292" alt="image" src="https://github.com/user-attachments/assets/a09bda29-282a-450c-b883-c43b49214d88" />
<img width="443" height="264" alt="image" src="https://github.com/user-attachments/assets/09a72696-c935-4c2e-a01c-945c281077ab" />
<img width="491" height="319" alt="image" src="https://github.com/user-attachments/assets/0754b2fd-c68f-4f5d-bcd7-8cfb920e725c" />

I did not need to shell the other side because I was able to create the opening by extruding through the opposite side of the box.

<img width="164" height="275" alt="image" src="https://github.com/user-attachments/assets/dcafd1fa-8cb1-4ce3-a1ad-ecf33a37734d" />
<img width="159" height="203" alt="image" src="https://github.com/user-attachments/assets/8270a02a-624c-44ff-997a-f410be52e464" />
<img width="376" height="259" alt="image" src="https://github.com/user-attachments/assets/5b5d1bc3-b726-4387-a217-427c1a780586" />

After that, I worked on the areas where the hooks would connect to the box. These features were important because they needed to line up with the hooks on the lid so that the two parts could snap together.


<img width="571" height="287" alt="Screenshot 2026-11-03 150317" src="https://github.com/user-attachments/assets/8e370787-2bdc-4402-86a0-dcb8b7a530f3" />
<img width="338" height="296" alt="Screenshot 2026-11-03 150428" src="https://github.com/user-attachments/assets/3a7795eb-0062-4d8d-923a-8d5c661284c3" />
<img width="414" height="269" alt="image" src="https://github.com/user-attachments/assets/0d38f59d-0867-43e5-8b68-a43572eea489" />

After completing both parts, I checked that the lid and box lined up correctly. The goal was to create a connection that would hold the lid in place while still allowing it to be removed when needed.

The final design uses the cantilever hooks to create a mechanical connection between the lid and the box. This makes it more useful than a simple lid that only rests on top of the box.

## Preprocessing and 3D Print

When preparing my design in PreForm, I wanted to avoid placing supports inside the box because I was concerned that removing them could damage the interior or affect the fit between the lid and the box. I tried several different orientations, but I found that completely avoiding supports inside the box was difficult. Some orientations also created weak areas, which PreForm highlighted in orange.

I eventually settled on the orientation shown below. Although some supports were still needed inside the box, I made sure they did not touch the snap-fit features. This was important because I wanted to keep the hooks and connection areas as clean and accurate as possible.

<img width="200" height="149" alt="image" src="https://github.com/user-attachments/assets/648748bd-466d-40a5-b483-a476ed8f869c" />
<img width="316" height="194" alt="image" src="https://github.com/user-attachments/assets/dab3cc1b-ad71-4cfc-a5e5-9172cfa4b8c5" />

<img width="323" height="391" alt="Screenshot 2026-11-03 152407" src="https://github.com/user-attachments/assets/6ed24bdf-c916-4a77-81de-a20f7686abe0" />

When I arrived at the FabLab, I originally planned to print using the printer I was familiar with, HiddenCod. I had already prepared my settings based on the material I planned to use.

However, HiddenCod was already being used, so I had to switch to another printer called MatureImpala. Luckily, both printers had the same settings already installed, including the same resin used which was ClearV5, so I was able to continue with my prepared setup without making major changes.

For the slicing process, I used the default settings provided in PreForm. I did not make any major changes to the support or resolution settings.

<img width="215" height="425" alt="Screenshot 2026-11-05 125135" src="https://github.com/user-attachments/assets/17fc86cd-a89e-4a10-8099-ab59104279d7" />
<img width="208" height="218" alt="Screenshot 2026-11-05 125202" src="https://github.com/user-attachments/assets/c36d5650-1740-4819-8560-bd292405f8ee" />

SLA printing is generally considered anisotropic because the strength of a printed part can change depending on the direction of the force and how the layers are connected. Since the Form 4 builds parts one layer at a time, the bond between layers may not behave exactly the same as the material within each layer. This is important for my design because the hooks need to bend slightly when the lid is attached.

I had to consider the printing direction because I did not want the hooks to break when they were being pushed into place.


## Post-Processing

<img width="284" height="222" alt="image" src="https://github.com/user-attachments/assets/0e435c75-54a9-434a-abef-4f3937331825" />
<img width="288" height="228" alt="image" src="https://github.com/user-attachments/assets/360d93b9-78dd-47b0-b649-2672bf834ced" />


After the print was complete, I moved on to post processing. One thing that worked out well was the support placement. Since I had kept the supports away from the main snap-fit features, I did not have to sand those areas down or worry about changing the shape of the hooks. The FabLab provided wire cutters, which made removing the supports much easier.

<img width="345" height="266" alt="image" src="https://github.com/user-attachments/assets/fb23c50a-2917-4f49-8295-1c5752bd01c4" />
<img width="368" height="257" alt="image" src="https://github.com/user-attachments/assets/600c560a-1778-4b63-8f86-55cec4daad4e" />
<img width="308" height="335" alt="image" src="https://github.com/user-attachments/assets/f4971046-aeb2-4bbd-9957-02d4b2abab7c" />


After removing the supports, I washed the parts for 5 minutes to clean off any uncured resin left on the surface. Once they were washed, I placed them in the curing machine for 15 minutes to finish hardening the resin.

<img width="298" height="258" alt="image" src="https://github.com/user-attachments/assets/bb0b3767-6ee1-499c-92c3-ca6522f6be02" />
<img width="329" height="290" alt="image" src="https://github.com/user-attachments/assets/f6d863d1-ebc8-4eb1-b843-ddac72ff3626" />
<img width="323" height="344" alt="image" src="https://github.com/user-attachments/assets/ae022cbe-e540-4228-b174-31888f7d118b" />

> Washing process - 5 minutes

<img width="355" height="292" alt="image" src="https://github.com/user-attachments/assets/bfecf8c1-ba08-4e21-83e6-402d96cc65a8" />
<img width="265" height="341" alt="image" src="https://github.com/user-attachments/assets/aa0b2219-8a09-4890-ad27-11f2734e990e" />

> Curing process - 15 minutes 

One thing I noticed about the curing process was that it made the parts feel stiffer. Since my design relied on the hooks bending slightly, I was worried about attaching the lid before the resin had fully cured because I did not want the hooks to break. I decided to wait until the curing process was finished before testing the snap fit. This made me realize how important the material is when designing something that needs to bend. The hooks needed to be flexible enough to connect the lid to the box, but also strong enough to hold it in place. SLA and FDM printing have some important differences, especially when it comes to strength and flexibility.

SLA printing uses liquid resin that is hardened using UV light. One advantage is that it creates a smoother surface and can capture smaller details. This is helpful for snap fit designs because the hooks and openings need to line up properly. FDM printing uses melted plastic that is pushed through a nozzle and built up layer by layer. This usually leaves visible layer lines on the surface. Depending on the material used, FDM parts can sometimes be more suitable for flexible snap fit designs.

Another difference is how the parts handle stress. Some SLA resins can be more brittle and may crack if they are bent too far. PLA can also be stiff and brittle, but other FDM materials, such as PETG, can offer more flexibility. For my project, the smooth surface of SLA printing helped create clean fitting areas. However, I had to be more careful with the hooks because I did not want them to bend too far and break.

## Validation

After printing and post processing both parts, I tested the lid to see if it would properly snap onto the box. The results were good. The hooks were able to connect to the box and hold the lid in place. The fit was not too tight or too loose. It felt just right, which meant the lid could be attached without too much force while still staying securely connected.

<img width="375" height="247" alt="image" src="https://github.com/user-attachments/assets/43b81a04-b59d-433a-bfc3-89244e9494ac" />

> Box Unnassemled

<img width="248" height="224" alt="image" src="https://github.com/user-attachments/assets/284891ac-55eb-4f79-aca9-dd48d3bc9dca" />
<img width="223" height="242" alt="image" src="https://github.com/user-attachments/assets/45ebf4a5-d239-4327-97fa-d8cfb5ca8288" />

> Box Assemled

During testing, I found that the snap fit worked as intended. The hooks were able to engage with the openings in the box and hold the lid securely. One thing I noticed, however, was that getting the hooks lined up with their openings took a little effort. The lid sometimes needed to be adjusted before everything lined up properly. If I were to improve the design, I would add small guide walls inside the box. These walls would help direct the hooks toward the correct openings when putting the lid on. This would make assembly easier because I would not have to spend as much time manually aligning the hooks. Even though the alignment could be improved, the snap fit itself worked well. The lid stayed in place, and the connection was secure.

## Lessons Learned

### Challenges During the Design Process

One of the biggest challenges I faced was designing the hooks around the properties of SLA resin. Since the hooks needed to bend during assembly, I had to be careful not to make them too thick or too stiff. I also had to think about the clearance between the lid and the box. Even a small difference in the dimensions could affect how the parts fit together. If the hooks did not have enough room, they could get stuck or break. If there was too much space, the lid would not stay in place.

Another challenge was figuring out the best print orientation. I wanted to avoid placing supports inside the box, especially near the snap-fit features. After trying different orientations, I found one that worked well without placing supports directly on the areas that needed to fit together.

### SLA Tolerances & Print Orientation

One thing that this project helped me understand that a design that looks correct in CAD does not always work exactly the same way once it is printed. Clearance is especially important when designing snap fit parts because the two components need to fit together without requiring too much force. I also learned that support placement matters more than I originally thought. Supports can leave marks on a part, so keeping them away from important fitting areas can save time during post-processing and help preserve the original dimensions.

I also learned that print orientation can affect the strength of a part. Since the hooks needed to bend, I had to consider how the layers were positioned and how the force would affect them during assembly.

### SLA vs FDM

One of the main differences I learned about is how the material affects the flexibility of the snap fit. SLA printing produces smooth and detailed parts, which is useful when two pieces need to fit together accurately. However, some SLA resins are stiffer and more likely to crack when bent too far. FDM printing can use different types of plastic, some of which are better suited for flexible parts. However, FDM prints usually have more visible layer lines, and the strength can change depending on the direction of the layers.

This project showed me that I cannot simply use the same snap fit design for every printing method. The shape and thickness of the hooks need to be designed around the material being used.

Although my snap fit worked well, there are still a few things I would improve if I were to make another version. The main improvement would be adding small guide walls inside the box to help line up the hooks with their openings. This would make the lid easier to attach and reduce the amount of adjusting needed during assembly. I would also consider testing slightly different hook dimensions and clearances to see if I could make the assembly process even smoother while keeping the lid secure.

### Time, Cost, & Resources

For this project, I used the FabLab's Form 4 printing equipment, PreForm for preparing the model, and CAD software to design both the lid and the box. The actual printing process took 1 hour and 35 minutes, with a total resin usage of 40.41 mL. After printing, I spent 5 minutes washing the parts and 15 minutes curing them. I also used wire cutters provided by the FabLab to remove the supports. 

Overall, this project took me bout 6 hours and it helped me understand how much planning goes into making a working snap fit. It was not just about designing two pieces that fit together. I am happy with the final result because the lid successfully snaps onto the box and stays in place. If I were to make another version, I would focus on improving the alignment of the hooks to make assembly easier.
