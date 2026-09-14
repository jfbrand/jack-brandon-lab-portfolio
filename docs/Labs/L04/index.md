

https://github.com/user-attachments/assets/6f14d12d-42a8-4d97-82f0-1e31a3244f9c



https://github.com/user-attachments/assets/fa7a77c1-4979-4bd4-8446-03cf8e896e89



https://github.com/user-attachments/assets/1a5e4898-1527-4b95-8787-0a1e13389045

# A4 – Benchmark a Parameter

## Objective

The goal of this project was to choose a parameter to test the limits of the Prusa Core One 3D printer. This would determine if the standard design constraints were universal (for every printer) or if there were enough differences between printers to make these rules generally recommended but not exact. Consequently, this would lead to more knowledge of the limitations of the Prusa Core One, resulting in superior 3D printed parts in the future.

## Parameter

**Analyze**

Given the four following parameters, one was to be selected for testing:

1. Overhang angle test
2. Pull strength test
3. Tolerance gauge test
4. Dimension calibration test

For the purpose of this project, the overhang angle test was chosen. The standard rule regarding overhangs is to avoid an angle of greater than 45 degrees from the vertical axis of the part. This constraint is exists because of the inherent limitations in unsupported filament before cooling. Angles less than 45 degrees have enough surface area contact between each prior layer and the next to create a shelf for that new layer. With more horizontal angles, lack of support and time it takes the filament to cool become the limiting factors.

**Prediction**

The predicted result was a noticeable reduction in print quality starting at angles greater than 45 degrees. At 49-50 degrees the print would fail/collapse.

## Design

**Decide**

<img width="1067" height="742" alt="image" src="https://github.com/user-attachments/assets/883db30d-d0f3-4ee5-a750-b790604520f5" />

The test part was designed to test overhang angles of 40 to 50 degrees. Each overhang had a different angle, starting at 40 on the first and increasing by 1 degree for each overhang until reaching 50 degrees on the last.

<img width="1917" height="1016" alt="Screenshot 2026-09-10 132716" src="https://github.com/user-attachments/assets/e97672bf-954c-4f5f-b9e0-4c55f161834c" />
<img width="1917" height="1018" alt="Screenshot 2026-09-14 145403" src="https://github.com/user-attachments/assets/aead1aa9-d866-4255-8c3a-ac7989b90d44" />
<img width="1917" height="343" alt="Screenshot 2026-09-14 145606" src="https://github.com/user-attachments/assets/bd54e632-3de5-4145-a3f0-13f9102912fc" />
<img width="1917" height="342" alt="Screenshot 2026-09-14 145543" src="https://github.com/user-attachments/assets/d2fc45f5-2915-40aa-bd84-878f2f56872a" />
<img width="1917" height="312" alt="Screenshot 2026-09-14 145519" src="https://github.com/user-attachments/assets/5be8937a-3b71-4acb-86c1-03caa6161d47" />

The following slicer parameters were chosen:

Infill: 15%, Grid pattern

Build Orientation: Bottom face down (same as CAD)

Supports: None

Scale: X: 100% Y: 100% Z:100%

**Design Process**

<img width="1257" height="515" alt="image" src="https://github.com/user-attachments/assets/2244e8ff-b0d5-4061-a491-22262adf7dfa" />

First a 5.5 in X 1.5 in rectangle was sketched.

<img width="1482" height="641" alt="image" src="https://github.com/user-attachments/assets/ba8366b9-e6cd-4977-987d-94e4567eb3d2" />

The rectangle was extruded to a height of .25 in.

<img width="1202" height="442" alt="image" src="https://github.com/user-attachments/assets/f62aa010-068c-40c6-acd3-a3d1485e13dd" />

1.5 in X .25 in rectangles were sketched on the top face of the rectangle as shown.

<img width="1437" height="761" alt="image" src="https://github.com/user-attachments/assets/a8dc616e-e444-4853-912d-bf53468f8287" />

Every other rectangle (11 total) that was just sketched on the top face is extruded to a height of 1 in.

<img width="1432" height="750" alt="image" src="https://github.com/user-attachments/assets/3cf8e5a4-23a7-440c-8afc-f32e18df9934" />

(Optional) The extra base material is extrude cut. This was done to save filament.

<img width="1432" height="640" alt="image" src="https://github.com/user-attachments/assets/f86073bf-32f8-473b-a5d9-528f877bcba5" />

The corresponding angle for each overhang was sketched on the side of each face (YZ plane), as shown. The angles range from 40-50 degrees, in 1 degree increments. This range was chosen to give a 5 degrees "above and below" test.

<img width="1447" height="716" alt="image" src="https://github.com/user-attachments/assets/6d979e8b-c5b1-45b6-ad45-6a7b956c8c3e" />

Finally, the material was extrude cut from each overhang, exposing the angle.

## Preprocessor

Material: PETG

Infill: The 15% density grid pattern infill was chosen because it is light and strength was not needed for this test. The purpose was simply to  test the capability of the printer to go beyond the 45 degree angle overhang and so strength was less important than print quality and finish. Furthermore, 15% density is a common infill density. 3D printed parts. The same is true of the grid infill: it is extremely common and in most slicers, standard unless changed, giving a good baseline for this test.

Walls: 2 perimeter walls were chosen to provide a worst case scenario for the test. More walls would theoretically provide more support.

Build orientation: The bottom side down build orientation was the only orientation that made sense for the printing of the test part. If it was printed in any other orientation, the overhangs would not be oriented correctly.

Supports: Supports were not used because the purpose of the test was to expose the limitations in printing overhangs with the Prusa Core One.

Scale: The scale was not changed as the part was designed with appropriate dimensions from the start.

## Print Artifact

<img width="1629" height="1000" alt="image" src="https://github.com/user-attachments/assets/2ffaf68c-98be-4c21-8fc7-9e8186207418" />

<img width="1920" height="540" alt="image" src="https://github.com/user-attachments/assets/db61a48a-5c16-45c0-8a70-d1b986aff6a4" />

The part tested the maximum overhang angle with the Prusa Core One 3D printer. 

## Lessons Learned

As can be seen from the photos, the overhangs performed better than my prediction. None of the overhangs experienced any severe sagging or failure. Viewing right to left in the photo, it can be seen that the print starts to diminish in quality as the angles get more horizontal. However, very little imperfections appear until 44/45 degrees. After the 45 degrees overhang, the face of the overhangs appear to get progressively more deformed with each step in angle. 
