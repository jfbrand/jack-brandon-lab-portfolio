# A11 - Snap Fit Design for SLA Printing (Form 4)

## Snap-Fit Research

**Key Design Principles**

The chosen design was a strap clip. This mechanism utilizes two cantilever flexures that elastically deform and then "snap" back into shape when the undercuts are inserted past two cutouts in the receiving end of the clip. 

**Sketch**

<img width="827" height="762" alt="image" src="https://github.com/user-attachments/assets/a714d0fc-bb38-4b32-aba7-b132f35481e5" />

**Mechanical Principles**

The amount of deflection in each flexure dictates the both the durability and the performance of the clip. Too little deflection, and the notches will not be large enough to provide a strong snap fit. Too much deflection and the flexure will be prone to snapping and the clip will require too much force to operate. The permissible strain is the amount of deflection that the material can undergo without plastically deforming or breaking. This is effected by material, flexure length, and geometry. This is a key factor when designing for durability. 

<img width="552" height="327" alt="image" src="https://github.com/user-attachments/assets/b1525474-7540-4618-ad91-0ca3d1f25613" />

A diagram from the Snap-Fit Design Guide displaying the crucial geometric parameters of a cantilever snap-fit design.

<img width="407" height="327" alt="image" src="https://github.com/user-attachments/assets/f79dc0af-e505-4bb5-be6a-9852b9e99ca1" />

A plot from the same source showing the yield strength and permissible strain for a cantilever snap-fit.

<img width="902" height="622" alt="image" src="https://github.com/user-attachments/assets/ed538e00-2989-4a6b-8711-753dbe279787" />

A table of equations to solve for undercut depth for each type of type snap-fit geometry.

**SLA Resin Properties**

SLA is a polymer with high stiffness that can work well for snap fits will small deflections. It is relatively brittle and prone to snapping with beam/flexure lengths that are too short or too thick.

## Design

**Snap-Fit Type**

The clip design uses a dual cantilever beam mechanism with undercut geometry that allows it to deform and then snap into place to hold the two parts together. 

**Intended Function**

The intended function of this mechanism was to allow for two straps to be clipped together. The slots in the two parts of the clip were designed with slots to allow for these straps to be fastened to either end of the clip. The clip was designed to have a strong enough hold to be used under high load situations.

**Design Explanation**

The hook shape and undercut geometry were chosen to provide the amount of deflection that maintained stress that was within the yield stress of the material and ensuring that the clip did not require too much force to operate while still providing a strong hold. Similarly, the cross-sectional area of the flexures was designed to be the correct proportion to the length of each flexure, again, ensuring the correct amount stress and strain.

Using the table from the Snap-Fit Design Guide:

$$
y = 0.67 \cdot \frac{\epsilon \cdot l^2}{h}
$$

$$
y = 0.67 \cdot \frac{0.13 \cdot (0.5)^2}{0.125}
$$

$$
\boxed{y = 0.1742 \text{ in}}
$$

$y$ = Deflection (in)  
$\epsilon$ = Allowable Strain for Grey V5 resin (in/in)  
$l$ = Flexure length (in)  
$h$ = Flexure thickness (in)  
$0.67$ = Empirical constant

Which gave a max undercut depth of 0.1742 in. However, in order to increase the durability and increase the safety factor, the undercut was reduced to less than half: 0.07 in.

The clip was not designed for separable assembly; once the parts were clipped together, they could not be taken apart.

<img width="695" height="491" alt="image" src="https://github.com/user-attachments/assets/62dd6920-e050-4c50-9d87-d4b4f84733ec" />

<img width="362" height="545" alt="image" src="https://github.com/user-attachments/assets/ad02fbef-75e7-483d-ad8b-76f293335940" />

<img width="630" height="685" alt="image" src="https://github.com/user-attachments/assets/c983434c-46c9-4bb8-bd07-4d7a2741967e" />

<img width="605" height="627" alt="image" src="https://github.com/user-attachments/assets/17fb8c8a-9a64-40c6-88d1-78595a073514" />

<img width="517" height="542" alt="image" src="https://github.com/user-attachments/assets/1a9ecc76-1147-4540-9e0a-5c1905dc9073" />

<img width="381" height="645" alt="image" src="https://github.com/user-attachments/assets/976621eb-704f-440c-8778-c5583f3e67e2" />

<img width="612" height="450" alt="image" src="https://github.com/user-attachments/assets/14fa94fd-8347-4ef8-9b6f-b362db9ee9d7" />

<img width="585" height="416" alt="image" src="https://github.com/user-attachments/assets/6f7c8cc0-de60-4027-a403-b73a8b659bfd" />

<img width="525" height="697" alt="image" src="https://github.com/user-attachments/assets/050d57c4-3438-4853-9e04-2b39e8cb5feb" />

<img width="432" height="572" alt="image" src="https://github.com/user-attachments/assets/797ade00-f3b1-486c-8f13-c3e40f3dbc7d" />

<img width="607" height="531" alt="image" src="https://github.com/user-attachments/assets/c105b50d-db35-4be5-9321-833899183646" />

<img width="402" height="552" alt="image" src="https://github.com/user-attachments/assets/ff8f556e-4f8d-479d-97c0-784615881c73" />

<img width="420" height="612" alt="image" src="https://github.com/user-attachments/assets/ec4d09e6-56e7-4813-8d80-5f8438dcc701" />


## Preprocessing

<img width="1191" height="630" alt="image" src="https://github.com/user-attachments/assets/b26f49c9-3856-4c8b-ad49-ed3873aa0a16" />

**Machine name and resin used:** HumorousPetrel, Grey V5

**Build orientation and reasoning:** One click setup default

**Layout on the build plate (2–3 student parts per plate):** One click setup default

**Support strategy, wall thickness, and resolution settings:** One click setup default

**Whether the design is isotropic or anisotropic, and why:** isotropic due to properties of SLA

**Clearance used for the snap fit engagement:** 30 thou (0.03") for slots/flexures 

**Layer height, print time, and build volume:** 0.05 mm, 1h 49m, 20.74 ml (for both students' assemblies combined)

## Post-Processing

<img width="600" height="642" alt="image" src="https://github.com/user-attachments/assets/eb284f37-94c6-44a9-8dfd-9e543023d761" />

**Wash:** Placed in alcohol bath for preset time (10 minutes).

**Cure:** Placed in curing station for preset time (15 minutes).

**Support Removal:** Snipped with wire cutters or broken off by hand.

## Validation

The snap fit functioned well with an audible snap and a very strong engagement. In fact, it was nearly impossible to remove after being snapped together, even when using hand tools to compress the flexures. The fit was only slightly loose, with some perceptible play. Adjustments were needed such as the spacing of the slots on the side from the intended receiving end of the outer clip. This resulted in the clip working better with the strap slot cut-out opposite/upside down from how it was originally designed. Apparently 0.03" was not enough clearance for the base of the flexure to the undercut. 

After the in-lab validation, the assembly was brought home and taken apart once again to re-use. This time however, one of the flexures snapped while inserting. This was only after the clip had been used several times successfully. Unfortunately, I did not have any photos of the assembled clip before it broke.

<img width="710" height="287" alt="image" src="https://github.com/user-attachments/assets/6a3dff0f-3732-49bd-89d8-ff690bc10e9f" />

The aftermath.

## Lessons Learned



