# A8 – Design and Print Something Useful

## Objective

The goal of this project was to design and print something that was useful to myself or others using the what we have learned in the class so far.

## Reading and Writing

Response to "Great Questions Lead to Great Design: A Guide to the Design-thinking Process" by Jorge Juan Perales

Asking smart questions can make the difference between a good product or a failed one. Without asking the right questions, a designer can have an unclear problem statement that makes the design process difficult or impossible. This can cause time to be wasted trying to decide what improvements or features to focus on in a design or come up with a solution for a problem that is outside the scope of a project. This can happen for several reasons: a designer can be afraid to ask enough questions in order to avoid being perceived as a nuisance, fail to ask enough open ended questions to fully understand the intent of the project/design, or forget to ask important closed ended questions that give the designer necessary facts about the problem. Asking the right questions encourages critical thinking which helps the designer better understand the root cause of a problem or intent of a design. As we have learned in this class, engineering is the art of making decisions you can defend. Asking the right number and type of questions is crucial to making a decision that is defensible.

## Problem Statement

**Purpose:** The design was a simple, durable, and lightweight phone stand that could be used around the house or easily taken with you in a pocket or a bag. It needed to work for phones of different sizes and in different orientations, while also offering enough stability to be used while on the stand. Many examples of these existed but few had a combination of all of these features while still being affordable.

**Discovery:** I noticed the problem while cooking in the kitchen. I realized that it was frustrating to try and scroll through and read a recipe on my phone with one hand while doing another task with the other. When the phone was lying flat on the kitchen counter, it could be hard to read and prone to getting in the way or getting food on it. I realized that there were stands for recipe books already, and that something could be made that would work for a phone as well.

**User:** The product was intended to be used by people who use their phones while multitasking. I figured that this was a large part of the population.

**Design Approach:** The overall design was nothing nothing new, I had seen something similar before used to hold dinner plates. I took this concept and adapted it for my purpose by sizing it appropriately for a phone, creating a notch that would hold the phone securely in place, and creating a simple hinge mechanism to allow it to fold in half. I went straight to CAD and began modeling as soon as I envisioned the concept of the design.

## Design

<img width="552" height="636" alt="image" src="https://github.com/user-attachments/assets/4e0f936a-5858-4b60-9c4a-b0ec23e84514" />

The overall geometry was sketched. The angle was selected to create a natural viewing angle.

<img width="782" height="376" alt="image" src="https://github.com/user-attachments/assets/7467d8b9-8c2f-424e-9d28-af1dd69507c4" />

The base was extruded to .25 in.

<img width="860" height="375" alt="image" src="https://github.com/user-attachments/assets/872aa1e1-8144-4b7e-9c1a-83ee4cae9778" />

The edges were filleted.

<img width="1212" height="485" alt="image" src="https://github.com/user-attachments/assets/6de5cba3-8e82-4486-b763-66fd23ec661b" />

The hinge geometry was sketched on the right side.

<img width="1226" height="442" alt="image" src="https://github.com/user-attachments/assets/050f43a5-f5a0-4fb4-8d19-0c95b36f9459" />

The hinge geometry was sketched on the left side. The hinge was designed to have a 10 thou gap between the hinge features that interface with each other. The clearance dictated the spacing/location of the rectangles sketched here.

<img width="1057" height="466" alt="image" src="https://github.com/user-attachments/assets/acf8c8b2-c70e-4348-96f7-5370c387a93a" />

<img width="1227" height="517" alt="image" src="https://github.com/user-attachments/assets/3e760860-d44f-4547-8499-76244f051117" />

The hinge features were extruded.

<img width="952" height="507" alt="image" src="https://github.com/user-attachments/assets/cd041781-8cbb-45d9-adef-2232e13154d5" />

The features were filleted to a semi circle shape to allow the hinge movement.

<img width="672" height="482" alt="image" src="https://github.com/user-attachments/assets/b67ac256-6b21-472f-9118-a84e75f15e22" />

The geometry for the hinge pins was sketched.

<img width="617" height="522" alt="image" src="https://github.com/user-attachments/assets/ba42843f-e80c-43ef-be39-05a268e3e2d1" />

The hinge pins were extruded.

<img width="487" height="496" alt="image" src="https://github.com/user-attachments/assets/8ecca01f-b3c0-4da0-b0f8-9aedcd65e011" />

The hole dimension was .135 in, 10 thou larger than the pin size. This tolerance was chosen to allow free movement at the hinge and easy assembly/disassembly.

<img width="1092" height="497" alt="image" src="https://github.com/user-attachments/assets/7da7356b-d370-46b7-b5ce-07a70f0936b4" />

The holes were made in the hinge features.

<img width="1482" height="672" alt="image" src="https://github.com/user-attachments/assets/799e4a40-d1d2-44b3-9efa-dc8527849bd7" />

The completed halves of the stand.

<img width="1097" height="491" alt="image" src="https://github.com/user-attachments/assets/676c65d1-5d5c-4401-a208-669f58776bd8" />

The completed assembly.

## 3D Print

<img width="1917" height="1017" alt="image" src="https://github.com/user-attachments/assets/5d79ff9f-0395-4d69-bd24-31d92de2af35" />

1. Machine number:
2. Raft: not used
3. Wall thickness: 2 perimeters
4. Infill: 15%
5. Supports: on build plate only. Necessary for hinge pins. Used standard supports.
6. Support removal: removed by hand.
7. Layers: 76
8. Layer thickness: .15 mm
9. Build volume: 10.63 in^3
10. Support surface finish: rough
11. Layout: hinge features facing right, with halves next to each other
12. Build orientation: hinge features facing up, so that flat faces were down
13. Slicer settings: standard slicer settings except for addition of supports
14. Slice information:
  a. Used filament: 23.95 g, 308.64 in, 1.15 in^3
  b. Cost: 0.67
  c. Estimated printing time:
      -normal mode: 50m
      -stealth mode- 1h0m

<img width="400" height="600" alt="image" src="https://github.com/user-attachments/assets/890bc9b6-6a49-48ff-b116-1ebd70ddfb3c" />

<img width="400" height="600" alt="image" src="https://github.com/user-attachments/assets/43b1de1b-1ba7-4028-8ef1-4fec076ee8ff" />

<img width="400" height="600" alt="image" src="https://github.com/user-attachments/assets/9a27710f-904e-43d3-b96b-c029d4b4feff" />

## Lessons Learned

This project forced me to practice my CAD skills to a surprising degree. I ran into issues with the copy component process in Fusion 360. At first I made one of the halves of the stand without making it a separate component from the parent assembly. This created issues when I tried to copy the solid body to make the other half. I then realized that if I made both separate components within the hybrid assembly file, I could copy one to make the other and make modifications to each one independently (as originally intended). One thing I found useful was aligning the halves together so that the hinge could be designed more efficiently. This allowed me to have a better grasp of how I wanted the features to interact without having to make a sketch first. However, after a test print of the hinge assembly, I realized that I needed to leave extra room for the hinge features to interface so that the two halves could be aligned. This meant resketching the features of the hinge so that there was a 10 thou clearance. That modification was successful and the finished product had very good alignment. This project took me 9 hours from start to finish.
