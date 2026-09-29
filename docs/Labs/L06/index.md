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

I chose a safety factor of 3 because it would more than suffice for the purpose of this project and I chose the radius because it was the required dimension to fit the holes on the motor. Lastly the transverse load was set to 1 lbf as a reasonable assumption of the force required to deflect the flexure. The length of the flexures was found to be too long to facilitate a tight mate between the motor mount and motor. The calculated length of .196 in was replaced by .18 in for this reason.

<img width="1186" height="266" alt="image" src="https://github.com/user-attachments/assets/0c046473-acf5-4f2b-b2bf-be084c356a40" />

<img width="722" height="726" alt="image" src="https://github.com/user-attachments/assets/1b822852-5aa7-45af-bf4b-16cc8a10c528" />

<img width="872" height="651" alt="image" src="https://github.com/user-attachments/assets/01b3f197-24e0-4073-beac-69349afca299" />

<img width="802" height="747" alt="image" src="https://github.com/user-attachments/assets/19ca3c03-7c6e-4e2f-8a94-1534e7b2e77c" />

<img width="852" height="546" alt="image" src="https://github.com/user-attachments/assets/6bd9ae5a-1abb-4d96-b0a2-69713e5ff4b4" />

<img width="716" height="737" alt="image" src="https://github.com/user-attachments/assets/acdce575-6ebe-4f28-b71f-d1596f35c7e1" />

<img width="822" height="632" alt="image" src="https://github.com/user-attachments/assets/d514150a-6e4b-4f8d-8fda-e85bcac7bb74" />

<img width="640" height="737" alt="image" src="https://github.com/user-attachments/assets/82847906-a021-4e35-acaf-7fe2c3852895" />

<img width="717" height="656" alt="image" src="https://github.com/user-attachments/assets/427c50e1-30c1-43f4-923c-50132c8e42e0" />

<img width="670" height="742" alt="image" src="https://github.com/user-attachments/assets/d22fa437-89fb-49ae-a356-606ba6f75cc3" />

<img width="622" height="757" alt="image" src="https://github.com/user-attachments/assets/c30bd388-b86f-4ca8-80bb-3803e6bb3c89" />

<img width="782" height="717" alt="image" src="https://github.com/user-attachments/assets/85c7d550-f4ee-4c59-87e8-79d65c3c787c" />

<img width="697" height="532" alt="image" src="https://github.com/user-attachments/assets/fac54788-2378-4aeb-b070-32238bc5efbd" />

<img width="607" height="730" alt="image" src="https://github.com/user-attachments/assets/5cdd0cfa-91a6-4a1e-b74b-3725c9e5979a" />

<img width="605" height="717" alt="image" src="https://github.com/user-attachments/assets/0fab3712-4ea6-4078-80f5-55724c5fb812" />

<img width="637" height="742" alt="image" src="https://github.com/user-attachments/assets/f7e9446f-adcf-4982-afec-f96ac19d4b79" />

<img width="672" height="697" alt="image" src="https://github.com/user-attachments/assets/4feb7b2b-b4d3-4250-9339-dfa94916a4c4" />

**Documentation**

Machine: Prusa Core #PC-15

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

<img width="481" height="640" alt="image" src="https://github.com/user-attachments/assets/de6aafc9-5a46-49dd-93eb-b69a9b4cd5ff" />

<video src="https://github.com/user-attachments/assets/6d56c7ac-cb52-49c9-a78a-156e1b4f16a3" controls="controls" style="max-width: 100%;">
</video>

**Lessons Learned**


