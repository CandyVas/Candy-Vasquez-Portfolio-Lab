# A10 – RC2 Sliding Fit Design

Design and fabricate a pair of parts (a hole/slot feature and a matching shaft/insert feature) that demonstrate an RC 2 sliding fit on a SLA print as defined in the Machinery’s Handbook:

> “RC 2 Sliding fits are intended for accurate location, but with greater maximum clearance than class RC 1. Parts made to this fit move and turn easily but are not intended to run freely, and in the larger sizes may seize with small temperature changes.”


## Research and Planning

<img width="75" height="374" alt="image" src="https://github.com/user-attachments/assets/2835a769-0123-4108-830e-d8732b738ee8" />
<img width="145" height="368" alt="image" src="https://github.com/user-attachments/assets/e3017963-a733-4778-a3ba-152d11f95024" />

The purpose of this project is to design and manufacture two components that demonstrate an RC 2 sliding fit. I researched the RC 2 running and sliding fit specification in Machinery's Handbook. An RC 2 fit is designed for components that need to slide relative to one another while maintaining accurate positioning. It provides a small clearance between two mating surfaces, allowing one component to move without requiring excessive force. Compared to a loose fit, an RC 2 fit allows less unwanted movement while still providing enough clearance for smooth operation.

Although I chose to design and manufacture my components using millimetres, the RC 2 tolerance table in Machinery's Handbook uses inches for its nominal sizes and tolerance values. Therefore, I first had to convert my original dimensions into inches to find the correct sections of the table.

<img width="222" height="141" alt="image" src="https://github.com/user-attachments/assets/bbb13484-7e1b-4a9e-a5a4-be39e1cd4f28" />

For my first sketch, I was simply trying to get an idea down, so I increased the size of my sliding component by 0.4 mm to make it fit. However, after reviewing the tolerance table, I realised I needed to consider the actual clearance allowed by the RC 2 fit. I identified the correct nominal size ranges, calculated the minimum and maximum clearances, and used these values in my revised sketch. Since the hole dimensions had a tolerance of zero, I left them unchanged and applied the RC 2 adjustments to the sliding component.

To apply the RC 2 fit, I converted my selected nominal dimensions into inches and identified their corresponding size ranges in Machinery's Handbook. I then calculated the minimum and maximum clearances and used these values to adjust the dimensions of the sliding component in CAD.

For my design, I chose to create a sliding locking mechanism inspired by the lock on my own back glass door. The mechanism consists of a smaller trapezoidal insert that slides into a larger trapezoidal housing. I chose this shape because the angled sides help prevent the insert from slipping or lifting out while still allowing it to slide in a straight line.

Another factor I had to consider was resin shrinkage. Resin printing does not always produce the exact dimensions shown in CAD, and post-curing can cause slight dimensional changes. This was especially important for my design because the RC 2 fit has a very small clearance. Even a small change in dimensions could make the sliding component too tight or too loose.

## 2. CAD Design

<img width="499" height="182" alt="image" src="https://github.com/user-attachments/assets/315a1e7e-7f66-4f27-81c5-68632a6a62b8" />

I transferred my hand sketch into SolidWorks and created parametric models of both components. This allowed me to control the dimensions and make changes to the design more easily. 

Throughout the CAD process, I used dimensions and geometric constraints to keep the two components consistent. The most important dimensions were the internal width of the housing and the external width of the sliding insert, as these controlled how the two parts fitted together.

Part A: Hole or slot feature

<img width="265" height="262" alt="Screenshot 2026-10-29 013409" src="https://github.com/user-attachments/assets/62b6e53f-53c0-4fb4-814a-5928c33fac04" />
<img width="527" height="311" alt="Screenshot 2026-10-29 013445" src="https://github.com/user-attachments/assets/9653bf06-8bd5-45fa-a578-4670ab9803a5" />


Part B: Shaft or insert feature

<img width="263" height="272" alt="Screenshot 2026-10-29 012628" src="https://github.com/user-attachments/assets/1151da7c-aad4-4002-9513-9a50e0148b33" />
<img width="694" height="326" alt="Screenshot 2026-10-29 012802" src="https://github.com/user-attachments/assets/d085fc51-675f-4c55-909f-c9685cc08725" />
<img width="228" height="238" alt="Screenshot 2026-10-29 013003" src="https://github.com/user-attachments/assets/36173d94-3b99-4190-8599-fbbf375d459c" />

Here, the two components are assembled in SolidWorks. I also used the interference detection tool to check for overlapping geometry and confirm that there were no unwanted interferences between the parts.

<img width="479" height="377" alt="Screenshot 2026-10-29 170329" src="https://github.com/user-attachments/assets/9b2a269c-416e-45d6-80a8-57c3dee23438" />

