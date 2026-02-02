# GSoC 2026 Ideas for InVesalius

See also the instructions for applying [here](https://github.com/invesalius/gsoc/blob/main/gsoc_application.md).

All the current ideas for GSoC 2026 are listed bellow:

## DRAFT - Under update ##

---

### 3D edition of masks

User can edit a mask in InVesalius slice by slice. That is a very repetitive and error prone job. Since InVesalius has 3D visualizations, it's possible to draw over the rendering area and remove the voxels projected in the painted areas.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Tool to edit masks using projections.

**Programming Languages**: Python

**Duration**: 350h

**Difficulty level:** Hard

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/91 and https://en.wikipedia.org/wiki/3D_projection

---

### Surface texture

Add texture to a surface based on the image tissue.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Tool to set a texture to a surface.

**Programming Languages**: Python

**Duration**: 350h

**Difficulty level:** Hard

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com

**References**: https://en.wikipedia.org/wiki/Texture_mapping

---


### Extract surface using Dual contouring

InVesalius uses Marching Cubes to extract surface from volumetric images. It's interesting to have other methods like Marching Tetrahedra and Dual Contouring.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Tool to generate surfaces using other methods than Marching Cubes.

**Programming Languages**: Python and Cython

**Duration**: 350h

**Difficulty level:** Hard

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com
 
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

**Duration:** 90h

**Difficulty Level:** Medium 

**Mentor:** Renan Matsuda - renan_hiroshi@hotmail.com and Thais Marchetti - thaismarchetti123@gmail.com and Lucas Betioli - lucasantoniobetioli@gmail.com and Victor Malheiro - victorhugomalheiro@gmail.com

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

**Duration:** 175h  

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

**Duration:** 90h  

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

**Duration:** 350h  

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

**Duration:** 350h

**Difficulty Level:** Hard

**Mentor:** Victor H. Souza - vhosouza@gmail.com and Renan Matsuda - renan_hiroshi@hotmail.com and Victor Malheiro - victorhugomalheiro@gmail.com

**References**:
- Neuronavigation: [Track multiple coils simultaneously and show stylus/probe #827](https://github.com/invesalius/invesalius3/pull/827)
- tFUS: [tFUS Basics](https://doi.org/10.3389/fnhum.2021.749162)
  
---

### Adapt PACS implementation to current InVesalius

**Programming Languages:** Python

**Duration:** 

**Difficulty Level:** Medium

---

### Fix GUI inconsistencies

**Programming Languages:** Python

**Duration:** 

**Difficulty Level:** Easy

--- 

### Convert GUI from WXPython to Qt


**Programming Languages:** Python

**Duration:** 350h

**Difficulty Level:** Hard

