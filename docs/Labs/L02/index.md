# L02

## Individual Research
### DfAM (Design for Additive Manufacturing)

One design rule/guideline specific to Design for Additive Manufacturing is the fact that it is being built layer by layer. This is important because it helps not only reduce waste, but it is also highly effective when designing lightweight, complex designs. 
(https://www.sciencedirect.com/topics/engineering/additive-layer-manufacturing)  

### FDM (Fused Deposition Modeling)

The one FDM consideration I chose to study was warping, which happens when there is a temperature difference between layers, causing the hot plastic to cool fast and shrink. This is visible through lifted corners or curling. One way to work around it is fixing the bed adhesion by cleaning your area or using adhesive like glue or tape. (https://www.sovol3d.com/blogs/news/3d-printing-warping-causes-identification-and-solutions) 

> Something new my teammate taught me about warping is if the design you have is too thick, the layers will start to peel. One way to combat this is by hallowing out your design and adding more space in the middle. 

## Finding a Design

We were tasked to download something from the website printables which offers an endless amount of free 3d prints that the public can download and print themselves. In honor of Halloween coming up soon, I wanted to find a design that was spooky, but cute enough to be incorporated into what I normally carry around. 



### Rejected Design 
> **Vintage Halloween Bat Wall Decor**
> A design that i thought to download but chose not to were these [Bats](https://www.printables.com/model/299289-vintage-halloween-bat-wall-decor) meant for wall decor. I decided not to because in our previous lecture we were discussing FDM considerations and in my research i looked into warping and layer adhesion. I was afraid that printing a flat design would cause the edges to lift, and these are lab printers used by plenty of students, so i didnt want a super thin deisgn to stick to the plate and struggling to take it off. 

<img width="130" height="124" alt="image" src="https://github.com/user-attachments/assets/8bb01ba5-0e51-4244-a052-94dbd1418057" />


### Final Design 
> **Halloween Ghost Keychain**
> The design I ended up settling on was a [Ghost Keychain](https://www.printables.com/model/288657-halloween-ghost-keychain). Not only does it fit in the terms of my own personal preferences, but it also fits inside the constrains found in this assignment. Keychains are meant to be small since and easily transportable. The design is much thicker than my initial decision, so the concern of warping isn't too relevant here. 

<img width="130" height="124" alt="image" src="https://github.com/user-attachments/assets/079e333e-6056-4bf7-b51e-4575841cf9ba" />



## Importing Files

<img width="652" height="160" alt="image" src="https://github.com/user-attachments/assets/c8ca4476-a1a4-470d-8349-2f3b8a5fdf28" />

>STL download

When downloading this model, i noticed that the download was in the format of a STL file, which is used for 3D printing which is exactly what's being done in this assignment. That file was then imported into PrusaSlicer and the printer we were instructed to choose from being the Prusa CORE One with a 0.4 mm nozzle. SInce PLA was the required material for this assignment, i also made sure to incoorprate that into the settings of my deisgn. 

<img width="959" height="500" alt="image" src="https://github.com/user-attachments/assets/95f56360-c349-43a7-8155-bfac2c279b27" />

>Imported Ghost into PrusaSlicer

This was what i was immediately met with after opening said STL file. No supports were needed in this model because it is not a floating design, nor will it overhangs anywhere. The build orientation i decided on was predetermined by the modeler of this object since that is exactly how it showed up when opening the model. on the other side of the design of the halloween face is a flat surface that helps secure it to the build plate. Meaning it would be printed flat, like how displayed in the image above. 

### Scaling
I was lucky enough to discover out this print matched most of this assignments requirements, and that i didn't have to do much tinkering when it came to downsizing my model. The only issue i came across was that the z value, the height of the print, surpassed the .25 inch height requirement. Thankfully not by a whole lot, and it was simple to fix. 

<img width="414" height="190" alt="image" src="https://github.com/user-attachments/assets/d914cac9-00be-40cf-8ffb-5265d8edb3f3" />
<img width="210" height="150" alt="image" src="https://github.com/user-attachments/assets/9fac0535-1120-4458-8301-6346c0bdc057" />

> Object Selected & Sliced info

This could have been fixed by either using the "Scale" [S] button on the right corner, which allows the user to drag and change the dimensions of their mode. However, i chose the option of simply going to the object manipulation window on the left side of my screen, and reducing my number down to exactly .25. 

This seems to have automatically scaled down the rest of my model down approximately 79% smaller. This change in size also impacted the print time, albeit a small amount, it makes sense that a smaller object would take less time to make because it wont take up as much room or materials. 

<img width="648" height="240" alt="image" src="https://github.com/user-attachments/assets/d67c96f7-81be-480a-908f-d24d1356c0e5" />

> Scaled Object & Object Manipulation Settings

### Slicing 

After making my alterations with the size, i clicked on the "slice now" button, keeping the default slicer settings. It changed my model from green to an orange highlight. Only after slicing did it give em the estimated time to print and the ability to export my model

<img width="414" height="190" alt="image" src="https://github.com/user-attachments/assets/4a5b7a11-b4bb-4522-8828-9f825d7c7d57" />
<img width="210" height="150" alt="image" src="https://github.com/user-attachments/assets/5f4ebda3-8509-4370-b55a-f5a548e8fb30" />

> Object Sliced & Sliced Info

Hence, I was able to finally exported my work into a g-code file, and made sure to import it into my USB. 
<img width="652" height="160" alt="Screenshot 2026-08-27 150822" src="https://github.com/user-attachments/assets/7c8af14d-21eb-41ed-86e2-509223cbb779" />
> G-Code Dowload

## Printing 

In the printing lab, there was a plenty of printers to choose from, but limited available for everyone present in the lab. I ended up pairing my design with a teammate, Kaileigh Hill. We decided on the printer that had the connected USb PC-07. This printer uses PLA filament as their material for printing. This was considered when choosing the printer settings since it was required in the assignment instructions. 

<img width="270" height="190" alt="PC 7" src="https://github.com/user-attachments/assets/8edc7838-542d-4cab-ab55-63d591a7bf01" />
<img width="190" height="230" alt="Screenshot 2026-08-31 134048" src="https://github.com/user-attachments/assets/532c8300-88df-404d-9e8e-4da5306b0edc" />
<img width="190" height="180" alt="image" src="https://github.com/user-attachments/assets/61d20ac5-59da-4ab5-bebd-7be97bc2f7bb" />

> 3-D Printer Setting Screen & PLA Filament

We added both our models to the same plate. After both were incorporated and we were happy with its placement, the design was sliced and given an estimation of 13 minutes to print, which makes sense considering these are two small designs meant to consider design speculations. 

<img width="763" height="406" alt="image" src="https://github.com/user-attachments/assets/b386bcc7-4d67-475d-94ff-ba8c607491ae" />

> Cherry & Ghost Model on Printing Plate

Using the designated USB PC-07 for the printer, the USB was slotted into the laptop in order to export the G-code (available after being sliced). From there we took the usb back into the printer with our designs on it and began the printing process.

### Printing Progress

I noticed that the printing did not happen immediatlley, and in the printing screen that displays the image being printed, it showed an estimate of 4 minutes for the nozzle to heat up. This makes sense since it's essentially melting material to be shaped layer by layer. As the time went on, we continuousl checked on the progress of our models to confirm weverythin was going well. 

<img width="190" height="270" alt="image" src="https://github.com/user-attachments/assets/0fbc2e42-6382-4f90-aafc-d7534dd9e0d7" />
<img width="250" height="230" alt="image" src="https://github.com/user-attachments/assets/bf111767-c27d-43a2-b6f6-8c9750dfd751" />

> Cherry & Ghost Printing Progress

If youll notice in the first iage above, the display shows not only both designs, but the percentage of completion for the prints. It shows a progress of 76%, as well as the remaining time for the print to finish, which was 3 minutes by the time that picture was taken. if you'd like to see a video progression of the printing, i have a 15 second video available [here](https://github.com/user-attachments/assets/4017d8cb-76a3-4264-b6a5-d051622c9464)

## Finished Product

After the 17 minutes, the models were finished and ready to be removed from the printing plate. I was fortunate enough to not have any issues with my ghost- removing it from the plate took no effort and there was no need for the scraper. It did not experience any of the warping i was initially afraid of with the intiial deisgn i almost picked. 

My only qualm, however this is a personal preference that seems unavoidable with 3D rinting is the textured outcome of the model. If i wanted it to have a smooth finish for painting, I'd probably have to sandpaper it. However it makes sense that a little texture exists, becase if you saw from the video above, 3D printing works in layers accomplished by lines and lines stacking on top eachother. 

<img width="140" height="134" alt="image" src="https://github.com/user-attachments/assets/62133b37-0f4b-4a52-88dd-cc73f3acb4d8" />
<img width="130" height="134" alt="image" src="https://github.com/user-attachments/assets/ab945b53-fe17-433c-a84c-16e1d745e27d" />

> Ghost Finished Result

## Lessons Learned

### 1. Look at Your Slice
>Only after slicing a design will it gave you the useful information of estimated printing times and how much filiment will be used. Useful information if you are on a time crunch or working with limited materials.

### 2. Check and Confirm Settings
>not every model is built the same, you can't expect to download a file and it fitting all your criteria. It's important that you choose the correct printer settings, filament that is going to be used, and connect it to the correct printer model.

### 3. Estimated Print Times
>3D printing is already a slow process because we are building on layer by layer. I was given an estimate of 13 minutes to print, however the printer needed time heating up which extended the time for the design to be finished by 4 minutes. Look at the given slice time as an approximate, not an exact amount of time a print will finish.

### 4. Object Infill
>The inside of a 3d design isn't always purely solid. When watching my ghost keychain get printed, the inside of my ghost was accomplished using a cross hatch design. This opposed to a hallow design, which may be lighter but not structurally as strong. Or a completely solid inside, which may take more material and time to print.
    
Something i would have changed throughout this process is probably choosing a more challenging design, especially since this was my first ever 3D print. Something more complicated could have pushed me to learn and look more into PrusaSlicer, especially if i were to go in and adjust orientation. 

+ The time it took to complete this excerise was approximately 60 minutes.

    + **20 minutes** was spent during the beginning of class, looking for a design.
 
    + Dowloading the file and adjusting the settings took **5 minutes**
      
    + Checking and confirming the slice off PrusaSlicer took **5 minutes**

    + We were given an introduction to the Rapid Prototyping Lab as well as how to work the printers, which took **10 minutes**

    + And finally, the printing came down to **17 minutes**
+ ... which totals to 57 minutes total.

Finally, I'd like to recognize Kaileigh Hill for the collaboration of this project as we manufactured our designs together. 

## Resources

[Printables](https://www.printables.com/) - Website I used to browse free 3-D printing designs

[Halloween Ghost Keychain](https://www.printables.com/model/288657-halloween-ghost-keychain) - The design I ended up printing.

[Vintage Halloween Bat Wall Decor](https://www.printables.com/model/299289-vintage-halloween-bat-wall-decor) - Rejected design I chose not to print

[PrusaSlicer](https://www.prusa3d.com/p/prusaslicer/) - Used for scaling and slicing chosen design to convert into appropriate G-Mode file

Rapid Prototyping Lab, UNC Charlotte  - Lab accessed for manufacturing chosen designs 