> Interference Detection

<img width="276" height="292" alt="image" src="https://github.com/user-attachments/assets/58da6960-5d88-45e0-b9ee-695f058ff9d0" />

## 3. Preprocessing for 3D Printing 

After completing the CAD models, I imported both components into PreForm to prepare them for resin 3D printing.

I connected to the Niner Net guest Wi-Fi and accessed the available resin printers in the Super Fab Lab. I selected the printer named HiddenCod, which was a Formlabs Form 3, and used the available print settings.

<img width="401" height="200" alt="Screenshot 2026-11-03 100208" src="https://github.com/user-attachments/assets/739b1a6a-7232-4366-8cb6-e462f6f28cc7" />


<img width="316" height="218" alt="Screenshot 2026-11-03 100215" src="https://github.com/user-attachments/assets/46dd6d68-1c73-41a8-b1e0-20e1eb97e785" />

These were the initial results after importing both components into PreForm.

<img width="191" height="219" alt="image" src="https://github.com/user-attachments/assets/38a02b79-2527-4e41-9ec8-4c0c724f3805" />

<img width="220" height="205" alt="image" src="https://github.com/user-attachments/assets/cbe9874f-5ca0-4716-8db3-744e6d274612" />

One of the main things I considered during this stage was the orientation of the components on the build plate. Unlike FDM printing, resin printing requires support structures to hold the parts in place during printing. Because my design relies on two surfaces sliding against one another, I wanted to avoid placing supports directly on these areas. Removing supports from the sliding surfaces could leave marks or rough spots, which would increase friction and affect the fit.

I used PreForm's One-Click feature to help position the supports. I then reviewed the suggested orientation and made sure the supports were kept away from the main sliding surfaces as much as possible.

<img width="222" height="255" alt="image" src="https://github.com/user-attachments/assets/c9c7034c-4c11-4ff8-b556-5ff9153c64f2" />

<img width="124" height="118" alt="Screenshot 2026-10-29 183126" src="https://github.com/user-attachments/assets/fef6274f-8912-48f0-8fc5-6ffa3c4da36e" />

<img width="126" height="115" alt="Screenshot 2026-10-29 182938" src="https://github.com/user-attachments/assets/ac95f574-79f3-4ccb-ba4f-9ba8509789f5" />

The final printing settings were:


<img width="202" height="386" alt="Screenshot 2026-10-29 182414" src="https://github.com/user-attachments/assets/f6db5b65-5221-44ba-b2af-3a3265f1274e" />

<img width="218" height="404" alt="Screenshot 2026-10-29 183116" src="https://github.com/user-attachments/assets/ba52cf80-1e10-48e0-84ec-79457ccadb15" />


## 4. Post-Processing 

This is what it looked like after printing. I needed to remove the support structures from both components. This needed to be done carefully because the parts contained small features and precise sliding surfaces.

<img width="300" height="241" alt="image" src="https://github.com/user-attachments/assets/12610ccb-9627-44f3-ad14-ba7707c33192" />

<img width="300" height="206" alt="image" src="https://github.com/user-attachments/assets/8c006ac7-c3b9-4cf7-835d-84ee3fc4b357" />

<img width="200" height="206" alt="image" src="https://github.com/user-attachments/assets/de577633-a1cd-4c78-ac30-e45f662be206" />

I paid particular attention to the areas around the sliding surfaces because removing supports too roughly could damage the geometry and affect the final fit.

<img width="342" height="271" alt="image" src="https://github.com/user-attachments/assets/b7f0d302-cded-4056-835f-7dec27c2467b" />
<img width="275" height="214" alt="image" src="https://github.com/user-attachments/assets/6926b069-5449-44ee-83fe-658bd42bfdae" />

Following support removal, the components were washed to remove uncured resin remaining on their surfaces.

### Washing

After removing the supports, I washed the components to remove any uncured resin left on their surfaces. This stage took around 10 minutes.

<img width="292" height="319" alt="image" src="https://github.com/user-attachments/assets/32b5d95a-0c68-4308-b20e-f7147949bacb" />
<img width="468" height="359" alt="image" src="https://github.com/user-attachments/assets/305a5db9-fd96-4f90-b2d4-731c091fd9bc" />

### Curing 

Following washing, I cured the components for 15 minutes to complete the resin curing process.

Post-curing helps harden the resin, but it can also cause slight shrinkage as the material continues to cure. This was important to consider because even small dimensional changes could affect the clearance between my two components.

<img width="300" height="201" alt="image" src="https://github.com/user-attachments/assets/89930200-a1c9-43dc-9980-04f7d8928f3d" />

