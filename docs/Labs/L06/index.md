# A6 – Design Fits for an Artifact

## Objective

The goal of this project was to design a part that snap fits to an object that we selected in order to hone our skills in measuring, parametric modeling, and the iterative process.

## Analyze

**Instructions:**

In order to design a mated part, take measurements of an artifact's feature you wish to mate your design.
Parametrically design something small that snap fits (fits that cannot be pulled apart easily) into one of the features of the artifact measured in class. 
Use parameters in CAD
Use constraints in CAD
Test your design, if it does not fit properly redo.

## Decide

For this project I chose a small DC motor for my artifact. The motor had 2 small holes for screws on  its body and I decided that those would be perfect places for my snap fit pins 

## Communicate

**Parametrically Design**

<img width="1497" height="600" alt="image" src="https://github.com/user-attachments/assets/b7956e30-27d5-4839-9934-3f19a79025d8" />

The parameters used were yield strength of PETG (YS), second moment of inertia of a semi cylinder (I), radius, centroid, safety factor (SF), transverse load (P), and length of the flexures (L).

I chose the parameters because I wanted to be able to calculate the proper flexure length given the properties of PETG, the dimensional constraints of the feature, and the desired function.

I chose a safety factor of 3 because it would more than suffice for the purpose of this project. I chose the radius because it was the required dimension to fit the motor that. 

<img width="672" height="697" alt="image" src="https://github.com/user-attachments/assets/4feb7b2b-b4d3-4250-9339-dfa94916a4c4" />

**Documentation**

Machine: PC-12

Print Size: 2" X .305" X 1.5

Layout: Auto

Build Orientation: The part was oriented with the flexures parallel to the build plate in order to avoid shear stress between layers.

Supports: "Support on build plate only" due to not wanting supports inside the recessed holes of the motor mount.

Wall thickness: 2 perimeters.

Layers: 381 (.10mm) layers

Layer thickness: .10 mm

Build Volume: .33 cubic inches

Slicer settings: .10mm layer height- in order to facilitate the level of precision and detail required for the snap fit. 10% infill- More infill wasn't necessary 
given the lack of stress on the part. Grid infill- sufficient for the function of the part. 2 Perimeters- provided the necessary stiffness to the flexures.

Support removal: the supports were easily removed by hand.

Design modifications: the original top snap extrusions had too much overhang from the flexure and prevented the flexures from fitting into the holes in the motor. The diameter was decreased to a size only slightly larger than the nominal diameter of the holes.

**Show and Tell**

**Lessons Learned**


