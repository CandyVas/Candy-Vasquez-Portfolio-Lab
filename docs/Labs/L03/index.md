# A3 – Print a Design!

# Finding a Design

We were tasked to download something from the website printables which offers an endless amount of free 3d prints that the public can download and print themselves. In honor of Halloween coming up soon, I wanted to find a design that was spooky, but cute enough to be incorporated into what I normally carry around. 

The design I ended up settling on was a ghost keychain, which can be found via this link (https://www.printables.com/model/288657-halloween-ghost-keychain/comments). Not only does it match the vibe i was aiming for, but it also matches the stipulations of this assignment- keychains are small since it's meant to be easily transportable.
<img width="791" height="346" alt="image" src="https://github.com/user-attachments/assets/a1560496-011b-4048-bb92-a4ec494e0ded" />

A design that i thought to download but chose not to were these bats meant for wall decor. I decided not to because in our previous lecture we were discussing FDM considerations and in my research i looked into warping and layer adhesion. I was afraid that printing a flat design would cause the edges to lift, and these are lab printers used by plenty of students, so i didnt want a super thin deisgn to stick to the plate and struggling to take it off. 

<img width="758" height="352" alt="image" src="https://github.com/user-attachments/assets/9f365f86-ddf7-42f3-a7c8-a76629107b8b" />


# Importing Files

<img width="452" height="113" alt="image" src="https://github.com/user-attachments/assets/c8ca4476-a1a4-470d-8349-2f3b8a5fdf28" />

When downloading this model, i noticed that the download was in the format of a STL file, which is used for 3D printing which is exactly what's being done in this assignment. That file was then imported into PrusaSlicer and the printer we were instructed to choose from being the Prusa CORE One with a 0.4 mm nozzle. SInce PLA was the required material for this assignment, i also made sure to incoorprate that into the settings of my deisgn. 

<img width="959" height="500" alt="image" src="https://github.com/user-attachments/assets/95f56360-c349-43a7-8155-bfac2c279b27" />

This was what i was immediately met with after opening said STL file. No supports were needed in this model because it is not a floating design, nor will it overhangs anywhere. The build orientation i decided on was predetermined by the modeler of this object since that is exactly how it showed up when opening the model. on the other side of the design of the halloween face is a flat surface that helps secure it to the build plate.  

it would be printed flat, like how displayed in the image above. I was lucky enough to discover out this print matched most of this assignments requirements, and that i didn't have to do much tinkering when it came to downsizing my model. The only issue i came across was that the z value, the height of the print, surpassed the .25 inch height requirement. Thankfully not by a whole lot, and it was simple to fix. 

<img width="514" height="220" alt="image" src="https://github.com/user-attachments/assets/d914cac9-00be-40cf-8ffb-5265d8edb3f3" />
<img width="310" height="148" alt="image" src="https://github.com/user-attachments/assets/9fac0535-1120-4458-8301-6346c0bdc057" />


This could have been fixed by either using the "Scale" [S] button on the right corner, which allows the user to drag and change the dimensions of their mode. However, i chose the option of simply going to the object manipulation window on the left side of my screen, and reducing my number down to exactly .25. This seems to have automatically scaled down the rest of my model down approximately 79% smaller. This change in size also impacted the print time, albeit a small amount, it makes sense that a smaller object would take less time to make because it wont take up as much room or materials. 

<img width="748" height="263" alt="image" src="https://github.com/user-attachments/assets/d67c96f7-81be-480a-908f-d24d1356c0e5" />

After making my alterations with the size, i clicked on the "slice now" button, keeping the default slicer settings. It changed my model from green to an orange highlight. Only after slicing did it give em the estimated time to print and the ability to export my model

<img width="424" height="247" alt="image" src="https://github.com/user-attachments/assets/4a5b7a11-b4bb-4522-8828-9f825d7c7d57" />
<img width="311" height="150" alt="image" src="https://github.com/user-attachments/assets/5f4ebda3-8509-4370-b55a-f5a548e8fb30" />


Hence, I was able to finally exported my work into a g-code file, and made sure to import it into my USB. 
<img width="461" height="116" alt="Screenshot 2026-08-27 150822" src="https://github.com/user-attachments/assets/7c8af14d-21eb-41ed-86e2-509223cbb779" />

# PRINTING 

In the printing lab, there was a plenty of printers to choose from, but limited available for everyone present in the lab. I ended up pairing my design with a teammate, Kaileigh Hill. We decided on the printer that had the connected USb PC-07. This printer uses PLA filament as their material for printing. This was considered when choosing the printer settings since it was required in the assignment instructions. 

<img width="290" height="212" alt="PC 7" src="https://github.com/user-attachments/assets/8edc7838-542d-4cab-ab55-63d591a7bf01" />
<img width="212" height="290" alt="image" src="https://github.com/user-attachments/assets/9b167479-613b-47c9-8bad-f653e557e293" />
<img width="209" height="196" alt="image" src="https://github.com/user-attachments/assets/61d20ac5-59da-4ab5-bebd-7be97bc2f7bb" />

We added both our models to the same plate. After both were incorporated and we were happy with its placement, the design was sliced and given an estimation of 13 minutes to print, which makes sense considering these are two small designs meant to consider design speculations. 

<img width="763" height="406" alt="image" src="https://github.com/user-attachments/assets/b386bcc7-4d67-475d-94ff-ba8c607491ae" />

Using the designated USB PC-07 for the printer, the USB was slotted into the laptop in order to export the G-code (available after being sliced). From there we took the usb back into the printer with our designs on it and began the printing process.

I noticed that the printing did not happen immediatlley, and in the printing screen that displays the image being printed, it showed an estimate of 4 minutes for the nozzle to heat up. This makes sense since it's essentially melting material to be shaped layer by layer. As the time went on, we continuousl checked on the progress of our models to confirm weverythin was going well. 

<img width="207" height="350" alt="image" src="https://github.com/user-attachments/assets/0fbc2e42-6382-4f90-aafc-d7534dd9e0d7" />

<img width="374" height="356" alt="image" src="https://github.com/user-attachments/assets/bf111767-c27d-43a2-b6f6-8c9750dfd751" />

Iff youll notice in the first iage above, the display shows not only both designs, but the percentage of completion for the prints. It shows a progress of 76%, as well as the remaining time for the print to finish, which was 3 minutes by the time that picture was taken. if you'd like to see a video progression of the printing, i have a 15 second video available here 