<img width="300" height="206" alt="image" src="https://github.com/user-attachments/assets/4b0e2ca3-a340-4d0d-b3f4-4f3feecb7d69" />

After washing and curing, I sanded the components to improve their surface finish and remove imperfections.

However, sanding ended up affecting the final fit. The two components initially fitted together and were able to slide, but after sanding, the mechanism became too loose. I believe I removed too much material from the mating surfaces, increasing the clearance between the parts.

This showed me that sanding precision components requires more care than sanding a regular 3D print. Even removing a small amount of material can affect how well the parts fit together.

## 5. Fit Test (20%)

After printing and post-processing, I used digital calipers to measure the finished components and compare them with my original CAD dimensions.

Some of the internal features were difficult to measure because the calipers could not reach certain recessed areas and grooves. Because of this, some of my measurements were estimates rather than exact readings.

The measurements I recorded were:

<img width="275" height="273" alt="image" src="https://github.com/user-attachments/assets/a88ba805-f6e8-463f-9176-661ce7447bf8" />
<img width="274" height="323" alt="image" src="https://github.com/user-attachments/assets/e2a05ba5-65a8-4bf1-87d3-ebe30dcc4359" />
<img width="284" height="296" alt="image" src="https://github.com/user-attachments/assets/48428583-0ed6-434a-be54-1caf61ea0cb5" />
<img width="290" height="274" alt="image" src="https://github.com/user-attachments/assets/5264cfcb-fc21-4714-a1eb-e3165d43e10b" />
<img width="305" height="305" alt="image" src="https://github.com/user-attachments/assets/63e1f39c-1fba-4b6f-b024-f17f3f647b1e" />
<img width="311" height="280" alt="image" src="https://github.com/user-attachments/assets/c0783283-5422-48c3-bbc9-4e17b9623294" />

Some of these measurements were difficult to obtain because the digital calipers could not reach certain internal surfaces, particularly within the recessed sections of the housing. I had to estimate some dimensions based on the accessible areas.

### Physical Fit

During the initial assembly, the two components fitted together and could slide along the housing. However, after sanding, I noticed that the mechanism had become too loose. I believe this was caused by removing too much material from the sliding surfaces, which increased the clearance between the parts.

Another issue I noticed was the handle on the sliding insert. During testing, the insert could slide into the housing until it reached the handle, where its movement stopped.

<img width="245" height="277" alt="image" src="https://github.com/user-attachments/assets/52f166e5-2ce1-43d4-9db9-2f9da00497c6" />

<img width="199" height="224" alt="image" src="https://github.com/user-attachments/assets/b77b6bf1-d4e1-4fdb-8d4b-c7953f438189" />

This showed me that I needed to consider the entire assembly, not just the sliding surfaces. The handle also needed to be positioned carefully so that it would not interfere with the movement of the mechanism.

Overall, the parts could slide together, but the final fit was looser than I wanted. Therefore, the finished mechanism did not fully achieve the accuracy expected from an RC 2 fit.

## 6. Lessons Learned (10%)

One of the biggest challenges I faced was understanding how to apply the RC 2 tolerance specification to my design. At first, I focused more on the overall shape than the relationship between the two parts. After researching Machinery's Handbook, I realised how important it was to calculate the clearance before finalising my CAD model. Converting my measurements from millimetres to inches also took some extra time because the tolerance table used imperial units.

The biggest lesson I learned came from sanding. The parts initially fitted together, but after sanding, they became too loose. I believe I removed too much material from the sliding surfaces. This taught me that even a small amount of sanding can affect the fit of precision components. In the future, I would sand more carefully and test the fit regularly instead of removing too much material at once.

Another challenge was measuring the finished parts. Some of the internal grooves were difficult to reach with my digital calipers, so I had to estimate certain measurements. Next time, I would use better tools for measuring internal features or make sure the design has areas that are easier to measure.

If I were to repeat this project, I would research the tolerances before starting my CAD model to avoid having to make major changes later. I would also print a small test piece with different clearances to see how accurately the resin printer produces the dimensions. Most importantly, I would be more careful during sanding and check the fit throughout the post-processing stage.

Overall, this project helped me understand that designing a good fit involves more than just getting the dimensions right in CAD. Printing, curing, sanding and measuring all affect the final result. Although my final parts were too loose, the project helped me understand how small changes during manufacturing can affect the performance of a mechanism.

### APpendix 

Machinery's Handbook – RC 2 running and sliding fit tolerance tables.

Solidworks – Design and modelling of the two components.

PreForm – Resin printing preparation and slicing.

Resin 3D printer – Physical production of the components.
