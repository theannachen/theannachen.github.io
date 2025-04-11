---
title: "Top Down Modeling"
excerpt: "Top down modeling demonstration for phone holder for your bike"
header:
image: /assets/img/render.png
teaser: /assets/img/render.png
gallery:
- url: /assets/img/render.png
  image_path: assets/img/render.png
  alt: "Render of Holder"
- url: /assets/img/1.png
  image_path: assets/img/1.png
  alt: "Handle and Base"
- url: /assets/img/2.png
  image_path: assets/img/2.png
  alt: "Bottom Handle"
- url: /assets/img/3.png
  image_path: assets/img/3.png
  alt: "Mount Enclosure"
- url: /assets/img/4.png
  image_path: assets/img/4.png
  alt: "Clamp"
- url: /assets/img/analysis.png
  image_path: assets/img/analysis.png
  alt: "Analysis of locking rotation mechanism"
- url: /assets/img/real-life.png
  image_path: assets/img/real-life.png
  alt: "Printed In Use"
- url: /assets/img/trimmed.gif
  image_path: assets/img/trimmed.gif
  alt: "Working Gif"
---
# Top Down Modeling
If you've worked in any CAD software, you're probably familiar with the option to import past models into a new file to use it as an external component. This allows you to create assemblies of multiple parts to make sure everything fits together. 
However, if you're creating multiple parts in their own files, you either have to create driven dimensions or keep copying and pasting the same parameters between parts, making it very easy for you to mess up and forcing you to keep track of multiple files and components. Furthermore, each time you edit a feature, you have to update it in the assemblies to catch it up. Wouldn't it be nice to be able to create all the parts in the same file?
With top down assembly, that is possible! Create all your parts in the same file, separated by components. You can project geometries between components for easy sketching, use the same parameters between components, and still assemble them using joints just like a normal assembly. The only downside is managing the sketches and extrusions, making sure that you are always in the active component you want before adding sketches and extrusions and making sure that all components are in the right parent component. 

# Bike Phone Holder Model Design
To try out this approach, I created a phone mount for a bike, allowing for easy usage of it for navigation while riding, etc. In order to make the mount fit any phone and any bike, I wanted to create something universal. 

## Bike Clamp
In order to fit multiple sizes of bike handles, I created this arc based shape that's held together by M5 bolts and nuts, allowing it to be tightened securely on the handlebars. 

## Phone Holder 
To hold the phone in, I added two spring-loaded clamps to the mount, allowing them to stretch to accommodate any sized phones. This would then be locked in onto the bulk in the middle with the rotational device. 

## Portrait/Landscape Rotation
When riding a bike, you might need to have the phone be displayed landscape or portrait. To allow the rotation, I designed hooks inside the mount that can accept an expansion spring and rotate between two separate orientations, locking in place with the spring each time. 

## Final Design
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a420dd0b4e7fb7b5ae?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Printing
The whole print was done using rigid PLA as that allowed for the best clamping force between for the phone. I originally had a bigger diameter for the circular part holding the detent spring, but shrunk it to create a tighter clamping motion. 

# Assembly 
The assembly of the phone holder is quite simple. First, attach an expansion spring inside of the enclosure, making sure it's one that's short enough to still be slightly expanded when fully closed. 
Then, attach the springs to the side of the enclosure and the clamps, again checking for a slight pull when fully closed. 
Finally, attached the handles to the back of the base using M3 bolts and nuts and use 4 M5 bolts and nuts to put the two parts of the handles together. Make sure to have bolts long enough to allow the handles to go around the handlebar of your bike. 

# Final Thoughts on the Design 
Overall, I am quite happy with my design. The clamping force of the phone holder was a lot more than I expected. Additionally, the handles gripped onto the bike handles fairly well, despite having no TPU part. I was initially worried that it wouldn't be enough as I had also just gotten a newer, larger, heavier phone before the final testing date, but it held up well. However, if I was to redo this, I would definitely have added an insertable TPU grip to make it hold onto the handlebars better. Can't have the phone sliding upside down while using it as a GPS!

{% include gallery caption="Individual Parts and Real Life Assembly" %}
