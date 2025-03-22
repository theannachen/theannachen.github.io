---
title: "Microfluidic Separator"
excerpt: "Microfluidic Separator capable of separating particles between and "
header:
  image: /assets/img/MicrofluidicFusionSS.png
  teaser: /assets/img/MicrofluidicFusionSS.png
gallery:
- url: /assets/img/mold-black.png
  image_path: assets/img/mold-black.png
  alt: "Resin printed mold of microfluidics device"
- url: /assets/img/mold.png
  image_path: assets/img/mold.png
  alt: "Casted PDMS device."
---
# Introduction
Have you ever wanted to sort the microplastics in your bloodstream? Filter out all the coffee grounds that fall through the filter? Well, a microfluidic sorting device is what you're looking for!
Microfluidic (sometimes notated μFluidic) devices manipulate tiny volumes of fluids, typically in the microliter or nanoliter range, within precisely engineered channels. These systems use principles from fluid dynamics, allowing for controlled mixing, sorting, and other operations. Due to their small size and efficiency, microfluidic devices are widely used in fields like medical diagnostics, drug development, environmental monitoring, and lab-on-a-chip technologies.
Pinch flow fractionation (PFF) is a microfluidic sorting technique used to separate particles based on size. It works by introducing a fluid stream containing the particles into a tiny channel alongside a second fluid stream. As the fluids converge at a narrow region (the "pinch" point), the larger particles are pushed closer to the channel walls, while smaller particles remain near the center. Downstream, the channel widens, and carefully positioned outlet streams collect the size-fractionated particles. PFF is particularly useful for sorting biological cells, nanoparticles, and other microscale materials without requiring external forces like electricity or magnetism.
An example of how this is used in the medical field is for early detection of cancer cells in the blood stream [Nagrath, et. al. (2007)](https://www.nature.com/articles/nature06385).
This page will use an example that separates particles 125 – 150 μm and 425 – 500 μm as reference.

# Instructions
But how do we actually do this? Is it feasible to get this technology at home? Well, there's actually a process for the rapid prototyping of these devices at home, albeit with some equipment.
If you have a resin printer and access to Parylene, polydimethylsiloxane (PDMS), and a microscope slide, here are the steps to creating your own microfluidics sorter at home.

- Creating a CAD model for the mold
  - First, design a CAD model in your favourite CAD software, taking into consideration the calculations for the particle sizes for the PFF. 
  - Also, remember that half of the liquid is coming from the channel without the particles and take that into account when you're designing the device. 
  - Finally, keep in mind that this is a negative/mold when building.
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a404fe0a090d794359?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
- Resin printing the mold
  - After creating the cad model,the use of resin printing technology can help create a high fidelity mold. 
  - Be sure to print the model flag on its back to guarantee a clean surface where the microscope lens touches the device
  - Postprocess and cure the resin mold after printing to ensure there is no tackiness on the build.
- Parylene application
  - Most resins are not bio-compatible, and would kill any cells that come in contact. Therefore, the application of parylene is essential for biocompatibility as well as helping strengthen the mold and release easier. 
  - This should be done in a well ventilated environment through chemical vapor deposition to achieve even coating. 
- PDMS Casting
  - Polydimethylsiloxane (PDMS) is a silicon based polymer that can be used for the creation of the actual devices and will be used for its biocompatibility and being clear, which will help us monitor the microfluidic process. 
  - The device will then be plasma bonded with a microscope glass, allowing a viewing window and a flat structure. 

# Discussion
This specific process in creating a microfluidic device allows for a quick, relatively cheap way to create biocompatible microfluidic devices. The parylene separation layer along with the PDMS material creates an environment that is easy to handle and safe for use with blood, one of the main applications of the technology, where a sorter could be used to separate cells by size. 
This specific design of the microfluidic separator utilizes 4 output holes, one for each particle size and two for the output streams, in order to balance the output flow rates. Additionally, it uses thicker, wider channels for the longer channels to help balance it. 
Choosing a pinch width of .75mm allows for all particles to get past and also takes into consideration the resolution of the resin printers. The widest part of the device for the separation was designed to give the particles enough room to settle into the right widths for the separation. 

{% include gallery caption="Images of the finished microfluidics device." %}


