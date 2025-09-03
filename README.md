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
<h2>The Designed Antenna — Geometry</h2>

<div style="display: flex; align-items: flex-start; gap: 20px;">
  <div style="flex: 1;">
    <p>
      The rectangular microstrip patch antenna designed with a patch length of 28.76 mm and a width of 37.97 mm is centrally placed on a dielectric substrate of dimensions 39.12 mm × 47.57 mm with a thickness of 1.6 mm. The ground plane fully covers the bottom surface of the substrate, while the patch is located on the top surface. Feeding is implemented using the inset feed technique, where a microstrip line of width 3.3 mm extends into the patch by 11.12 mm to achieve proper impedance matching. A feed gap of 1.2 mm is introduced at the feeding point.
    </p>
  </div>
  <div style="flex: 1;">
    <img src="https://github.com/user-attachments/assets/da43c88e-d9e8-420c-8f56-348b0c5dd79f" alt="Designed Antenna" width="100%">
  </div>
</div>

<p><strong>Figure 3:</strong> Geometry of the designed inset-fed microstrip patch antenna</p>

 ---
 The antenna designed according to the above requirements ,the results as follows:
 **Return Loss**
 
<img width="1064" height="491" alt="image" src="https://github.com/user-attachments/assets/bff5bb82-786e-4836-8bb9-5a0a0e0abb32" />

**Figure 4**: Return loss of designed inset-fed microstrip patch antenna
**VSWR**
<img width="1321" height="546" alt="image" src="https://github.com/user-attachments/assets/7c603466-7380-49ac-8efa-5934eebebb5d" />

**Figure 5**: VSWR of designed inset-fed microstrip patch antenna

We note that the obtained results different  from those presented in the reference paper used for benchmarking

<img width="1404" height="499" alt="image" src="https://github.com/user-attachments/assets/94a78646-fffb-493a-b0cb-9cf15b7cb6c0" />

To solve this difference, we performed an optimization process on the patch length (patchl). The optimization was carried out to minimize the mismatch between the simulated and the desired performance at the operating frequency. As a result, the optimal value of patchl was determined to be in the range of 14.38 mm to 43.14 mm. This adjustment improved the antenna performance and aligned the simulated results more closely with the target specifications.
<img width="1323" height="447" alt="image" src="https://github.com/user-attachments/assets/b168e59b-dc95-4fa1-bdbb-fa3163ddde4c" />

## The Designed Antenna — final results -Return Loss
The antenna shows a return loss of -26.03 dB at 2.418 GHz, indicating excellent matching. The (-10) dB bandwidth is 66.5 MHz

<img width="1165" height="750" alt="image" src="https://github.com/user-attachments/assets/4b6997ae-54f3-4ebe-acb9-5ccd082d7020" />
---
 ***The Designed Antenna — final results -VSWR***

<img width="2000" height="779" alt="image" src="https://github.com/user-attachments/assets/5c406708-b976-4a7a-add6-58e50f7a70f1" />

 ***The Designed Antenna — final results -Realized Gain***

 <img width="866" height="522" alt="image" src="https://github.com/user-attachments/assets/b7501362-2970-4197-b93f-16349c353009" />

 ***The Designed Antenna — final results -Directivity***
 <img width="909" height="490" alt="image" src="https://github.com/user-attachments/assets/6e5c92dd-0ce5-4621-9a07-e97652d6858c" /> <img width="1004" height="495" alt="image" src="https://github.com/user-attachments/assets/a6da2faa-1b49-44ec-92e4-70fee9738b64" />


***The Designed Antenna — Benchmark***
<img width="933" height="342" alt="image" src="https://github.com/user-attachments/assets/6370a9c4-98eb-4cb4-8471-ab103d103fd5" />



 
