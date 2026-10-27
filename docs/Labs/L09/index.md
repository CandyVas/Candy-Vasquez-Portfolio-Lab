# A9 –  Laser Cutter

## Overview
The goal of this project was to design, laser cut, assemble, and document a parametric construction kit that accounts for material thickness, laser kerf, and joint clearance. The design process involved measuring the material, testing different slot sizes, and using the results to determine suitable dimensions for the final assembly.

## Measure Material & Kerf

The material thickness was measured with calipers at three locations. The recorded measurements were 0.105 in, 0.109 in, and 0.107 in. The mean thickness was calculated as:

+ Mean thickness = (0.105 + 0.109 + 0.107) / 3 = 0.107 in (or 2.72 mm)

<img width="300" height="240" alt="image" src="https://github.com/user-attachments/assets/bd3de602-7714-44b4-a0dd-983f389b6b77" />

Then to measure kerf, we made a 20 × 20 mm square was created in Solidworks which was trasnferred to Inkscape and cut using the laser cutter. The resulting square was measured with calipers in both the X and Y directions. The X-direction measurement was 19.70 mm (marked with the **red** dot), and the Y-direction measurement was 19.74 mm (marked with the **purple** dot).

<img width="300" height="240" alt="Screenshot 2026-10-22 174315" src="https://github.com/user-attachments/assets/3cdba93a-4288-43e6-8978-f5446a6a1092" />

<img width="300" height="240" alt="image" src="https://github.com/user-attachments/assets/a708196f-01e5-42d0-9663-0f920948aa38" />
<img width="240" height="240" alt="image" src="https://github.com/user-attachments/assets/12f28c30-89b3-468c-a726-276f92f91c87" />


The kerf was calculated by subtracting each measured dimension from the original 20 mm dimension:

X-direction kerf: 20.00 − 19.70 = 0.30 mm

Y-direction kerf: 20.00 − 19.74 = 0.26 mm

The average of the two measurements was 0.28 mm. The difference between the X and Y measurements shows that the measured kerf was not identical in both directions. 

## Coupon
A fit-test coupon was used to investigate how slot width affected the fit of the parts. The first coupon measured 40 × 40 mm and contained five slots with widths increasing in 0.10 mm increments, from 2.00 mm to 2.40 mm. None of these slots was large enough to accept the 20 × 20 mm square tab.

A second fit test was then conducted using a larger range of slot widths, approximately 2.40–2.80 mm. The 2.40 mm slot was difficult to assemble and required enough force that there was concern about bending or damaging the material. The 2.50 mm slot produced the best fit among the tested options, as everything afterword's was too loose. 

<img width="357" height="320" alt="Screenshot 2026-10-22 182132" src="https://github.com/user-attachments/assets/8b103742-7ebc-4765-959f-7e7ba2de6723" />
<img width="402" height="305" alt="Screenshot 2026-10-22 183452" src="https://github.com/user-attachments/assets/49377045-72bb-4b42-b9a2-034eb2fe71da" />

<img width="333" height="269" alt="image" src="https://github.com/user-attachments/assets/48effb03-4fb0-4c22-8bc5-512b97727481" />
<img width="325" height="243" alt="image" src="https://github.com/user-attachments/assets/f195753d-e9b2-4717-80bf-91a299984b8b" />


## Design
I started by creating a centerline. Since my design would be flat and assembled, I decided to create the sketches on the same top plane. I began with the first shape, a rectangle. I created a 30 mm rectangle centered on the centerline, then added a slit that extended halfway down the shape. I used a parametric design so that if I needed to make changes, I could update the dimensions through the Equation Manager instead of changing each dimension individually.

<img width="313" height="276" alt="Screenshot 2026-10-27 103544" src="https://github.com/user-attachments/assets/5158f813-1c5c-4c46-902c-492c2e24247e" />
<img width="250" height="304" alt="Screenshot 2026-10-27 103905" src="https://github.com/user-attachments/assets/9bfaa2e5-576a-47c4-9fc6-0630b79a4c12" />

I repeated these steps for the other two shapes, creating the circles and squares with similar slits so the pieces could fit together.

<img width="512" height="319" alt="image" src="https://github.com/user-attachments/assets/ca4d30e1-4b4d-4ddf-81a4-45b4846864cc" />

I then used the Trim Entities tool to adjust the sketch geometry and ensure the slot openings were properly defined before proceeding with the final design.

<img width="616" height="258" alt="image" src="https://github.com/user-attachments/assets/5cf19e49-fec4-4099-8356-7dc614b6c709" />

