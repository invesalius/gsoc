# GSoC 2026 Ideas for InVesalius

See also the instructions for applying [here](https://github.com/invesalius/gsoc/blob/main/gsoc_application.md).

All the current ideas for GSoC 2026 are listed bellow:

---

### Fixes in 3D mask editing and mask preview

Fix 1 - 3D edition tools: Polygons are not removed after using the tool. https://github.com/invesalius/invesalius3/issues/1078   

Fix 2 - 3D edition tools: The “Clean Polygons” button clears the edits even when “Edit in 3D” is disabled. https://github.com/invesalius/invesalius3/issues/1079   

Fix 3 - 3D edition tools: Incorrect volume selection when it occupies the entire viewport. https://github.com/invesalius/invesalius3/issues/1084   

Fix 4 - 3D edition tools: Empty volume screen when activating 3D editing after DICOM import. https://github.com/invesalius/invesalius3/issues/1085   

Fix 5 - 3D edition tools: Incorrectly edited volume after importing a DICOM study and enabling “Edit in 3D”. https://github.com/invesalius/invesalius3/issues/1086   

Fix 6 - Mask Preview:  Volume is not updated after selecting part of the mask. https://github.com/invesalius/invesalius3/issues/1080

Fix 7 - Mask Preview: Update the volume color (in red), as in the slices, when a region is selected with "Tools -> Mask -> Select parts". https://github.com/invesalius/invesalius3/issues/1081   

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Bug fixes for the 3D mask editing and mask preview tools.

**Programming Languages**: Python

**Duration**:  175h (medium)

**Difficulty level:** Medium

**Mentor:**  
Thiago Franco de Moraes - totonixsame@gmail.com  
Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/91 and https://en.wikipedia.org/wiki/3D_projection

---

### Surface texture

Add texture to a surface based on the image tissue.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Tool to set a texture to a surface.

**Programming Languages**: Python

**Duration**: 350h (large)

**Difficulty level:** Hard

**Mentor:**  
Thiago Franco de Moraes - totonixsame@gmail.com

**References**: https://en.wikipedia.org/wiki/Texture_mapping https://doi.org/10.1080/21681163.2016.1254069

---


### Extract surface using Dual contouring

InVesalius uses Marching Cubes to extract surface from volumetric images. It's interesting to have other methods like Marching Tetrahedra and Dual Contouring.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Tool to generate surfaces using other methods than Marching Cubes.

**Programming Languages**: Python and Cython

**Duration**: 350h (large)

**Difficulty level:** Hard

**Mentor:**  
Thiago Franco de Moraes - totonixsame@gmail.com
 
**References**: https://0fps.net/2012/07/12/smooth-voxel-terrain-part-2/ https://en.wikipedia.org/wiki/Marching_tetrahedra https://en.wikipedia.org/wiki/Isosurface


---


### Importing `.nii` Masks into InVesalius

Implementation of a basic feature to import segmentation masks in **NIfTI format (.nii / .nii.gz)** into InVesalius. This allows users to load externally created masks (e.g., regions of interest) and visualize them together with existing medical image data.

**Requirements:**
Computer with Windows, Linux, or Mac OS installed.
Python programming language and InVesalius library dependencies.
A source code editor.

**Deliverables:**
- Import of `.nii` / `.nii.gz` mask files into mask lisk 
- Basic documentation  

**Programming Languages:** Python

**Duration:** 90h (small)

**Difficulty Level:** Medium 

**Mentor:**  
Renan Matsuda - renan_hiroshi@hotmail.com  
Thais Marchetti - thaismarchetti123@gmail.com  
Lucas Betioli - lucasantoniobetioli@gmail.com  
Victor Malheiro - victorhugomalheiro@gmail.com

**References**:
- Similar to import mesh: https://github.com/invesalius/invesalius3/pull/68


---



### Visualization of the Selected Marker on Image Slices

Implementation of a feature to visualize the **selected marker** on axial, sagittal, and coronal slices. When a marker is selected in the marker list or 3D view, its position is highlighted on the corresponding image slices.

This improves spatial understanding during neuronavigation tasks.

**Requirements:**  
Computer with Windows, Linux, or Mac OS installed.  
Python programming language and InVesalius library dependencies.  
A source code editor.

**Deliverables:**  
- Highlight of the selected marker on 2D slices  
- Synchronization between marker selection and slice views  
- Basic documentation  

**Programming Languages:** Python  

**Duration:** 175h (medium)

**Difficulty Level:** Medium  

**Mentor:**  
Renan Matsuda - renan_hiroshi@hotmail.com  
Thais Marchetti - thaismarchetti123@gmail.com  
Lucas Betioli - lucasantoniobetioli@gmail.com  
Victor Malheiro - victorhugomalheiro@gmail.com  

**References:**  
- Existing neuronavigation and marker visualization modules in InVesalius  

---


### Saving Timestamp for Each Created Marker

Implementation of a feature to automatically store a **timestamp (date and time)** when a marker is created. The timestamp is saved together with the marker data and can be used for later analysis and synchronization with external systems (e.g., EEG, EMG, TMS).
Backward compatibility with older marker files is required.

**Requirements:**  
Computer with Windows, Linux, or Mac OS installed.  
Python programming language and InVesalius library dependencies.  
A source code editor.

**Deliverables:**  
- Timestamp stored for each created marker  
- Timestamp saved in project and export files  
- Basic documentation  

**Programming Languages:** Python  

**Duration:** 90h (small) 

**Difficulty Level:** Low  

**Mentor:**  
Renan Matsuda - renan_hiroshi@hotmail.com  
Thais Marchetti - thaismarchetti123@gmail.com  
Lucas Betioli - lucasantoniobetioli@gmail.com  
Victor Malheiro - victorhugomalheiro@gmail.com  

**References:**  
- Existing marker save/export implementation in InVesalius  

---

### TMS-Evoked Potential (TEP) Visualization Integration in InVesalius

Implementation of a visualization module for **TMS-evoked potentials (TEPs)** within InVesalius. Initially, EEG signals containing TEP data are loaded from files and visualized alongside neuronavigation data, enabling spatial and temporal correlation between cortical activity, stimulation sites, and navigation events (e.g., markers). The software architecture must be **flexible and extensible**, allowing future integration of **real-time TMS-EEG acquisition**.

The system should support visualization of **TEP-derived metrics** (e.g., amplitude, latency, or frequency-band power such as alpha power) mapped onto the cortical surface or regions of interest over time, enabling spatiotemporal representations of brain responses to TMS. Users must be able to interact with individual signals (e.g., zoom, scale, channel selection) and adjust visualization parameters.

Basic signal processing tools should be included, such as noise filtering and moving average filters, serving as a foundation for future advanced processing.

**Requirements:**  
Computer with Windows, Linux, or Mac OS installed.  
Python programming language and InVesalius library dependencies.  
A source code editor.  
Basic knowledge of EEG, TMS, and TEP analysis.

**Deliverables:**  
- Import of EEG files containing TEP data  
- Interactive temporal visualization of EEG/TEP signals  
- Spatiotemporal mapping of TEP features onto 3D brain surfaces or ROIs  
- Basic signal processing tools (e.g., noise filters, moving average filters)  
- Temporal alignment between TMS events, neuronavigation markers, and EEG data  
- Modular and extensible codebase prepared for future real-time TMS-EEG integration  
- Technical documentation  

**Programming Languages:** Python  

**Duration:** 350h (large) 

**Difficulty Level:** Very Hard  

**Mentor:**  
Renan Matsuda - renan_hiroshi@hotmail.com  
Marcio Campos - marcio.campos6@gmail.com  
Lucas Betioli - lucasantoniobetioli@gmail.com  

**References:**  
- https://mne.tools/stable/_images/sphx_glr_30_ecog_003.png
- https://www.fieldtriptoolbox.org/tutorial/tms/tms-eeg/
- http://www.tmseeg.com/tutorials/

---

### Implement neuronavigation capability for transcranial focused ultrasound (tFUS)

Development and integration of the functionality for neuronavigation of transcranial focused ultrasound transducers (tFUS). InVesalius currently supports only neuronavigation for Transcranial Magnetic Stimulation (TMS) coils. We aim at extending the support to tFUS, which is becoming an important neuromodulation tool to study and and interact with brain function non-invasively. This new feature will significantly extend the user based on InVesalius to support accurate and reproducible neuroscience. 

**Requirements:**
Computer with Windows, Linux, or Mac OS installed.
Python programming language and InVesalius library dependencies.
A source code editor.

**Deliverables:**
- Visualization interface for coregistration of tFUS transducers.
- Targeting and guiding interface for tFUS.
- Minor adjustment to UI/UX considering the tFUS user requirements.

**Programming Languages:** Python

**Duration:** 350h (large)

**Difficulty Level:** Hard

**Mentor:**  
Victor H. Souza - vhosouza@gmail.com  
Renan Matsuda - renan_hiroshi@hotmail.com  
Victor Malheiro - victorhugomalheiro@gmail.com

**References**:
- Neuronavigation: [Track multiple coils simultaneously and show stylus/probe #827](https://github.com/invesalius/invesalius3/pull/827)
- tFUS: [tFUS Basics](https://doi.org/10.3389/fnhum.2021.749162)
  
---

### Adapt PACS implementation to current InVesalius

There is a pull request (https://github.com/invesalius/invesalius3/pull/644) for the PACS tool that requires updates in order to be merged. The tool also needs more testing on servers such as DCM4CHEE and Orthanc. This activity will focus on code fixes to enable the merge and on testing the interaction between InVesalius (client) and PACS servers for DICOM send, retrieve, and query operations.

**Requirements:** 
Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. A PACS server like Orthanc or DCM4CHE.

**Deliverables:**
A tool capable of sending, retrieving, and querying DICOM data on PACS servers.

**Programming Languages:** Python

**Duration:** 175h (medium)

**Difficulty Level:** Medium

**Mentor:**  
Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com  
Thiago Franco de Moraes - totonixsame@gmail.com

---
<!--
### Fix GUI inconsistencies

**Programming Languages:** Python

**Duration:** 

**Difficulty Level:** Easy

--- 

### Convert GUI from WXPython to Qt


**Programming Languages:** Python

**Duration:** 350h

**Difficulty Level:** Hard-->
