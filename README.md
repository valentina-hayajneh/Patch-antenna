<img width="11867" height="102" alt="image" src="https://github.com/user-attachments/assets/89e02bbe-08c2-49ff-ac82-7c20fd2f2a1d" /># Inset-Fed Microstrip Patch Antenna @ 2.4 GHz

## Overview
An inset-fed microstrip patch antenna is a popular antenna type used in wireless communication due to its compact size, low profile, and ease of fabrication. The inset-feed technique involves cutting a notch into the patch and feeding the signal at an optimized position within this notch. This method improves the impedance matching between the patch and the feed line compared to simple edge-feeding techniques.
This project involves the design and simulation of an inset-fed microstrip patch antenna operating at 2.4 GHz using HFSS ,
The design is inspired by and benchmarked against the research paper(Design of 2.4 GHz Single Band Inset-Fed Rectangular Microstrip Patch Antenna)([URL](https://www.researchgate.net/publication/379504173_Design_Of_24_GHZ_Single_Band_Inset-Fed_Rectangular_Microstrip_Patch_Antenna))

## The Antenna Used for Benchmarking

The figure below shows the reference antenna layout and its physical dimensions used for benchmarking. The design includes the **substrate**, **ground plane**, **rectangular patch**, and **inset feed**.

<img width="1411" height="573" alt="image" src="https://github.com/user-attachments/assets/ab94611d-d4cd-4755-bf62-7b90bef69f48" />

 **Figure 1**: Layout and dimensional specifications of the reference antenna operating at 2.4 GHz.
---

The following performance metrics are the **expected results** of the reference inset-fed microstrip patch antenna, based on the design parameters shown earlier. These values are taken directly from the paper used for benchmarking and represent the **theoretical performance** of the antenna.

<img width="1409" height="546" alt="image" src="https://github.com/user-attachments/assets/c62bb86d-8126-4c8d-9679-e86dc6257598" />

 **Figure 2**: Expected performance of the benchmark antenna based on the reference paper.
---
## The Designed Antenna — Geometry

The rectangular microstrip patch antenna designed with a patch length of 28.76 mm and a width of 37.97 mm is centrally placed on a dielectric substrate of dimensions 39.12 mm × 47.57 mm with a thickness of 1.6 mm. The ground plane fully covers the bottom surface of the substrate, while the patch is located on the top surface. Feeding is implemented using the inset feed technique, where a microstrip line of width 3.3 mm extends into the patch by 11.12 mm to achieve proper impedance matching. A feed gap of 1.2 mm is introduced at the feeding point. 
<img width="615" height="508" alt="image" src="https://github.com/user-attachments/assets/da43c88e-d9e8-420c-8f56-348b0c5dd79f" />
> **Figure 3**: Geometry of the designed inset-fed microstrip patch antenna.

