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
---
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

To improve impedance matching and reduce reflection losses, a parametric sweep of the patch length was performed. The patch length was varied from 14.38 mm to 43.14 mm, and the return loss at the target frequency of 2.4 GHz was monitored.

The simulation results indicated that a patch length of 28.76 mm provided the best impedance matching, achieving the lowest return loss ,This confirms that 28.76 mm is the optimal patch length for the target frequency in the current design environment and substrate configuration.

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

## Summary

The designed inset-fed microstrip patch antenna operating at 2.4 GHz successfully meets the performance expectations based on the benchmark reference. The optimization process, especially adjusting the patch length, significantly improved the impedance matching and overall antenna performance.Since  minor differences in gain and frequency offset are within acceptable limits, confirming the validity of the design methodology used in this project.

---
## Center-Inset Rectangular Microstrip Patch Antenna for 2.4 GHz


## Overview

This section presents the independent design and simulation of a rectangular microstrip patch antenna with inset feeding, operating at a target frequency of 2.4 GHz. The antenna is excited through a microstrip transmission line inset into the patch, which provides improved impedance matching compared to conventional edge feeding.

Inset-fed rectangular patch antennas are widely employed in modern wireless communication systems due to their planar profile, low cost, and ease of fabrication. By adjusting the inset position, the input impedance can be finely tuned, minimizing reflection and enhancing overall antenna performance.

---
## Antenna Geometry
The proposed antenna is a rectangular microstrip patch designed to operate at 2.4 GHz. The patch dimensions are 38.04 mm × 29.59 mm, printed on a dielectric substrate of thickness 1.6 mm with a copper cladding of 0.035 mm. The overall length of the structure is approximately equal to the free-space wavelength (λ ≈ 124.91 mm).

The antenna is excited using a microstrip transmission line with an inset feed, positioned 2 mm from the patch edge along the X-axis and 0.5 mm along the Y-axis, with an inset depth of 7 mm. This feeding technique enables fine-tuning of the input impedance for better matching.

To ensure accurate resonance at the target frequency, the patch dimensions were optimized using a correction factor of 0.93, which accounts for fringing effects and the effective dielectric constant of the substrate.


<img width="602" height="557" alt="image" src="https://github.com/user-attachments/assets/005136a3-95b2-4172-9b15-db4304a505a8" />

**Figure 1**:  Geometry of the designed antenna

---
## Return Loss

The return loss plot shows a clear resonance at approximately 2.4 GHz, with a -10 dB bandwidth ranging from 2.334 GHz to 2.430 GHz, indicating good impedance matching within this frequency range.

<img width="1320" height="563" alt="image" src="https://github.com/user-attachments/assets/b178088f-b879-4d74-b7c7-0f8ebc8340ee" />

**Figure 2**: Return loss of the designed antenna 

---
## VSWR

<img width="1774" height="735" alt="image" src="https://github.com/user-attachments/assets/87945a45-0833-4ab6-be9a-e29af3cb330f" />

**Figure 3**: VSWR of the designed antenna 

---
## Realized Gain 

The plot shows a maximum gain of 5.58 dB, with a typical directional pattern, indicating effective radiation in the broadside direction.

<img width="1178" height="747" alt="image" src="https://github.com/user-attachments/assets/07540d3d-2c77-45b6-9f78-2a33d16e47d3" />

**Figure 4**: Realized Gain of the designed antenna 

## Summary  
The proposed center-inset rectangular microstrip patch antenna resonates at 2.4 GHz with a −10 dB impedance bandwidth spanning approximately 2.334–2.430 GHz. The design achieves a peak realized gain of 5.58 dBi and maintains VSWR below 2 across the operating band, indicating satisfactory impedance matching and radiation performance for typical ISM-band applications. The inset feed and applied correction factor (0.93) effectively compensate for fringing effects and substrate dispersion. Minor discrepancies with the benchmark reference are attributable to substrate property variations and ground-plane dimensions; these can be further reduced through tolerance analysis and feed-position optimization.
