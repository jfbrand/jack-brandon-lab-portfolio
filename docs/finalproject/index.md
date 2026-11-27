# Final Project – Water Bottle Holder

## Objectives

The goal of this project is to select a real-world problem that you, a friend, or a family member personally experience and refine your prototype design to address it.

# Part 1

## Research

**Spiral Design Process:**

Planning: The spiral process begins with requirements and planning as well as risks.

Risk Analysis: Closely tied to the planning stage. The risk increases with an increase in interfaces, for example; mechanical-mechanical, mechanical-electrical, mechanical-human.

Engineering: Uses incremental, iterative, and evolutionary design methods.

Evaluation: important that the product passes stakeholder approval. There are limitations to how much R&D can be economically feasible once the product is marketable.

Explain how this process can guide your own project iteration and improvement.

Source: https://incose.onlinelibrary.wiley.com/doi/10.1002/sys.70003

**FDM anisotropic:**
Investigate how the Fused Deposition Modeling (FDM) process inherently produces anisotropic parts. Document how this anisotropy may influence the performance and design of your prototype. Additionally, explore strategies to either leverage this behavior to your advantage or mitigate its limitations through design decisions, material selection, or process parameters.

FDM is inherently anisotropic because of the weakness in the z-axis when compared to the x and y. This is due to the way that FDM printing works, which is each part is printed layer by layer. These layers are not ideally welded together because the previous layer is cooler than each subsequent one. This can cause the layers to separate or crack at these interfaces.

In the case of my prototype this will not be an issue. The forces will be mostly pushing perpendicular to the welded interfaces not parallel. This means that the risk of shear forces delaminating those layers is extremely low. Second, the clip which will have more more forces applied to it through bending, will be isotropic since it will SLA printed instead.

Source: https://rapidmade.com/isotropic-vs-anisotropic-strength-in-3d-printing/

**SLA Shrinkage:

Resin printer tends to be very accurate at +/- 0.05-0.15 mm. However, shrinkage is still a concern. It can vary based on which resin is being used but shrinkage in resin prints tends to be roughly 7-11%. This has to be taken into account when designing parts or assemblies that require a high degree of accuracy.  

Given that the body will be FDM printed and the clip being inserted will be SLA, the shrinkage factor should not create any issues. If the clip is slightly smaller than designed, it will still likely snap into the body without issue. The main concern will be getting a tight fit that does not have too much play or slop.

Source: https://www.3dmag.com/3d-wikipedia/resin-printing-sla-uv-resin-technology-guide/

## Problem Definition

**"I cant get every bit of toothpaste out of the tube"**

The difficult task of trying to squeeze the last bit of toothpaste out of the tube. This effects almost everyone and could be solved with a few different mechanisms.

**"I need to seal a bag chips that I opened"**

That annoying bag of chips that you cant reseal. Again, this is a very common problem that can be solved relatively easily.

**"I don't have large enough cupholders in my car for my water bottle"**

Depending on the size of water bottle and cupholders in your car, it can be difficult to find a place to put it, causing it to roll around while driving. This is an issue that I have run into personally. It can be especially frustrating when in a hurry and trying to stay hydrated throughout the day.

## Problem Selection

**Water Bottle Holder**

I will be choosing this problem due to my own personal desire to have a solution and the fact that the other two ideas seems to be less unique. This problem can be solved using a simple hanging or clip-on water bottle holder that is made out of 3D printed and SLA resin parts. It will hold the water bottle in place using a bottle holder and then use a clip piece to hang or clip onto either a door pocket or cupholders in center console of your car. Due to material limitations I will be printing the main body out of PLA and the snap on clip will be made of SLA.

## Concept Development

<img width="806" height="642" alt="image" src="https://github.com/user-attachments/assets/4ecd6a99-35ef-4ba1-a1c7-e2c63e99842d" />

The rough sketch showing the basic assembly. Note, the clip will be a separate part and will be made from SLA. It will be snap fit to the main body holding the water bottle which will be printed from PLA. 

<img width="615" height="640" alt="image" src="https://github.com/user-attachments/assets/e38c0b59-4ae5-46d2-aead-2e1f7c441dea" />

The rough model of the main body/water bottle holder. This will be printed from PLA. Thickness of the walls may be adjusted for strength and changes may need to be made for the snap fit cutout on the side.

<img width="367" height="707" alt="image" src="https://github.com/user-attachments/assets/06cfc3e4-80e2-4c9d-b171-8fce78f0dde1" />

