# Rear Sprocket FEA and Topology Optimization
## Overview
One of the projects I completed for the Formula SAE team was the FEA and topology optimization (top op) of 
the rear sprocket of the drivetrain module. The goal of this optimization was to reduce the mass of the sprocket by 30%
while maintaining a safety factor of at least 2.

## Assumptions and Constraints
Based on the calculations made from my peers the sprocket was assumed to be subject to an axial force of 3,250N 
and a torque of 400 Nm. Furthermore, the bolt holes around the inner diameter of the sprocket were constrained
to displace only in the axial direction (no radial displacement). The image below shows the system of forces acting
on the sprocket. It can be noted that the image shows the already optimized sprocket but serves only to demonstrate the forces.

<img width="460" alt="Forces" src="https://github.com/user-attachments/assets/9b1f6a29-af35-406b-84d3-de0d420ab5e7" />


## Initial Sprocket
The pilot sprocket used is made of 6061 Aluminum alloy which remains the same throughout the FEA and top op.
An initial analysis was conducted where the stresses in the sprocket were determined and can be seen in the image below.

<img width="460" alt="RearSprocket_FEA Static Pre Op" src="https://github.com/user-attachments/assets/556d47da-ca2f-4284-afa2-88dcd55c2d86" />

The FEA conducted on the initial sprocket allowed to determine which areas presented the highest local stress.
As seen in the image, most of the stress was located around the bolt holes. 

## Optimized Sprocket
Using the information gathered from the initial analysis and through researching various sprocket cutout methods 
the shape of the cutouts necessary to attain our mass reduction goal was determined. Unfortunately,
SOLIDWORKS built-in topology optimization performs rather poorly at high computing times but by trial and error
our goal was obtained. I conducted multiple analyses on various cutout shapes and determined the most effective to be filleted
equilateral triangular shapes which are seen in the image below. 

<img width="460" alt="RearSprocket_Model.Post.Op" src="https://github.com/user-attachments/assets/0aceb232-d5ee-4b51-aafa-0e227cbf6e96" />

Furthermore, the FEA analysis was performed once again on the 
optimized sprocket and yielded the results seen below.
It can be noted that even though the stresses are almost double that of the sprocket before the cutouts were made, they are still well below the yield strength of the material and by a safety factor of at least 3.8.

<img width="460" alt="Rear.Sprocket.Top-Op" src="https://github.com/user-attachments/assets/73bbdd7e-bb65-4796-8625-115ef946d2f7"/>


