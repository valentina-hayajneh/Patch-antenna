## Inset-Fed Microstrip Patch Antenna @ 2.4 GHz

## Overview

An inset-fed microstrip patch antenna is a popular antenna type used in wireless communication due to its compact size, low profile, and ease of fabrication. The inset-feed technique involves cutting a notch into the patch and feeding the signal at an optimized position within this notch. This method improves impedance matching between the patch and the feed line, compared to simple edge-feeding techniques.

This project involves the design and simulation of an inset-fed microstrip patch antenna operating at 2.4 GHz using HFSS. The design is inspired by and benchmarked against the research paper:([URL](https://www.researchgate.net/publication/379504173_Design_Of_24_GHZ_Single_Band_Inset-Fed_Rectangular_Microstrip_Patch_Antenna))

## Reference Antenna Design

The following figure shows the layout and physical parameters of the reference antenna used for benchmarking:

<img width="1411" height="573" alt="image" src="https://github.com/user-attachments/assets/ab94611d-d4cd-4755-bf62-7b90bef69f48" />

 **Figure 1**: Dimensions and layout of the benchmark inset-fed microstrip patch antenna

---

Expected results from the reference design are shown below:

<img width="1409" height="546" alt="image" src="https://github.com/user-attachments/assets/c62bb86d-8126-4c8d-9679-e86dc6257598" />

 **Figure 2**: Theoretical performance of the benchmark antenna as reported in the reference paper.
 
---
## The Designed Antenna — Geometry

The designed antenna uses the same basic structure, with dimensions derived from the reference. The patch length is 28.76 mm, width 37.97 mm, and it is centered on a substrate of dimensions 39.12 mm × 47.57 mm with a thickness of 1.6 mm. The inset feed line is 3.3 mm wide and inset by 11.12 mm, with a feed gap of 1.2 mm.

<img width="617" height="509" alt="image" src="https://github.com/user-attachments/assets/be299061-6742-45dc-8887-6858c0658882" />

 **Figure 3**: Geometry of the designed antenna.
 
 ---
## Initial Simulation Results
 **Return Loss**
 
 Return Loss (RL) is a key parameter in RF systems that measures how well power is transferred from a source (like a transmission line or feed) to a load (such as an antenna). It specifically quantifies the amount of signal reflected back due to impedance mismatches.
 
<img width="1064" height="491" alt="image" src="https://github.com/user-attachments/assets/bff5bb82-786e-4836-8bb9-5a0a0e0abb32" />

**Figure 4**: Return loss before optimization.

**VSWR**

indicates the ratio between the maximum and minimum voltage values along the line, resulting from the interference of the incident and reflected waves due to impedance mismatches.

<img width="1321" height="546" alt="image" src="https://github.com/user-attachments/assets/7c603466-7380-49ac-8efa-5934eebebb5d" />

**Figure 5**: VSWR before optimization.

We note that the initial results different from the reference. To improve performance and match the target frequency, optimization was necessary.

<img width="1404" height="499" alt="image" src="https://github.com/user-attachments/assets/94a78646-fffb-493a-b0cb-9cf15b7cb6c0" />

**Figure 6**: results from the reference

## Optimization Process

To reduce mismatch, the patch length was optimized. The optimal value was found to be between 14.38 mm and 43.14 mm, which improved matching and brought the results closer to expectations,This optimization step confirms that a patch length of **28.76 mm** yields the best impedance matching at the target frequency (2.4 GHz).

<img width="1323" height="447" alt="image" src="https://github.com/user-attachments/assets/b168e59b-dc95-4fa1-bdbb-fa3163ddde4c" />

**Figure 7**: Patch length optimization range.

---

## Final Results
***Return Loss (Final)***

<img width="1034" height="435" alt="image" src="https://github.com/user-attachments/assets/f201506d-93ff-4b70-b973-5916ffaea700" />


**Figure 8**: Final return loss result.

---
 **VSWR (Final)**

<img width="2000" height="779" alt="image" src="https://github.com/user-attachments/assets/5c406708-b976-4a7a-add6-58e50f7a70f1" />

**Figure 9**: Final VSWR.

 ***Realized Gain***

<img width="856" height="470" alt="image" src="https://github.com/user-attachments/assets/f0cdac10-6c3b-4196-bb72-47ddb32095cc" />

 **Figure 10**: Final realized gain.

 **Directivity**

<img width="1018" height="310" alt="image" src="https://github.com/user-attachments/assets/83e7f5b4-f5c5-4931-9a12-dccf67613f6d" />

**Figure 11**: Final directivity in different views.

**Comparison with Reference**
<img width="933" height="342" alt="image" src="https://github.com/user-attachments/assets/6370a9c4-98eb-4cb4-8471-ab103d103fd5" />

**Figure 12**: Final benchmark comparison.


**Despite some minor differences, the final simulated results show good alignment with the reference paper, confirming the validity of the design approach**

 
