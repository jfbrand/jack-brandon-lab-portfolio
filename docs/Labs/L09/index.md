# A9 – Laser Cutter

## Objective

1. Evaluate laser cutting as a viable manufacturing process. You will select and record machine settings, and explain the process's strengths and limits compared with FDM printing.
2. Measure laser kerf and actual material thickness, and apply both as engineered allowances so your joints fit reliably across the whole sheet.
3. Translate a parametric 3D model into 2D cut files, then back into a working 3D assembly.

**Team:** The project allowed us to work in groups of two to three. I worked with Josef Chelala and Joel Holder.

## Design

**Parameter Table**

| Variable Name | Value | Units | Source | What it controls |
|---|---|---|---|---|
| Material Thickness | 2.77 | mm | measured | slot height |
| Kerf (x) | .097 | mm | calculated | slot dim. |
| Kerf (y) | .137 | mm | calculated | slot dim. | 
| Clearance | 0.2 | mm | research, testing | fit |
| Slot Width | 2.95 | mm | testing | fit |

The above table shows the values obtained from measuring the material thickness with calipers by taking at least three measurements of each sheet used and calculating the mean value. The values of the kerf are also recorded for both the x and y. The values of the material thickness, kerf, and clearance were then used to calculate the slot width (y-direction). 

**Explanation**

We originally selected an insert to slot clearance of 0.1 mm based on research. However, after doing practical testing with our coupons to determine kerf and fits we found that a +0.25 mm in the Y and -0.475 in the X of our slots gave us the most reliable and desirable fit. This made sense as the material thickness across the sheet was roughly constant so we could make our slots 0.25 mm larger in the Y (width/height) than nominal. However, in the X direction (length) of the slot, both the slot and insert would have a kerf. This meant that we had to reduce the length of our slots to account for the double kerf for our wings. It was unknown as to why our test resulted in a good fit using a slot width that when added to our kerf resulted in a theoretical clearance of roughly 0.28 mm. This would seem to be too large when compared to our desired clearance of 0.2 mm. Similarly with our slot length being almost half a mm smaller than the nominal it would seem that it would be too tight (slight interference fit) lengthwise. This discrepancy will be discussed later.

**Modeling**

For our design, we decided to make a simple model aircraft. We tried our best to emulate the silhouette but focused mainly on the interfaces between the wing inserts and the slots in the fuselage and engines.

<img width="1502" height="605" alt="Screenshot 2026-11-11 144200" src="https://github.com/user-attachments/assets/dcaef081-0f58-4ba4-8323-77669f3b9b3a" />

The parametric table showing the slot width which was a constant due to the sheet width not changing (drastically). The x_diff variable was a constant that was subtracted from the length of each slot (which varied). Note the "fx" before each slot dimension in the sketches below showing the parametric references. 

<img width="1012" height="467" alt="Screenshot 2026-11-11 144306" src="https://github.com/user-attachments/assets/859940da-8466-411a-a44b-a826e80a7f1d" />

<img width="731" height="522" alt="Screenshot 2026-11-11 144855" src="https://github.com/user-attachments/assets/4da8078a-cde2-44e0-811d-c9e8fe2ce888" />

<img width="958" height="356" alt="Screenshot 2026-11-11 142854" src="https://github.com/user-attachments/assets/b77f35b0-72f9-4c92-84e8-2034b0881345" />

<img width="1247" height="426" alt="image" src="https://github.com/user-attachments/assets/8a410104-faf2-48a6-b8cf-5096e0fec2e5" />

<img width="830" height="582" alt="Screenshot 2026-11-11 144009" src="https://github.com/user-attachments/assets/a76e2a10-0822-4f85-9b25-55ecdac69d89" />

<img width="802" height="510" alt="image" src="https://github.com/user-attachments/assets/2fd96b6b-8456-4e83-9284-a590125d8c7f" />

The assembled parametric model.

## Manufacturing

**Process Research**

Laser cutting works by using a high powered laser to burn material guided by a motion control system (CNC or G-code) to cut or etch a pattern. The laser functions by stimulating "lasing materials" via electric discharges. The resulting light is then reflected with a series of mirrors through a lens to intensify it. The beam tends to be roughly 0.3 mm in diameter but a kerf as small as 0.1 mm is possible depending on the material thickness. 

