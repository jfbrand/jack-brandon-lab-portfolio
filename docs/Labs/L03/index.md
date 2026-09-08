# A3 – Design Something Small

## Objective

The goal of this project was to gain experience creating a design, modeling it in a CAD software of choice, and subsequently printing that design on one of the printers in the UNCC print farm.

## Analyze

The design requirements were as follows:

1. No more than 0.5 inch tall
2. No overhangs (a deliberate simplification for this lab, supports are covered in a later lab)
3. Large enough to use infill
4. Modify wall thickness
5. Print in PLA or PETG
6. No more than 1.5 inches by 1.5 inches
7. Print time < 1.5 hours; confirm this using PrusaSlicer's estimated print time before sending to print

Given these requirements I figured the part would ideally be something relatively simple and mostly solid.

## Decide

<img width="852" height="490" alt="image" src="https://github.com/user-attachments/assets/2c337283-9472-4f51-a326-cb00ebba16d0" />

I decided to go with a basic pyramid design for this project. I chose this design because of its simplicity and solid geometry (no hollow parts or crevices) lending it to be plenty large enough for infill. Due to its shape it is also without overhangs. From a modeling perspective the shape is interesting because it is most easily created by using the loft function which I didn't have much experience with in Fusion. 

## Communicate

**Design**

<img width="657" height="615" alt="image" src="https://github.com/user-attachments/assets/159994b2-0b98-4b7f-93c0-8ec9ae9ead7f" />

First, I began by sketching a 1.5 by 1.5 inch square in the x-y plane (top view).

<img width="482" height="556" alt="image" src="https://github.com/user-attachments/assets/bbf1596e-47df-4398-985c-2d0ad039e5ee" />

Next, I found that the easiest way to produce the desired geometry was to create a point 0.5 inches above square, along the z axis (front view).

<img width="1477" height="782" alt="image" src="https://github.com/user-attachments/assets/435511e4-2fae-4a35-aa01-b1bb930a4b81" />

Then, the loft tool was used to create the desired geometry by selecting the square and then the point I had made in the last step.

**Research**

Three less common types of Infills in 3D Printing: Hilbert Curve, Archimedean Chords, Octagram Spiral.

Hilbert Curve: Looks like a rectangular maze. Used for filling a clear print with epoxy resin.

Archimedean Chords: A spiral that starts in the center of the part. Allows for easy bending for flexible parts and filling with liquid. 

Octagram Spiral: An eight sided spiral shape. Good for supporting flat top layers and easy to fill with liquid. 

Infill percentage effects the density of the part being printed. A part with higher density is stronger but also heavier. Different infill patterns can effect the mechanical properties of the part by decreasing the weight without it being at the expense of strength. Infills like honeycomb, for example, are lightweight and strong but have higher strength in certain directions. Infills like gyroid are isotropic and can better distribute stress in more directions than honeycomb. 

**Preprocessor and Printing**

Slicer Info:

The build orientation chosen was upright, resting on the bottom, square face. Because the part had a simple geometry this orientation worked well. 

Did you need to scale? If so, why and how?
What different infill was used in your print versus the default, and why was it used?
What was the wall thickness modified to, and why? Directly answer: why use different wall thicknesses?
Detail any mistakes throughout the process.

**Print**

<body>
  <h1>My Page</h1>
  <p>Some existing content...</p>

  <video controls width="100%">
    <source src="/videos/clip.mp4" type="video/mp4">
  </video>

  <p>More content...</p>
</body>

**Lessons Learned**
Detailed lessons learned throughout the process, the more detail the better. Which includes detailing any mistakes throughout the process and how you fixed them.
Actual time it took from start to finish, and resources.
What would happen if you scaled this decision up? If your infill percentage or wall thickness choice were applied to a structural or safety-critical part instead of a small desk object, what would the consequences of getting it wrong be?
What mistake did you catch, and what mistake might you not have caught? Detail an error you found and fixed. Then, more importantly: what's one flaw in your design or process that could have gone to print undetected, and what would need to change (in your process, not just this part) to catch it next time?
How does this connect to a real product decision? Identify a consumer or industrial product where infill strategy, wall thickness, or material choice affects user safety (it doesn't have to be 3D printed). Briefly explain the parallel.
**Resources**
List all resources used
