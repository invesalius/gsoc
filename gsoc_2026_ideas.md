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

### Improvements in user response (loading and saving files)

When saving or loading files (except DICOM), InVesalius does not provide any feedback to the user. The goal of this task is to implement a window that displays the progress when loading or saving the different types of files that InVesalius handles. This task also includes replacing the progress bar of the volume rendering functionality.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background in GUI.

**Deliverables**:
- Windows with progress bar for the functionalities specified in the referenced issues (references).

**Programming Languages**: Python

**Duration**: 90h

**Difficulty level:** Easy

**Mentor:** Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

 
---

### Use Github Actions to create installers for macOS

[Github Actions](https://docs.github.com/en/actions) is used for various softwares to run tests when a commit or pull request is submitted.
Also, it can be used to compile software and create binaries ready to be used by the users.
The idea in this task is to use Github Actions to create nightly and release InVesalius installers for macOS.

**Requirements**: Computer with Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Github action to create nightly and release installers for InVesalius for macOS.

**Programming Languages**: Python

**Duration**: 175h

**Difficulty level:** Intermediate

**Mentor:** Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com and Thiago Franco de Moraes - totonixsame@gmail.com

**References**: https://docs.github.com/en/actions https://pyinstaller.org/en/stable/


---


### Simultaneous visualization and control of Two Robots for Dual Transcranial Magnetic Stimulation

Development and integration of the functionality for simultaneous control of two robots, aimed at applying dual-site Transcranial Magnetic Stimulation (TMS) in InVesalius (currently, support is provided for only one TMS coil attached to one robot). This feature is based on the existing implementation for the use of two or more coils, adapting it for multiple robots. The inclusion of this feature not only improves the speed, accuracy, and safety of the stimulatory process, but also enables the scientific exploration of interactive brain networks, by allowing concurrent, targeted TMS pulses to multiple brain areas. 

**Requirements:**
Computer with Windows, Linux, or Mac OS installed.
Python programming language and InVesalius library dependencies.
A source code editor.

**Deliverables:**
- Visualization interface showing the robots' movements integrated into the InVesalius neuronavigation system.
- Coordinate communication between the websocket data receiver, InVesalius brain targets, and GUI.
- Software module for control and synchronization of the two robots.

**Programming Languages:** Python

**Duration:** 350h

**Difficulty Level:** Hard

**Mentor:** Renan Matsuda - renan_hiroshi@hotmail.com and Thais Marchetti - thaismarchetti123@gmail.com and Lucas Betioli - lucasantoniobetioli@gmail.com and Victor Malheiro - victorhugomalheiro@gmail.com

**References**:
- Neuronavigation: [Track multiple coils simultaneously and show stylus/probe #827](https://github.com/invesalius/invesalius3/pull/827)
- Robot control: https://github.com/biomaglab/tms-robot-control 

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
