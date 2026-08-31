# A2 – First Print

Additive Manufacturing vs Subtractive Manufacturing

1. Additive manufacturing avoids unnecessary waste by only only using material needed for a given design, where as subtractive manufacturing starts with excess which is removed in the process.

2. Additive manufacturing can make parts that have much more complex geometries that would be otherwise impossible or extremely difficult to reproduce by subtractive manufacturing.

Design Rules in DfAM

1. Print orientation - Effects part strength and finish. This is to avoid overhangs or "stair stepping" which can create sagging in the part. Source: Google AI

Considerations in FDM

Overhangs - When unsupported material is bridging a gap in the part. This can cause problems with sagging while printing. The work around is either to change the print orientation to compensate for this or by increasing the part cooling to attempt to harden the filament faster.

Overhangs (Andy) - One work around is to add supports to the part to support the overhang. 

Layers/surface finish (Andy)- Typically visible on the part but can be made less visible by reducing layer thickness to 0.1mm for example (detailed setting) in order to increase the print resolution and improve the surface finish. The downside is it roughly doubles the print time.

Lab #2: Print Something Small

Downloaded from: https://www.printables.com/model/237108-master-chief-mark-vi-helmet-the-master-chief-colle

Halo is my favorite video game of all time and Master chief is of course my favorite character so naturally I decided to make a model of his helmet.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/128de4a2-2b3e-4cd2-ac68-393c9929b4ea" />

When I opened the file in Prusa slicer I immediately noticed that the model was massive: 10.37 X 14.96 X 11.76in.

<img width="792" height="552" alt="image" src="https://github.com/user-attachments/assets/de2cb8fd-5f8d-439f-86bc-d6cea96a5389" />

In order to meet the dimension requirements of the part (2 X 2 X .25in) I scaled down the size to only 2%. The height limit of .25in resulted in a very tiny part. Knowing this and wanting to retain some detail, I changed the layer height to .10mm. I also tilted the helmet back to roughly 315 degrees to create a 45 degree angle with the visor with respect to the build plate. This was done to reduce sagging. Finally I selected "supports everywhere" to give the helmet a stable build platform.

<img width="502" height="487" alt="image" src="https://github.com/user-attachments/assets/cb1cdc6a-b5dc-4ea3-a2b0-95cdf3962dc5" />

I then clicked "slice now" and left the default slicer settings. 

<img width="1917" height="1020" alt="Slicer Screenshot" src="https://github.com/user-attachments/assets/bc57f7a0-e4b7-483d-8280-cb7620d5d8a1" />

I then inserted the Prusa printer flash drive and exported using the "Export to SD/USB drive button (small disk/drive icon). I then saved to the connected flash drive, and clicked the eject button in the bottom right corner of PrusaSlicer to remove the flash drive.

Next, I inserted the flash drive into the printer and selected the gcode file. I used standard eSUN PLA filament and Printer 5 in the Super Fab Lab. 

[![Watch the video](https://shields.io)](https://drive.google.com/file/d/1giiN5Ri11dBXm_wngNWB4mpthpZF61l-/view?usp=sharing)

After roughly two minutes of print time, it was finished. Here is the model after removal from the print bed, with supports still attached. It's tiny!

<img width="480" height="640" alt="image" src="https://github.com/user-attachments/assets/55e75d72-fc89-435a-8b57-1f30dc5e6b67" />

The finished product.

<img width="1440" height="1920" alt="image" src="https://github.com/user-attachments/assets/6ce09a6c-f3e1-4ca5-947f-a093babf92d6" />

<img width="1440" height="1920" alt="image" src="https://github.com/user-attachments/assets/9c07005e-e9d3-42e3-91f4-87b2a5216d7d" />

If the goal was to "make something small" I'd say I accomplished that! 

<img width="1440" height="1920" alt="image" src="https://github.com/user-attachments/assets/a7b2c48d-504f-420c-a579-e3c591626388" />

