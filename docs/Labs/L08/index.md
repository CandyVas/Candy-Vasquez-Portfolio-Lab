# L8 – Design Something Useful

## Objective
> For this week you get to design something useful to you or someone else. Thinking of and solving a problem is an extremely useful skill as a mechanical engineering. 

## Great Questions... 

Asking smart questions matter because it helps designers look beyond the obvious and truly understand a problem before trying to solve it. Instead of making assumptions, asking questions allows them to discover details they might have missed and help figure out what actually needs to be fixed. This is especially important when is comes to design because an idea might sound great at first but still have weaknesses when put into action. SO by asking questions, designers can catch these issues early and come up with better solutions. 


## Problem Statement
**State the purpose of your design. What problem are you trying to solve? (make sure do list your research)
How did you notice the problem
Who are you designing the product for? Who is your ideal user?
What is your approach to your design?**

The purpose of my design is to create a headphone stand for my headphones. I noticed this problem because, after using my headphones, I would simply leave them lying on my desk. This is not ideal because it contributes to desk clutter. I like to keep things tidy, and my desk is already relatively small because I want to avoid taking up too much space in my room. Therefore, I wanted to create a solution that would keep my headphones organized without taking up too much desk space.

I am designing this product primarily for myself. However, after looking online, I found that many products already exist to solve this exact problem. A headphone stand is ideal for people who regularly use headphones while sitting at a desk, like gamers, people attending office meetings, or those making phone calls from home. On the other hand, someone who mainly listens to music on the move or use them when commuting more from a headphone case than a stand.

