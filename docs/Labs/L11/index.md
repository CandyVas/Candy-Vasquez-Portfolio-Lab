# A11 – Motor Selection

## Objective


## Snap Fit Research

All types of snap joints have in common the principle that a protruding part
of one component, e.g., a hook, stud or bead
is deflected briefly during the joining opera-
tion and catches in a depres-sion (undercut)
in the mating component.

After the joining operation, the snap-fit fea-
tures should return to a stress-free condition.
The joint may be separable or inseparable
depending on the shape of the undercut; the
force required to separate the compo-nents
varies greatly according to the design. It is
particularly im-portant to bear the following
factors in mind when designing snap joints:

this can be sen in the cantilver design snap fit where 

The four cantilevers on the control panel mod-
ule shown in Fig. 1 hold the module firmly in
place in the grid with their hooks, and yet it can
still be removed when required.

<img width="197" height="241" alt="image" src="https://github.com/user-attachments/assets/01ae782d-e9ae-42f9-9d78-c88f468c1b2f" />

Good results have been obtained by reducing
the thickness (h) of the cantilever linearly so
that its value at the end of the hook is equal to
one-half the value at the root; alternatively, the
finger width may be reduced to one-quarter of
the base value (see Table 1, designs 2 and 3).
With the designs illustrated in Table 1, the vul-
nerable cross section is always at the root (see
also Fig. 8, Detail A). Special attention must
therefore be given to this area to avoid stress
concentration.

<img width="326" height="212" alt="image" src="https://github.com/user-attachments/assets/41e290bb-439e-415e-b55f-4a1425f0790e" />
<img width="529" height="236" alt="image" src="https://github.com/user-attachments/assets/6926da0a-3d30-45a9-9873-ffd67c8441ab" />


Thick sections will usually result in sinks and/or voids
which are signs of high residual stress. For this
reason, the designer should reach a compro-
mise between a large radius to reduce stress
concentration and a small radius to reduce the
potential for residual stresses due to the cre-
ation of a thick sec-tion adjacent to a thin sec-
tion. 


<img width="501" height="346" alt="image" src="https://github.com/user-attachments/assets/aaf3261c-9253-4521-8ed1-898869a0ebf1" />

in this image we will only be focusing on column A for th sake of design convenience. 

The permissible deflection y (permissible
undercut) depends not only on the shape but
also on the permissible strain E for the mate-
rial used.

## CAD

The type of snap-fit I designed was a cantilever 

starting on the top plane i center my square to make it 60 by 60 mm and extrude it by 2.5

<img width="270" height="245" alt="image" src="https://github.com/user-attachments/assets/df703c7b-adf0-488d-8172-4c358bfe5029" />
<img width="566" height="310" alt="image" src="https://github.com/user-attachments/assets/03e0345c-8fe8-455f-9023-f70154d563ca" />

<img width="444" height="317" alt="image" src="https://github.com/user-attachments/assets/d408e033-422e-4fe6-84bd-cec0f62a1ebc" />


<img width="467" height="278" alt="image" src="https://github.com/user-attachments/assets/ffe259c4-6ad1-4701-bf67-d83fff73d93c" />

For the hooks i made a line of 1.5 mm and turned it into a triangle so it can snag onto something

<img width="244" height="204" alt="image" src="https://github.com/user-attachments/assets/f30680c9-ddc8-4994-bc83-daae557afe9e" />

i essentially repeated the same steps from earlier and mirrors this piece to the other side and extruded it. 
<img width="487" height="191" alt="image" src="https://github.com/user-attachments/assets/fcc648e7-25f7-4f3a-b1c0-ea719c82f69b" />


i added filets to reduce stress, and that concluded mylid 

Starting on th box itself, i made anoter box that was 60 by 60 and extruded it by 20 mm

<img width="443" height="292" alt="image" src="https://github.com/user-attachments/assets/a09bda29-282a-450c-b883-c43b49214d88" />
<img width="443" height="264" alt="image" src="https://github.com/user-attachments/assets/09a72696-c935-4c2e-a01c-945c281077ab" />

i clicked on the topplace and shelled it by 2.5 
<img width="491" height="319" alt="image" src="https://github.com/user-attachments/assets/0754b2fd-c68f-4f5d-bcd7-8cfb920e725c" />

there was no need to do the other side as i extrude dthru the toher side of the box 

<img width="164" height="275" alt="image" src="https://github.com/user-attachments/assets/dcafd1fa-8cb1-4ce3-a1ad-ecf33a37734d" />

<img width="159" height="203" alt="image" src="https://github.com/user-attachments/assets/8270a02a-624c-44ff-997a-f410be52e464" />

<img width="376" height="259" alt="image" src="https://github.com/user-attachments/assets/5b5d1bc3-b726-4387-a217-427c1a780586" />



<img width="571" height="287" alt="Screenshot 2026-11-03 150317" src="https://github.com/user-attachments/assets/8e370787-2bdc-4402-86a0-dcb8b7a530f3" />

<img width="338" height="296" alt="Screenshot 2026-11-03 150428" src="https://github.com/user-attachments/assets/3a7795eb-0062-4d8d-923a-8d5c661284c3" />

<img width="414" height="269" alt="image" src="https://github.com/user-attachments/assets/0d38f59d-0867-43e5-8b68-a43572eea489" />

## Preprocessing and 3D Print

i wanted to avoid supports being on the inside of my box so it wouldnt interefere with my fit, however after many attempts of orienting my bo, it looked to be impossible to avid supports on the interior, atleast not wihtout weak spots hich PreFOrm displays with orange. Therefore i settle don this, and upon closer inspection you will notice that it does *not* touch the snap feature, which is example that iw as looiking for 

<img width="200" height="149" alt="image" src="https://github.com/user-attachments/assets/648748bd-466d-40a5-b483-a476ed8f869c" />
<img width="316" height="194" alt="image" src="https://github.com/user-attachments/assets/dab3cc1b-ad71-4cfc-a5e5-9172cfa4b8c5" />

<img width="323" height="391" alt="Screenshot 2026-11-03 152407" src="https://github.com/user-attachments/assets/6ed24bdf-c916-4a77-81de-a20f7686abe0" />

I gt to th fablab and was hoping to print on th printer i was familiar with which was HiddenCod since that is what i estalished my settings for in terms of the material that it's going to print in. However HiddenCod was taken up, so I ended up printing on MatureImpala, luckily they had the same settings 

<img width="215" height="425" alt="Screenshot 2026-11-05 125135" src="https://github.com/user-attachments/assets/17fc86cd-a89e-4a10-8099-ab59104279d7" />
<img width="208" height="218" alt="Screenshot 2026-11-05 125202" src="https://github.com/user-attachments/assets/c36d5650-1740-4819-8560-bd292405f8ee" />

## Post-Processing

## Validation