My final kit was three circles, three rectangles and three squares (a total of nine pieces) comprising three different part types. That was sufficient to meet the minimum requirements for both number of part types and total number of pieces. The slits enabled the individual pieces to be joined together and the kit could be assembled without any recourse to the original box design.

### Reparameterization 

Although my measured material thickness was approximately 2.72 mm, the fit-test coupon showed that a 2.50 mm slot width produced the best fit. Based on this physical test, I returned to the Equation Manager and changed the relevant dimension from 2.72 mm to 2.50 mm. This allowed me to update the design through its parameters rather than manually changing individual dimensions.

The fit test demonstrated that the measured material thickness did not necessarily correspond to the slot width that worked best in practice. Testing the physical parts helped me choose a dimension that produced a successful assembly.


<img width="663" height="254" alt="image" src="https://github.com/user-attachments/assets/7db51534-f258-4a04-b6ed-86addabc8bce" />
<img width="737" height="346" alt="image" src="https://github.com/user-attachments/assets/cdcff266-97ab-47b7-847f-720f242b4c13" />

So since the pieces have slits that allow them to slide together. I modeled the parts in SolidWorks and used a 2.50 mm slit width, which produced a successful fit in the final laser-cut assembly.

<img width="487" height="137" alt="image" src="https://github.com/user-attachments/assets/5a6fa3c5-ab96-47dd-bcf4-16a2c83df9a0" />

> parameters measured

<img width="490" height="146" alt="image" src="https://github.com/user-attachments/assets/c2511a47-b864-4fee-bb00-34d655191f5e" />

> altered parameters
<img width="314" height="244" alt="image" src="https://github.com/user-attachments/assets/b0f97ced-3ba2-41e7-bd43-dfd89d09058d" />
<img width="555" height="210" alt="image" src="https://github.com/user-attachments/assets/a8c744ae-c3b3-49ac-a9cc-4f1bbc550825" />

> transferred onto inkscape- settings applied to avoid blown-out look

<img width="200" height="240" alt="Screenshot 2026-10-22 191044" src="https://github.com/user-attachments/assets/e16edd80-2a6a-41c9-b757-e9b80b0e4169" />

## Manufacturing

Laser cutting uses a focused laser beam to cut material along a path defined by a digital design. The laser's heat removes material to create precise shapes and slots. Kerf must be considered because the laser removes a small amount of material along each cut.

Compared with FDM 3D printing, laser cutting can be faster for flat parts because multiple shapes can be arranged on one sheet and cut in one job. It also works well with sheet materials such as wood and acrylic. FDM printing builds objects layer by layer and is better suited for complex three-dimensional shapes, while laser cutting is useful for making flat parts that can be assembled into larger structures

I used the SFL LA-5 and LA-4 laser cutters, depending on which machine was available. The material was wood labeled as 1/8 inch thick. I used one 12 × 12 inch sheet, and the average measured thickness was 0.107 inches, or approximately 2.72 mm.

<img width="378" height="421" alt="image" src="https://github.com/user-attachments/assets/8f2bf389-2c2e-43ab-86dd-04c76a217464" />

For the final cut, I used a speed of 15%, power of 100%, frequency of 20%, and one cycle. Staff helped me focus the laser. Air assist was on during the laser cutting and it essentially serves to blow air towards the cut area to assist in the removal of smoke and particulates to reduce excessive burning and to improve the quality of the cut edge. The exhaust is there to take away the smoke, fumes and particulates generated during the cutting process. Under normal operating conditions the exhaust should be on throughout the cutting process. This was discussed during our orientation to help prevent any fires within the lab.

<img width="293" height="349" alt="image" src="https://github.com/user-attachments/assets/e0f0b67c-d722-4116-be15-ba0c567ee2b6" />

I arranged the three circles, three rectangles, and three squares within the available 12 × 12 inch sheet. Using one sheet allowed me to manufacture all nine pieces without needing additional material. I also changed my original box design to a simpler construction kit to meet the assignment requirements without overcomplicating the design.

<img width="930" height="439" alt="Screenshot 2026-10-22 191632" src="https://github.com/user-attachments/assets/3e30a0b5-7b4a-4437-996d-095621dce2e8" />