Compared to FDM, laser cutting is much faster and has less material limitations. For example, laser cutting can be used on a variety materials such as wood, metal, ceramics, and plastics. The cost comparison reveals that laser cutting is much more cost effective for large production volumes when compared to 3d printing. However FDM is still more cost effective for small volume or prototyping. Geometrically, the two processes differ greatly; laser cutting is limited to 2D only, whereas 3D printing allows for complex 3D forms.

Sources: 

https://www.twi-global.com/technical-knowledge/faqs/what-is-laser-cutting

https://forgelabs.com/blog/3d-printing-vs-laser-cutting

**Laser Process Record**

| Setting	| Kerf coupon	| Fit coupon | Final cut |
|---|---|---|---|
| Laser cutter (name or number) | SFL LA-5 | SFL LA-5 | SFL LA-5 |
| Material type	| wood | wood | wood| 		
| Nominal thickness	|	3 | 3 | 3 |	
| Measured thickness (mean) | 2.77 | 2.77 | 2.7 |	
| Speed | 20% | 20% | 20% |
| Power	| 100% | 100% | 100% |
| Frequency or PPI (if applicable) | 20%| 20% | 20% |
| Number of passes | single | single | single |
| Focus method and how you confirmed it | default | default | default |
| Air assist on? Exhaust on? | both on | both on | both on |
| How you set origin and alignment | top left | top left | top left |

<img width="1077" height="625" alt="image" src="https://github.com/user-attachments/assets/64a08b45-a2e3-41a3-ab78-aa7cb3b975fb" />

<img width="510" height="681" alt="image" src="https://github.com/user-attachments/assets/54f5d1ea-4d42-479b-9811-f1fb2c76f1f8" />

The test print was used to measure the kerf by choosing a nominal square size (25mm x 25m in this case) and measuring the resulting square coupon. The measured dimensions from the coupon were then subtracted from the nominal for both the X and Y to determine the kerf. Note the slot test fits as well as the different clearances being tested. We decided to try three fits: tight, target, and loose.

**Cutting Video**

[Cut Video](https://drive.google.com/file/d/1Yhd49Kubzwd0K4hGeQ5sQCxCN9s4oubA/view?usp=sharing)

**Nesting/Layout**

<img width="305" height="445" alt="image" src="https://github.com/user-attachments/assets/f959ee2a-5336-440c-9ea7-7e052c0ac528" />

Our parts were laid out relatively close together to keep the overall surface area compact. This was done to save time by reducing the amount of traversing required to cut the parts.

**Air Assist/Exhaust**

We noticed that the ventilation system worked well to reduce the apparent amount and smell of smoke coming from the laser cutter. We intentionally waited for roughly 30 seconds before opening the laser cutter to ensure that all harmful smoke had been ventilated prior.

**Edge Quality**

We did not have any issues with edge quality during the project.

## Lessons Learned

**Process Log**

| Date | Time | Step | Occurrence/Decision |
| ----| ----- | ----| --------------------- |
| 10/23/26 | 1:57pm | 1 | Material thickness measured (2.70 mm) |
| 10/23/26 | 2:38pm | 2 | Test Coupon cut, Measured |
| 10/23/26 | 3:24pm | 3 | Fit test V1 cut |
| 10/23/26 | 3:32pm | 3 | Fit test V2 cut |
| 10/23/26 | 3:39pm | 3 | Fit test V3 cut |
| 10/23/26 | 3:50pm | 3 | Fit test V4 cut |
| 10/23/26 | 4:02pm | 3 | Fit test V5 cut |
| 10/23/26 | 4:10pm | 4 | Clearance chosen (.100 mm) |
| 10/26/26 | 2:24pm | 2 | Kerf calculated (.097 mm X, .137 mm Y) |
| 10/26/26 | 3:05pm | 5 | Initial CAD completion |
| 10/26/26 | 5:04pm | 5 | Final CAD completion |
| 10/26/26 | 6:16pm | 5 | Final Inkscape file made |
| 10/26/26 | 6:31pm | 5 | Final laser cut completed |
| 10/26/26 | 6:44pm | 5 | Final assembly completed |
| 10/26/26 | 11:28pm | 6 | Parameter and Laser Process Record completed |
| 10/27/26 | 1:24pm | 6 | Documentation Completed |


