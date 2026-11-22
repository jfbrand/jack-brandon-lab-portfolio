# A10 – RC2 Sliding Fit Design and Verification

## Objective

The goal of this project was to design and fabricate a pair of parts (a hole/slot feature and a matching shaft/insert feature) that demonstrated an RC 2 sliding fit on a SLA print as defined in the Machinery’s Handbook.

## Research and Planning

**ASME RC 2 Sliding Fit Specification from Machinery’s Handbook**

“RC 2 Sliding fits are intended for accurate location, but with greater maximum clearance than class RC 1. Parts made to this fit move and turn easily but are not intended to run freely, and in the larger sizes may seize with small temperature changes.”

**RC2 Tolerance Range:**

Shaft/Bore diameter for 0.25" nominal:

Shaft: 0.2496 - 0.2498"

Bore: 0.25 - 0.2504"

Minimum clearance: 0.2 Thous (0.0002")

Maximum clearance: 0.8 Thous (0.0008")

**Hand Sketch**

<img width="972" height="781" alt="image" src="https://github.com/user-attachments/assets/ff99ee14-ff3c-413e-b90b-d3484c0e22b3" />


**Real World Applications**

An RC2 class fit would be used where some sliding and accurate location is needed. It's main advantage would be allowing movement without introducing unwanted play in components. Due to this RC2 fits are best used where accuratee location and sliding are needed such as lathe spindles, locating pins, sliding gears and clutches. This fit is also useful for jigs or fixtures where repeated locational accuracy is important. This fit is not suited for machinery that requires high speed sliding or rotating as it would generate too much friction and the fit clearance can fluctuate with temperature changes.

Source: Google

**Shrinkage and Expansion of Resin Prints**

Resin prints typically shrink by 0.3-2% linearly during printing and curing. Although it would seem that the a printed shaft and bore would theoretically shrink at the same percentage, there are variations in wall thickness and the polymer itself has high surface friction causing the fit to fail. Due to bleed/overcure, the inside wall of the bore can cure slightly inside and as the resin shrinks and contracts, the inner diameter of the bore decreases. This alone can account for 4-8 thou of lost clearance between the components. Similarly, the outer diameter of the shaft can cure outside of the correct diameter. It is these characteristics of SLA printing as well as the friction of polymer on polymer interfaces that necessitate a much larger engineered clearance for the SLA RC2 fit.

Source: Google

In order to avoid the parts seizing, the assembly was designed to have 12 thou (0.012") of clearance. This was estimated by accounting for the shrinkage, wall thickness fluctuations, friction, and seeing other test prints.

Chosen shaft/bore diameter:

Shaft: 0.238"

Bore: 0.25"

Key: 0.022" X 0.016" (L X H)

Slot: 0.03" X 0.016" (L X H)

Shaft/Bore Clearance: 12 thou (0.012")

Key/Slot Clearance: 8 thou (0.008")

## CAD Design

<img width="702" height="592" alt="image" src="https://github.com/user-attachments/assets/e3d422e2-2844-4091-bd55-e6e926034a7e" />

Base sketch.

<img width="707" height="647" alt="image" src="https://github.com/user-attachments/assets/30ce305c-06c1-4ee3-a42c-8a4469dee5c6" />

Shaft sketch.

<img width="712" height="537" alt="image" src="https://github.com/user-attachments/assets/82581874-f2cf-4812-9c0a-1908a5386425" />

Exploded view.

<img width="710" height="602" alt="image" src="https://github.com/user-attachments/assets/b45dba6c-c85a-45b1-9096-a9f387607a75" />

Assembled, compressed configuration.

<img width="688" height="657" alt="image" src="https://github.com/user-attachments/assets/25f986eb-9987-4e57-ba3c-bd3b8a06f2e6" />

Assembled, extended configuration

## Preprocessing for 3D Printing

<img width="946" height="817" alt="image" src="https://github.com/user-attachments/assets/71cf9da4-2f33-4c62-ab81-10e53af18bfc" />

**Machine name:** MatureImpala

**Build Orientation:**

Base: canted at ~ 45 degrees due to one click setup default settings

Shaft: vertical to prevent postprocess surface roughness from supports

**Layout:** 2 assemblies, 4 parts total, dispersed evenly in center of build plate

**Support Settings and Wall Thickness:**

Supports: one click setup default with rafts

Wall Thickness: default

**Layer Height and Print Time:** 

Layer Height: 0.1 mm

Print Time: 1h for both assemblies

**Total Volume**: 16.41 mL

**Allowable Clearance for Shrinkage:**

## Postprocessing

**Support Removal**

<img width="602" height="542" alt="image" src="https://github.com/user-attachments/assets/5e53c3e4-5293-4d44-b985-cf7b7037c0a2" />


## Fit Test

**Caliper Measurements**

Shaft:

Bore:

Key:

Slot:

**Measurement-Tolerance Comparison**

**Fit**

The parts slide relatively smoothly. The shaft can slide in and out of the bore with little effort as well as rotate to the "locked position". There is no perceptible play in the assembly.

## Lessons Learned


