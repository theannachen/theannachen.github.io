---
title: "Multi-Materials Pliers"
excerpt: "TPU and PLA filament printed pliers that are ready to use right after printing."
header:
  image: /assets/img/final-pliers.png
  teaser: /assets/img/final-pliers.png
gallery:
- url: /assets/img/first-pliers.png
  image_path: assets/img/first-pliers.png
  alt: "First Pair of Pliers"
- url: /assets/img/second-pliers.png
  image_path: assets/img/second-pliers.png
  alt: "Second Pair of Pliers"
- url: /assets/img/final-pliers.png
  image_path: assets/img/final-pliers.png
  alt: "Final Pair of Pliers"
- url: /assets/img/final-pliers.gif
  image_path: assets/img/final-pliers.gif
  alt: "Gif of Final Pair of Pliers"
---
# Print-in-Place Tools
Print-in-place (PIP) 3D printing is a filament printing technique that allows for both the creation of complex, articulated structures in a single print job, eliminating the need for assembly and using multi-material printing to design prints with parts that different in physical properties. By designing movable parts with precise clearances, PIP allows components like hinges, gears, and joints to function seamlessly straight off the print bed.
The goal of printing in place is to finish with a part that's ready to use and has full functionality right off the print bed. 

## Applications of Print-in-Place 3D Printing
PIP has been employed across various domains to produce functional and intricate designs:

Mechanical Assemblies: Designers have crafted gear bearings that operate smoothly without post-print assembly, showcasing the potential for creating functional mechanical components in one go. 

Collapsible Tools and Toys: Innovative designs like collapsing katanas and flexible animal models demonstrate PIP's capability to produce articulated and foldable items, allowing movable parts with ease.

Functional Household Items: PIP has been utilized to create items such as spring-loaded boxes and sliding bolt locks, offering practical solutions that are ready to use immediately after printing. 

An example of a practical usage would be if an astronaut on the ISS needed a pair of pliers and had access to a 3D printer. They could utilize print in place filament printing to create pliers that work, either through clever jointing or through multimaterial printing, which is what we will be walking through today.

## Material Combinations for Print-in-Place
PIP can utilize multimaterial printing to vary the part properties and allow for different colors, designs, or features to be available right after printing. 

Selecting appropriate materials is vital for the success of PIP designs, as well as understanding how the chosen filaments interact as some filaments will not bond together easier, creating a weak part or causing print failures. 

**Possible Combinations**
_PLA and PETG:_ Using PLA as a base with PETG printed on top results in easily separable layers, making this combination suitable for support structures that need to be removed cleanly.

_ABS/ASA and PETG:_ When PETG is printed onto ABS or ASA, the materials tend to weld together, creating a strong bond. This is advantageous for producing durable, multi-material components.

_TPU and PLA_: Combining flexible materials like TPU with rigid ones such as PLA can be challenging due to adhesion issues. Designing interlocking features can enhance the mechanical bond between these materials as well as creating movement with the TPU areas.

## Mutilmaterial Plier Design
Here is what went into my design of the multimaterial pliers. Technically this isn't a true PIP given that the parts were printed separately and assembled due to lack of access to multimaterial printers, but the design should continue to work in a true PIP setting. 

### Criteria 
For my pliers, the goal at the end was to be able to pick up and move resistors. Therefore, they needed to have a few criteria: 
- Small tips for picking up resistors
- Tips that don't open too wide but close together 
- And for fun, I wanted some ergonomic fingerholes for my handles. 

# Iterations
I went through two main designs on these pliers and three total prints. The main design was to have 5 total printed parts, 2 PLA handles, 2 PLA jaws, and 1 TPU flexible section to allow compressive movement.

The first design can be seen here, and did not close at the tips. Additionally, the fingerholes were in the handles themselves, which made them harder to use due to the angle of the hand required to put fingers through. The connection between the center piece and the handles were not firm, allowing for a lot of twisting motion causing he tips to be unable to fully meet up, making it difficult to precisely pick anything up. 
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4aa1c559bf55ebca3?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

After some tweaking, I increased the distance between the handles as well as elongated the tips, adding a slight angle to the ends to allow them to meet properly. 

On my second print, it was closer to being successful and the ends were angled to close all the way with easier to use fingerholes, but the handles were still just a bit too wide for the tips to meet.
### Final Design
For the final design, I printed one with even more distance between the handles, allowing the pliers to finally close properly, forming a nice closing point. The center piece is solid in the model, but was sliced without the top and bottom layers, alongside a grid support structure that mimicked the exact pattern needed to create the compression motion.

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4af75bd8c8ef1f120?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

The final pliers can open to 14mm wide and close all the way, with a 23mm are that closes all the way along with a total jaw length of 75 mm.

{% include gallery caption="Iterations of pliers" %}
