# L8 – Design Something Useful

## Objective
> For this week you get to design something useful to you or someone else. Thinking of and solving a problem is an extremely useful skill as a mechanical engineering. 

## Great Questions... 

Asking smart questions matter because it helps designers look beyond the obvious and truly understand a problem before trying to solve it. Instead of making assumptions, asking questions allows them to discover details they might have missed and help figure out what actually needs to be fixed. This is especially important when is comes to design because an idea might sound great at first but still have weaknesses when put into action. SO by asking questions, designers can catch these issues early and come up with better solutions. 


## Problem Statement

The purpose of my design is to create a headphone stand for my headphones. I noticed this problem because after using my headphones I would simply leave them lying on my desk. This is not ideal because it contributes to a cluttered desk, and as someone who likes to keep things tidy, I wanted to create something that would fix this. My desk is already relatively small so creating this would keep my headphones organized without taking up too much desk space.

I am designing this product primarily for myself. However, after looking online, I found that many products already exist to solve this exact problem. A headphone stand is ideal for people who regularly use headphones while sitting at a desk, like gamers, people attending office meetings, or those making phone calls from home. On the other hand, someone who mainly listens to music on the move or use them while commuting might benefit more from a headphone case rather than a stand.

I wanted to research existing headphone stands to understand what makes a good design. I looked at popular designs on both Amazon and Printables. One design that caught my attention was the Omega-shaped stand which was particularly tempting as someone pursuing engineering. However, after doing further research, I found an [article](https://headphones.com/blogs/features/the-most-popular-headphone-stand-might-be-ruining-your-headphones-why-pads-matter) explaining how this particular shaped headphone stand could damage headphones over time. That's because can place continuous pressure on the ear cushions and over time flatten the padding and potentially affect the headphones fit. This made me reconsider my initial design idea because I wanted to create a stand that would organize my headphones without damaging them.

Another potentially harmful headphone stand design is one that has a small area for holding. After looking more into different designs, this [website](https://www.moon-audio.com/blogs/expert-advice/stands-storage-cases-traveling-portable-audio-gear) highlights how a small hook can concentrate the headphones weight on one small area of the headband, potentially causing dents or stretching the padding over time. Wheras a wider, curved support distributes the weight more evenly and helps reduce pressure on a single point.

Overall, these sources helped me develop a better understanding of what makes a suitable headphone stand. Rather than focusing only on its appearance, I wanted to create a design that would solve my original problem while also considering the headphones long term condition.

## Design 

Using my research, I decided to design a stand that supports the headband across a wider area rather than using a small hook that concentrates the weight in one spot. This should help minimize pressure on the headband and keep the ear cushions from resting against the desk or other surfaces.

I decided on a design similar to the one shown in my sketch below.

<img width="370" height="200" alt="IMG_2515" src="https://github.com/user-attachments/assets/310b47bf-d223-43e6-b074-42e334f88946" />


At the top of the stand, I designed a wide saddle to support the headband. I wanted the saddle to have a smooth, curved surface that follows the shape of the headphones to distribute the weight more evenly.

Another important consideration was leaving enough clearance for the ear cups so they would not press against the stand or the desk. I also wanted a wide, stable base to avoid the stand tipping over when removing or placing the headphones.

### Measuring the Headphones

Before creating my CAD model, I needed to determine the dimensions of my headphones. Sadly, HyperX has not published an exact measurement for the width or height of the headband padding on the HyperX Cloud III Headset. SO i decided to measure the headphones myself, but this was somewhat difficult because the headband is curved and the padding is flexible rather than rigid. Based on my measurements, I estimated the following dimensions:

+ Headphone height: Approximately 19.5 cm (195 mm or 7.68 inches).
+ Headband width: Approximately 4.1 cm (41 mm or 1.61 inches).

These measurements gave me a starting point for designing the stand. However, I wanted to verify the dimensions before continuing. After looking further online, I found a listing on Sam's Club that included the headphones specifications. This was helpful in checking my measurements and determining the dimensions to design my stand. 

<img width="392" height="230" alt="image" src="https://github.com/user-attachments/assets/31407156-338f-4b6c-9073-8847ca63ad2f" />

> [Link](https://www.samsclub.com/ip/HyperX-Cloud-III-Wired-Gaming-Headset-PC-PS5-Xbox-Series-X-S-Angled-53mm-Drivers-DTS-Memory-Foam-Durable-Frame-Ultra-Clear-10mm-Mic-USB-C-USB-A-3-5mm/20278224795?classType=REGULAR&from=/search) for the headphones and its specifications. 

### CAD Model 

Since the stand was a large piece, I decided to design it as separate components rather than printing the entire model as one piece. I remembered that, in a previous assignment, printing a rod upright greatly increased the printing time. I wanted to avoid a similar issue with this design and make the parts easier to print.

<img width="522" height="334" alt="image" src="https://github.com/user-attachments/assets/253a2b57-4f81-47b5-811d-b4165171f83c" />
<img width="321" height="175" alt="image" src="https://github.com/user-attachments/assets/c1e213ec-08a5-4818-bfe4-9510257415b4" />

For the stem, I aligned it with the center of the base. This helped distribute the load more evenly and kept the design symmetrical. Centering the stem also helped maintain the stand's balance when the headphones were placed on it.

<img width="271" height="257" alt="image" src="https://github.com/user-attachments/assets/0029248c-0fa7-4d7a-ab45-486ca1543497" />
<img width="358" height="310" alt="image" src="https://github.com/user-attachments/assets/5d3f1587-256f-4201-a006-bc350346ebf3" />

<img width="351" height="206" alt="image" src="https://github.com/user-attachments/assets/50c9e673-35cd-45c3-a56c-bbdef01fb273" />
<img width="351" height="206" alt="image" src="https://github.com/user-attachments/assets/edfb655a-9593-46ce-bae4-5618e9d28f4e" />

As I continued modeling, I made adjustments to ensure the overall dimensions were appropriate and accurate to what i had pre-planned. I wanted to keep the height a total of 250 mm so I avoided than adding the arch **on top** of the 250 mm stem. I went back to the extrusion feature and reduced it to 240 mm so that the arch would not extend beyond the top of the intended design.

I also wanted to reduce the amount of material in the large block that formed the saddle. To achieve this, I used the Extruded Cut feature in Solidworks to remove unnecessary material. 

<img width="379" height="196" alt="image" src="https://github.com/user-attachments/assets/3c023bbe-0cc8-4994-95d9-fa1f9b2d4a13" />
<img width="225" height="341" alt="image" src="https://github.com/user-attachments/assets/f9737bde-536d-4265-9814-6cf4b3dbd435" />

### Separation and clearances

Once I was happy with the overall design, I separated the components and considered how they would fit together after 3D printing. I wanted to avoid printing the entire stand upright as one piece because this could increase printing time and potentially affect the strength of certain features. Separating the parts also made the model more practical to print and assemble.

For the connecting feature, I used a clearance of 0.15 mm per side. This resulted in a total dimensional increase of 0.30 mm in both the length and width of the receiving hole. I decided on this to achieve a snug fit while allowing the parts to slide together after printing.

<img width="344" height="266" alt="Screenshot 2026-10-19 184111" src="https://github.com/user-attachments/assets/0c306b4f-b8a4-484c-b173-761f58b9f9b3" />
<img width="344" height="266" alt="image" src="https://github.com/user-attachments/assets/4cd5f83f-a1e0-4b87-a989-f17827ee6911" />

## 3D Print 

After completing my CAD model, I imported the parts into PrusaSlicer to prepare them for 3D printing. 

As I arranged the parts, I had a terrifying realization that my model was huge. The stand extended beyond the build plate, meaning they would not fit in their original orientation.

<img width="530" height="397" alt="image" src="https://github.com/user-attachments/assets/edeb388d-eda4-4bce-a3ea-8e34995ecf99" />

One option was to print the parts upright, but this would increase printing time and potentially make them weaker due to the direction of the layer lines. Instead, I rotated and repositioned the parts to fit the build plate.

<img width="428" height="317" alt="image" src="https://github.com/user-attachments/assets/e8cdf978-b8d8-4e9f-9f54-3a02c1044260" />

Finally with everything fit snug on the build plate, this is what I ended with.

<img width="413" height="320" alt="image" src="https://github.com/user-attachments/assets/476d0466-623f-4ac2-a372-e2a0228273b6" />

### Infill and Print Settings

Initially, I considered using 20% infill with a gyroid pattern because it provides internal support in multiple directions. However, after slicing the model and checking the estimated printing time, I realized I was already on a time crunch and would not be able to complete the print in time with those settings. I therefore had to make a sacrifice and settle for the default 15% infill with a grid pattern. However something that both have in common is that I chose three perimeter (which is one more than the default) and i kept the default layer height of 0.20 mm to keep a good balance between print quality and printing time. 

<img width="309" height="119" alt="image" src="https://github.com/user-attachments/assets/100520c7-3d3c-404e-a5c5-39578b298b24" />

> Gyroid pattern, 20% infill

<img width="314" height="149" alt="image" src="https://github.com/user-attachments/assets/591602c2-07b3-47d8-8a8f-f3d84c82b52b" />

> Grid pattern, 15% infill

I also aimed to minimize supports by choosing suitable print orientations. Avoiding unnecessary supports would save time and reduce marks left on the finished surface. I planned to print the parts directly on the build plate without a raft since they have enough contact. It's one of the reasons why I decided on a rectangular design for the stand and saddle rather than something circular which I saw a lot online.

<img width="269" height="255" alt="image" src="https://github.com/user-attachments/assets/b7924045-3a4c-4d9e-a171-fe6978ebac81" />

> PrusaSlcer Legend 

<img width="269" height="225" alt="image" src="https://github.com/user-attachments/assets/42a9a8f5-700a-4b12-a20e-50270b722d98" />

> 225 layers 

### UPDATE

As I was exporting the G-code, I realized there was a problem with my initial settings on PrusaSlicer. With the way I had my saddle oriented on its side, that meant there was an overhang. If I were to let it print as is, the top would have been susceptible to sagging. I'm relieved to have caught this before I started printing, as the printing time is already 4 hours.

<img width="298" height="289" alt="image" src="https://github.com/user-attachments/assets/3aa4e8d3-8fe0-4422-a826-fbc48c114973" />

> 265 Layers

<img width="622" height="497" alt="Screenshot 2026-10-20 094507" src="https://github.com/user-attachments/assets/bfa85219-0fcc-4a4d-9206-114832808388" />

> Legend, and saddle with newly added supports

<img width="277" height="125" alt="Screenshot 2026-10-20 094525" src="https://github.com/user-attachments/assets/40ec9f73-7e20-4287-aeaa-102f9407983a" />

> Final **official** time

### Printing 

I used machine PC_15 for two reasons- it had white filament which aesthetically matches my headphones. But the technical reason was that it is PLA filament, which is the setting I had applied when creating my G-Code

<img width="277" height="125" alt="IMG_2513" src="https://github.com/user-attachments/assets/5bcd0133-c144-4ccf-9396-0f7af85da6ff" />
<img width="150" height="125" alt="IMG_2511" src="https://github.com/user-attachments/assets/8ab7af71-d58f-413b-acb6-1c964aaaa601" />

Here is a progress shot and a [video](https://github.com/user-attachments/assets/30a5d2d5-c0be-4c1a-b228-f9079fc5478a) of my print while it was being printed. At this stage I was starting to see just how large the print would really be and I was hoping I did everything right since its such a large piece. 

<img width="298" height="289" alt="IMG_2517" src="https://github.com/user-attachments/assets/1e2a57b5-4d51-4204-be0a-7c46a1eed781" />

Things started to go awry when it came to printing the name. Since I’ve had this issue before, I wasn't surprised it happened. However, I wasn't too upset either; by then, the part had already extruded the appropriate amount and the letters were on top of the staff, meaning it was not going to hinder the tolerances. This didn't mean my design was a disaster. I could just go in with sandpaper to fix the unevenness and paint the piece instead of having my name extruded.

<img width="298" height="289" alt="IMG_2525" src="https://github.com/user-attachments/assets/5684474c-4ba6-4376-90bc-b6503cae98c6" />

Finally, here it is directly off the plate and assembled. 

*Pic*

The finish of the supports was about what I expected- it was rough which made me nervous since I was hoping to achieve a snap fit when snapping the staff into place. However removing the supports was simple and I still succeded to get it assembled. 

## Lessons Learned

One of the biggest lessons I learned from this project was the importance of early design planning. I was focused on creating a headphone stand that looked good and functioned as intended, but I did not fully consider how large the final model would be until I imported it into PrusaSlicer. Some of the parts extended beyond the build plate which forced me to go back and adjust their orientation.

Another challenge was balancing my ideal print settings with the time I had available. I originally wanted to use 20% gyroid infill, but after slicing the model, I realized that the estimated print time was not practical for my deadline. I settled on 15% grid infill instead, and although I was familiar with infill settings, this showed me how important it is to evaluate the actual print time early rather than assuming I will have enough time to use my preferred settings. In the future, I would slice my model earlier and use the estimated printing time to guide my design decisions.

I also learned to be more intentional about part orientation. I purposefully avoided orientations that would require unnecessary supports because they would increase printing time and leave additional marks on the finished parts. However, avoiding supports also meant I had to think carefully about how each component would sit on the build plate. It also doesn't hurt to have support in the first place. My overlook of the saddle could have cost me valuable time if I didn't catch it on time. Supports are meant to help not hinder your design, and after looking at the legend you will notice that it doesn't take much time to print at all.

The printing process itself took about 4 hours. However I had to put in research, measure, design my product, remove supports, then write my report which took about 5 hours. So in total this assignment took 9 hours. 

## Appendix 
[Toptal](https://www.toptal.com/designers/product-design/design-thinking-great-questions)

[Headphones.com](https://headphones.com/blogs/features/the-most-popular-headphone-stand-might-be-ruining-your-headphones-why-pads-matter)

[Moon Audio](https://www.moon-audio.com/blogs/expert-advice/stands-storage-cases-traveling-portable-audio-gear)

[Samsclub](https://www.samsclub.com/ip/HyperX-Cloud-III-Wired-Gaming-Headset-PC-PS5-Xbox-Series-X-S-Angled-53mm-Drivers-DTS-Memory-Foam-Durable-Frame-Ultra-Clear-10mm-Mic-USB-C-USB-A-3-5mm/20278224795?classType=REGULAR&from=/search) 

 
 
