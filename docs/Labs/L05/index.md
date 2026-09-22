# A5 – Design a Snap Fit

## Objective

The goal of this project was to design a snap fit assembly where two or more components fit together using elastic deformation.

## Analyze

**Instructions**

1. Parametrically design an assembly of two constituents which snap fit together.
2. Use parameters in CAD
3. Use constraints in CAD
4. Print the two components. On of the components needs to have support material.
5. Test the snap fit.
6. Iterate if needed.

**Constraints**

1. Safety factor of 3.5. 
2. Transverse load between .25 lbf - 5 lbf.
3. Axial load between 5 lbf - 10 lbf.
   
## Decide

I decided to design a snap connector for a gear. The concept I had in mind was a simple cylindrical pin with space between for the deformation to occur. A lip around the top would lock the gear in place. The gear would be snap fit to the base but still able to rotate.

<img width="1030" height="661" alt="image" src="https://github.com/user-attachments/assets/805718aa-2f6b-4d26-9595-ae294943a698" />

## Communicate

**Modeling**

<img width="512" height="732" alt="image" src="https://github.com/user-attachments/assets/94f5bc00-dce9-4e42-a8d0-af2c5a751826" />

First, the sketches were drawn of the rough geometry of the base of the pin. The cross sectional area in the calculations was simplified (I'll get into that later) compared to the actual geometry. 

The knowns and unknowns of the problem were stated to provide clarity and organization and were as follows:

Knowns: Yield Strength (6000 psi), Safety factor (3.5), Transverse force (21 lbf), Axial force (5 lbf-10lbf), Inner radius (0.1 in), Outer radius (0.22), Center cut length (.186 in), and Center cut width (.073 in).

Unknowns: Moment acting on each member, Second moment of inertia, Cross sectional area, Centroidal distance, and Length of the pin.

<img width="487" height="607" alt="image" src="https://github.com/user-attachments/assets/82d73342-601f-4840-909e-ed22996a992d" />

Next, the cantilever beam stress equation was used to solve for the length of the pin. I assumed each member's cross section was similar enough to a semi cylinder for that equation to be used to solve for the moment of inertia, I. The same was done for the centroidal distance, c. Once these values were found, they could be plugged into the equation and the length could be found. The result was a length of 0.16 in.

You will also notice some clearance notes I made below the bending equation. These were the clearance fits I used when deciding the hole size in the gear. More on this later.

The stress in the pin was found to be 1,678.69 psi which was less than 30% the yield strength of PLA. The stress was also below the factor of safety by a decent margin.

<img width="492" height="450" alt="image" src="https://github.com/user-attachments/assets/9950bcf1-03fd-4f9c-9a8e-96664521fc98" />

Lastly, both the axial stress and shear stress were calculated for the pin.

<img width="1700" height="645" alt="image" src="https://github.com/user-attachments/assets/6caa3eb4-b9a3-4edc-8d60-b7b4d5c0280c" />



<img width="915" height="610" alt="image" src="https://github.com/user-attachments/assets/bf1113a0-019a-48f0-894c-c1c5b4abdee6" />

<img width="1127" height="737" alt="image" src="https://github.com/user-attachments/assets/8a01bef5-2a06-4499-963e-ee63720d44cf" />

<img width="1026" height="527" alt="image" src="https://github.com/user-attachments/assets/ddd08b13-5ec7-4cf2-9595-965a3fab61df" />

<img width="1132" height="747" alt="image" src="https://github.com/user-attachments/assets/e8ef704d-656c-495e-8c2c-a8ceac2dd74c" />

<img width="1542" height="742" alt="image" src="https://github.com/user-attachments/assets/fececb24-0c33-4651-afbc-58369db0283d" />

<img width="1085" height="572" alt="image" src="https://github.com/user-attachments/assets/c642f1db-0c3d-4045-a409-675ac896edd1" />

<img width="1012" height="667" alt="image" src="https://github.com/user-attachments/assets/bf217962-7efb-482c-9dd1-6c7fd0b0ecd6" />

<img width="1461" height="685" alt="image" src="https://github.com/user-attachments/assets/87e7597e-1e83-4108-8396-976568ec6faa" />

<img width="1202" height="590" alt="image" src="https://github.com/user-attachments/assets/f9b83844-c2ac-4ef2-a866-55a655d05036" />

<img width="852" height="527" alt="image" src="https://github.com/user-attachments/assets/967c38f5-bdc8-407d-969c-cfe8db43a96e" />

<img width="722" height="552" alt="image" src="https://github.com/user-attachments/assets/0a81df12-2a22-4137-8104-fa76082de8dd" />

<img width="857" height="537" alt="image" src="https://github.com/user-attachments/assets/8b8a9ccb-0777-45aa-bc1f-4843be89fbfe" />

<img width="1917" height="800" alt="Screenshot 2026-09-21 150311" src="https://github.com/user-attachments/assets/c4b9765c-a199-490f-bc2c-b9d41252ca6f" />

<img width="1917" height="312" alt="Screenshot 2026-09-21 150322" src="https://github.com/user-attachments/assets/af18b5d1-86a9-4a58-8306-1cf0e0647406" />

<img width="1917" height="340" alt="Screenshot 2026-09-21 150337" src="https://github.com/user-attachments/assets/7a5dd4e7-cfa4-4c8a-8dcb-7a2c6f176a8a" />

<img width="1917" height="1020" alt="Screenshot 2026-09-21 150417" src="https://github.com/user-attachments/assets/c57e9fc0-7bbe-42d3-9268-44afa3d4ddbf" />

https://github.com/user-attachments/assets/e2b71f4e-0263-4920-b0db-62037d655d9b

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/da3a0a2e-4a67-4d9e-b73a-bcd0fa3e8b4d" />

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/7547eec0-4d37-4435-8326-a22274af6686" />