Here is a video of my [laser cuts](https://github.com/user-attachments/assets/c6dc6cf2-7f36-4c04-b627-db16a3b1e4b5)
Here is my [solidworks file](https://drive.google.com/file/d/1yvh0M3q4Oj6adgm9EunJYRLMb69mpE6b/view?usp=sharing) 

The finished wooden components did have some burn marks/soot along the edges. The burn marks could have been due to the heat of the laser, the cutting settings or the wood itself. This would explain why even though each part was designed with the same 2.50 mm slit, some are looser or tighter than others. 

<img width="215" height="377" alt="image" src="https://github.com/user-attachments/assets/a568a34f-7df3-4d5a-a630-8ffdb0709740" />
<img width="270" height="421" alt="image" src="https://github.com/user-attachments/assets/841983a1-364b-4f6d-b914-99542ca0abcf" />

<img width="434" height="349" alt="image" src="https://github.com/user-attachments/assets/62481b6f-bce5-4f6c-aa19-7d224520fced" />
<img width="347" height="213" alt="image" src="https://github.com/user-attachments/assets/57923f0a-7553-45f9-96fb-63cbdf5462bf" />

## Lessons Learned

The project involved orientation, training, measuring the material, creating kerf and fit-test coupons, designing the final kit in SolidWorks, cutting the parts, assembling the finished design, and writing this report. It took me approximately 9 hours to complete this assignment. 

### Mistakes
My original design for the construction kit was a box. As I went through the design process though we realized that the box only had six parts in it which didn't meet the requirement of at least eight parts. I considered modifying the box to add the additional parts, but I was concerned that doing so would complicate the design too much.

I also had to consider the limited amount of material we had. If the design was unsuccessful, it would require additional test cuts and another sheet of material which would have meant going through the kerf measurement process all over again.

<img width="477" height="199" alt="Screenshot 2026-10-22 165717" src="https://github.com/user-attachments/assets/c812afe9-cc42-4ebf-9e24-28dcb32d7dc2" />

> Rejected Box design

 <img width="593" height="194" alt="image" src="https://github.com/user-attachments/assets/d4e9c69d-668a-4416-b16a-6c232e8fb525" />

> conceptualizing the extra 2 pieces

Rather than risk wasting material or end up with a design that was far too complex, I decided to go the other way and produce a construction kit of circles, rectangles and squares with slits in them which could be joined up to make the design.

Another mistake was the first fit-test coupon had slot widths ranging from 2.00 mm to 2.40 mm, but none fit the test piece. I created a second coupon with larger slot widths and found that 2.50 mm provided the best fit. I used this dimension in my final CAD model, and the parts assembled successfully. The final cut had some burn marks or soot. If I repeated the process, I would verify the kerf measurements, document the air-assist and exhaust conditions, and improve the parametric model so that slot dimensions could be changed through a shared variable.

### Recourses 
I used one 12 × 12 inch sheet of wood with a nominal thickness of 1/8 inch. I used SolidWorks to design the parts, Inkscape to create the kerf coupon, calipers to measure the material and test pieces, and the SFL LA-5 and LA-4 laser cutters to manufacture the kit. I used the program Epilog Dashboard to prepare my design to be laser cut.

### Reflection

i. The wood was labeled as 1/8 inch thick, but my measured average was only 0.107 inches. This showed why measuring the actual material is important instead of relying on its nominal thickness. Using the assumed thickness could have resulted in joints that were too tight or too loose. The kerf coupon also showed that the laser removes material during cutting. Measuring the kerf and testing different slot widths helped me choose a 2.50 mm slot width that worked in the final assembly.

ii. Taguchi's quality loss function explains that quality decreases when a result differs from its target, even if the part still functions. In my fit tests, the 2.40 mm slot was too tight, while everything beyond 2.60 mm was loose. The 2.50 mm slot provided the best fit. If thousands of these parts were manufactured, overly tight joints could increase assembly time or cause damage, while loose joints could create unstable assemblies. Both problems could increase waste, rework, and production costs.

iii. Flat-pack furniture is an example of a product that can use interlocking sheet parts and tab-and-slot connections. If the material thickness or kerf were incorrect, the joints might be too tight to assemble or too loose to hold securely. Customers could experience difficult assembly, unstable furniture, or just overall poorly aligned parts.

iv. If I had one more cut, I would verify the kerf measurements and do additional fit tests before manufacturing the final kit. I would also improve my SolidWorks model by using a global variable to control the slot widths instead of entering each dimension manually. This would make the design easier to update and help maintain consistent fits if the material or design changed.

## Appendix
1 sheet of 3mm thick wood board

LA-4 and LA-5 laser cutters

InkScape Program 

Solidworks Program 

Epilog Dashboard Program

[SolidWorks model to Inkscape to laser cutting](https://www.youtube.com/watch?v=ptxyHT09A2M)

[Xometry](https://www.xometry.com/resources/3d-printing/3d-printing-vs-laser-cutting/)