The rough model of the clip. Note, the dimensions are subject to change after testing of the critical features of the snap fit.

<img width="635" height="642" alt="image" src="https://github.com/user-attachments/assets/3aaefbc1-01d7-4988-9c2c-bc3440bdb4fa" />

The full assembly.

## Testing Critical Features

The basic design of the snap fit was tested last week with the SLA snap fit project. This design will be implementing a very similar mechanism, albeit optimized for this purpose. The tolerances will be adjusted accordingly.

## Video Presentation

[![Watch the video here](assets/thumbnail.png)](https://drive.google.com/file/d/12mq3tQVJX0H_7B8eB8Z0kJVVTYCM1DMI/view?usp=sharing)

# Part 2

## Peer Feedback

<img width="820" height="1078" alt="Screenshot 2026-11-27 171159" src="https://github.com/user-attachments/assets/116dce1f-7b04-477b-b7fa-92b6bd59ad99" />

<img width="828" height="432" alt="Screenshot 2026-11-27 171218" src="https://github.com/user-attachments/assets/1261777a-9cdf-4963-b17f-f5634cea6c90" />

James' feedback was positive overall. He did suggest that I ensure that the snap-fit is strong enough to withstand bumps in the car. I will double check my calculations and dimensions before the final print, using the formulas we learned in lab 11.

<img width="802" height="1078" alt="Screenshot 2026-11-27 171227" src="https://github.com/user-attachments/assets/f676a476-2cb0-4e9d-944e-42ab5647205c" />

<img width="820" height="425" alt="Screenshot 2026-11-27 171240" src="https://github.com/user-attachments/assets/f0a3d87e-863c-402f-95c0-74401e187273" />

Andy's feedback was similar to James'. He was concerned about the strength of the snap-fit. The reflection for James' feedback also applies here.

<img width="807" height="1078" alt="Screenshot 2026-11-27 171252" src="https://github.com/user-attachments/assets/256268a3-0665-4391-9ed7-a375e40ee6cc" />

<img width="820" height="437" alt="Screenshot 2026-11-27 171304" src="https://github.com/user-attachments/assets/eab237e0-6e51-418a-83a8-a392694f8b9e" />

Juan's feedback was helpful. I agree with him that PETG would likely be a better material than PLA for dealing with the heat of a car interior. His suggestion about the clip was also insightful.

## Refinement

<img width="382" height="686" alt="image" src="https://github.com/user-attachments/assets/ab97866b-04fa-4f5f-ba1d-084b3fbd174e" />

<img width="550" height="555" alt="image" src="https://github.com/user-attachments/assets/af28d2b6-679c-4dab-858a-f892cde18bbe" />

The changes made from the first design were the following: adjustments to flexure length (for more flexibility/less risk of snapping) as well as widening the overall clip. These changes provide more strength and less risk of the snap-fit breaking during assembly. I would have liked to print in PETG instead of PLA but time and resource constraints did not permit. I would have also liked to refine the clip geometry further but saw the the design as functional, if not ideal.

## Documentation

<img width="481" height="640" alt="image" src="https://github.com/user-attachments/assets/2d8bdac5-ad9b-4efe-a78b-67c54d6d5ad2" />

After printing, the two components look as shown.

<img width="481" height="640" alt="image" src="https://github.com/user-attachments/assets/87c6d62d-a09f-4ea6-95bd-513dcfe1c1d8" />

The two components snap together as shown. There should be minimal play between the two components and the snap fit should have a strong hold.

<img width="481" height="640" alt="image" src="https://github.com/user-attachments/assets/b3ecc5bf-160a-42e0-a91f-921a10bdd92a" />

Once assembled, the bottle holder can be hung from any door pocket or cupholder that is close to an edge. Note: taller water bottles such as the one shown may have a high center of gravity and might be prone to falling over.

## Presentation Preparation

Link: https://docs.google.com/presentation/d/1k2Uio-MkJJX3TpT5PCZoaVYtbyGFMAuK/edit?usp=sharing&ouid=104710962502719169914&rtpof=true&sd=true

## Parametric Design

<img width="716" height="607" alt="image" src="https://github.com/user-attachments/assets/3666db57-641b-42aa-8d66-7fd32d476236" />

## Final Video

[![Watch the video here](assets/thumbnail.png)](https://drive.google.com/file/d/1OA_qkcrEr-kdB8dFP7a8xzMIU0iEmhos/view?usp=sharing)