Before deciding on my final design, I wanted to research existing headphone stands and understand what makes a good design. I looked at popular designs on both Amazon and Printables. One design that caught my attention was the Omega-shaped stand, which was particularly tempting as someone pursuing engineering. However, after doing further research, I found an [article](https://headphones.com/blogs/features/the-most-popular-headphone-stand-might-be-ruining-your-headphones-why-pads-matter) explaining how certain headphone stands could potentially damage headphones over time. Some large Omega-style stands can place continuous pressure on the ear cushions. Over time, this pressure may flatten the padding and potentially affect the headphones' fit. This made me reconsider my initial design idea because I wanted to create a stand that would organize my headphones without potentially damaging them.

Another potentially harmful headphone case design is one that has __. After looking more into different designs, this [website](https://www.moon-audio.com/blogs/expert-advice/stands-storage-cases-traveling-portable-audio-gear) highlights how a small hook can concentrate the headphones' weight on one small area of the headband, potentially causing dents or stretching the padding over time. A wider, curved support distributes the weight more evenly and helps reduce pressure on a single point.

Overall, these sources helped me develop a better understanding of what makes a suitable headphone stand. Rather than focusing only on its appearance, I wanted to create a design that would solve my original problem while also considering the headphones long term condition.

## Design 
**If you create a sketch, create a pdf and include it in the portfolio.
Take many pictures of the different stages of the CAD model.
Detail decision making along the way
Detail how you determined the engineered allowances of the interactive parts**

Using my research, I decided to design a stand that supports the headband across a wider area rather than using a small hook that concentrates the weight in one spot. This should help minimize pressure on the headband and keep the ear cushions from resting against the desk or other surfaces.

I decided on a design similar to the one shown in my sketch below.

*add sketch* 

At the top of the stand, I designed a wide saddle to support the headband. I wanted the saddle to have a smooth, curved surface that follows the shape of the headphones and distributes their weight more evenly.

Another important consideration was leaving enough clearance for the ear cups so they would not press against the stand or the desk. I also wanted a wide, stable base to reduce the possibility of the stand tipping over when removing or placing the headphones.

### Measuring the Headphones

Before creating my CAD model, I needed to determine the dimensions of my headphones. Sadly HyperX has not published an exact numerical measurement for the width or height of the headband padding on the HyperX Cloud III Wired Gaming Headset. I initially measured the headphones myself. This was somewhat difficult because the headband is curved and the padding is flexible rather than rigid. Based on my measurements, I estimated the following dimensions:

+ Headphone height: Approximately 19.5 cm (195 mm or 7.68 inches).
+ Headband width: Approximately 4.1 cm (41 mm or 1.61 inches).

These measurements gave me a starting point for designing the stand. However, I wanted to verify the dimensions before continuing. After looking further online, I found a listing on Sam's Club that included the headphones specifications. This was helpful in checking my measurements and determining the dimensions to design my stand. 

<img width="392" height="230" alt="image" src="https://github.com/user-attachments/assets/31407156-338f-4b6c-9073-8847ca63ad2f" />
> [Link](https://www.samsclub.com/ip/HyperX-Cloud-III-Wired-Gaming-Headset-PC-PS5-Xbox-Series-X-S-Angled-53mm-Drivers-DTS-Memory-Foam-Durable-Frame-Ultra-Clear-10mm-Mic-USB-C-USB-A-3-5mm/20278224795?classType=REGULAR&from=/search) for the headphones and its specifications. 

### CAD Model 

Since the stand was a relatively large piece, I decided to design it as separate components rather than printing the entire model as one piece. I remembered that, in a previous assignment, printing a rod upright greatly increased the printing time. I wanted to avoid a similar issue with this design and make the parts easier to print.

<img width="522" height="334" alt="image" src="https://github.com/user-attachments/assets/253a2b57-4f81-47b5-811d-b4165171f83c" />
<img width="321" height="175" alt="image" src="https://github.com/user-attachments/assets/c1e213ec-08a5-4818-bfe4-9510257415b4" />

For the stem, I aligned it with the center of the base. This helped distribute the load more evenly and kept the design symmetrical. Centering the stem also helped maintain the stand's balance when the headphones were placed on it.

<img width="271" height="257" alt="image" src="https://github.com/user-attachments/assets/0029248c-0fa7-4d7a-ab45-486ca1543497" />
<img width="338" height="320" alt="image" src="https://github.com/user-attachments/assets/5d3f1587-256f-4201-a006-bc350346ebf3" />


<img width="571" height="286" alt="image" src="https://github.com/user-attachments/assets/50c9e673-35cd-45c3-a56c-bbdef01fb273" />
<img width="351" height="206" alt="image" src="https://github.com/user-attachments/assets/edfb655a-9593-46ce-bae4-5618e9d28f4e" />

As I continued modeling, I made adjustments to ensure the overall dimensions were appropriate. I had initially made the arch a total height of 250 mm, rather than adding its height on top of the 250 mm dimension. To keep the final design within my intended height, I went back to the extrusion feature and reduced it to 240 mm so that the arch would not extend beyond the top of the intended design.

I also wanted to reduce the amount of material in the large block that formed the saddle. To achieve this, I used the Extruded Cut feature in SOLIDWORKS to remove unnecessary material and refine the shape. This helped make the design less bulky while retaining the support needed for the headband.

<img width="379" height="196" alt="image" src="https://github.com/user-attachments/assets/3c023bbe-0cc8-4994-95d9-fa1f9b2d4a13" />

After making these adjustments and adding the finishing touches, I had a more complete version of my headphone stand.

<img width="225" height="341" alt="image" src="https://github.com/user-attachments/assets/f9737bde-536d-4265-9814-6cf4b3dbd435" />
<img width="344" height="266" alt="Screenshot 2026-10-19 184111" src="https://github.com/user-attachments/assets/0c306b4f-b8a4-484c-b173-761f58b9f9b3" />

### Separation and clearance

Once I was happy with the overall design, I separated the components and considered how they would fit together after 3D printing. I wanted to avoid printing the entire stand upright as one piece because this could increase printing time and potentially affect the strength of certain features. Separating the parts also made the model more practical to print and assemble.

For the connecting feature, I used a clearance of approximately 0.15 mm per side. This resulted in a total dimensional increase of 0.30 mm in both the length and width of the receiving hole compared with the corresponding male component.

For example, if the male component measured 30.00 mm × 15.00 mm, the receiving hole would measure 30.30 mm × 15.30 mm. This was my intended starting point for achieving a snug fit while allowing the parts to slide together after printing.

<img width="383" height="334" alt="image" src="https://github.com/user-attachments/assets/4cd5f83f-a1e0-4b87-a989-f17827ee6911" />


## 3D Print 
**What number machine did you use?
Did you use a raft? If so, what were the settings?
What was the wall thickness?
What infill did you use and why?
Did you use supports? Why or why not? If you did, explain the technical process you used to support the print.
What did you use to remove the supports?
How many layers are used in the print?
What is the layer thickness?
What is the build volume of your print?
Comment on the surface finish of the supports
Outline reasons for the layout.
Outline reasons for build orientation.
Outline slicer settings and reasons for the settings.
Note the slice information on Prusa Slicer**

After completing my CAD model, I imported the parts into PrusaSlicer to prepare them for 3D printing. 

As I arranged the parts, I had a terrifying realization that my model was huge- some parts extended beyond the build plate, meaning they would not fit in their original orientation.

<img width="530" height="397" alt="image" src="https://github.com/user-attachments/assets/edeb388d-eda4-4bce-a3ea-8e34995ecf99" />

One option was to print the parts upright, but this would increase printing time and potentially make them weaker due to the direction of the layer lines. Instead, I rotated and repositioned the parts to fit the build plate. I purposefully avoided vertical orientations and orientations that would require unnecessary supports to reduce printing time and material waste.

<img width="428" height="317" alt="image" src="https://github.com/user-attachments/assets/e8cdf978-b8d8-4e9f-9f54-3a02c1044260" />

Finally with everything fit snug on the build plate, this is what I ended with.  
<img width="413" height="320" alt="image" src="https://github.com/user-attachments/assets/476d0466-623f-4ac2-a372-e2a0228273b6" />

### Infill and Print Settings

Initially, I considered using 20% infill with a gyroid pattern because it provides internal support in multiple directions. However, after slicing the model and checking the estimated printing time, I realized I was already on a time crunch and would not be able to complete the print in time with those settings. I therefore had to make a sacrifice and settle for the default 15% infill with a grid pattern. Although this reduced the amount of internal material, it was a reasonable compromise between strength, material usage, and printing time. However something that both have in common is that I chose three perimeters,(which is one more than the default) and i kept the default layer height of 0.20 mm to keep a good balance between print quality and printing time. 

<img width="309" height="119" alt="image" src="https://github.com/user-attachments/assets/100520c7-3d3c-404e-a5c5-39578b298b24" />

> Gyroid pattern, 20% infill

<img width="314" height="149" alt="image" src="https://github.com/user-attachments/assets/591602c2-07b3-47d8-8a8f-f3d84c82b52b" />

> Grid pattern, 15% infill

I also aimed to minimize supports by choosing suitable print orientations. Avoiding unnecessary supports would save time and reduce the marks left on the finished surface. I planned to print the parts directly on the build plate without a raft since they have enough contact for adhesion. It's one of the reasons why I decided on a rectangular design for the stand and saddly rather than something circular, a design which I've seen a lot when browsing online.

After finalizing the settings, I sliced the model in PrusaSlicer and got a total of contained 225 layers. I used the slicing preview to check the part layout, infill, and overall print preparation before sending the model to the printer.

<img width="269" height="255" alt="image" src="https://github.com/user-attachments/assets/b7924045-3a4c-4d9e-a171-fe6978ebac81" />
> PrusaSlcer Legend 

<img width="634" height="473" alt="image" src="https://github.com/user-attachments/assets/42a9a8f5-700a-4b12-a20e-50270b722d98" />
> 225 layers 

The final settings were a compromise between the ideal design and the time available. This process taught me that preparing a model for 3D printing involves more than simply creating a CAD design. The orientation, infill, supports, and available printing time all affect how practical the final print will be.


## Lessons Learned
**Detailed lessoned learned throughout the process, the more detail the better which includes detailing any mistakes throughout the process.
Actual time it took from start to finish and resources.**

## Appendix 
[Toptal](https://www.toptal.com/designers/product-design/design-thinking-great-questions)


