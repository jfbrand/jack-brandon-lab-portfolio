# A9 – Laser Cutter

## Objective

1. Evaluate laser cutting as a viable manufacturing process. You will select and record machine settings, and explain the process's strengths and limits compared with FDM printing.
2. Measure laser kerf and actual material thickness, and apply both as engineered allowances so your joints fit reliably across the whole sheet.
3. Translate a parametric 3D model into 2D cut files, then back into a working 3D assembly.

**Team:** The project allowed us to work in groups of two to three. I worked with Josef Chelala and Joel Holder.

## Analyze

| Variable Name | Value | Units | Source | What it controls |
|---|---|---|---|---|
| Material Thickness | .27 | mm | measured | slot height |
| Kerf (x) | .097 | mm | calculated | slot length |
| Kerf (y) | .137 | mm | calculated | slot width | 
| Clearance | .2 | mm | chosen | fit |
| Slot Width | 2.95 | mm | calculated | slot width |

The above table shows the values obtained from measuring the material thickness with calipers by taking at least three measurements of each sheet used and calculating the mean value. The values of the kerf are also recorded for both the x and y. The values of the material thickness, kerf, and clearance were then used to calculate the slot width (y-direction). 

<img width="1077" height="625" alt="image" src="https://github.com/user-attachments/assets/64a08b45-a2e3-41a3-ab78-aa7cb3b975fb" />

<img width="510" height="681" alt="image" src="https://github.com/user-attachments/assets/54f5d1ea-4d42-479b-9811-f1fb2c76f1f8" />

The V1 test print was used to measure the kerf by choosing a nominal square size (25mm x 25m in this case) and measuring the resulting square coupon. The measured dimensions from the coupon were then subtracted from the nominal for both the X and Y to determine the kerf. Note the slot test fits as well as the different clearances being tested. We decided to try three fits: tight, target, and loose.

## Decide

We selected 0.2 mm for our clearance. This clearance was essentially the kerf plus 0.1 mm in both the x and y. We chose this clearance after performing our test 

## Design

<img width="1502" height="605" alt="Screenshot 2026-11-11 144200" src="https://github.com/user-attachments/assets/dcaef081-0f58-4ba4-8323-77669f3b9b3a" />

<img width="1012" height="467" alt="Screenshot 2026-11-11 144306" src="https://github.com/user-attachments/assets/859940da-8466-411a-a44b-a826e80a7f1d" />

<img width="731" height="522" alt="Screenshot 2026-11-11 144855" src="https://github.com/user-attachments/assets/4da8078a-cde2-44e0-811d-c9e8fe2ce888" />

<img width="958" height="356" alt="Screenshot 2026-11-11 142854" src="https://github.com/user-attachments/assets/b77f35b0-72f9-4c92-84e8-2034b0881345" />

<img width="1247" height="426" alt="image" src="https://github.com/user-attachments/assets/8a410104-faf2-48a6-b8cf-5096e0fec2e5" />

<img width="830" height="582" alt="Screenshot 2026-11-11 144009" src="https://github.com/user-attachments/assets/a76e2a10-0822-4f85-9b25-55ecdac69d89" />

<img width="802" height="510" alt="image" src="https://github.com/user-attachments/assets/2fd96b6b-8456-4e83-9284-a590125d8c7f" />

## Manufacturing

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

## Lessons Learned

| Date and time	| Time spent |	Step |	What happened |	Decision or change made |
|---|---|---|---|---|
| 10/23 | | | | |
| 10/26 | | | | |
| | | | | |

