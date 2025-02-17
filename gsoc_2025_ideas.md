# GSoC 2025 Ideas for InVesalius

See also the instructions for applying [here](https://github.com/invesalius/gsoc/blob/main/gsoc_application.md).

All the current ideas for GSoC 2025 are listed bellow:


### Add unit tests to InVesalius to ease the process of adding new features

Use tools like unittest or pytest to add tests to InVesalius code. That way, when adding new features or bug fixes, you can verify that no previous code has been affected. Also run this code when committing and sending pull requests on Github.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Unit tests in InVesalius code
- Github-CI action for running tests when committing or posting a pull-request

**Programming Languages**: Python and YAML

**Duration**: 175h

**Difficulty level:** Intermediate

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/496 and https://realpython.com/python-testing/

---

### Add type information to functions, methods and classes in InVesalius

Since python 3.5 it is possible to add type information to the parameters of functions, methods and classes. With this information it is possible to use tools like Mypy to catch calls made with the wrong type. This way you can avoid errors and make your code easier to maintain and grow

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Type information added to InVesalius functions, methods and classes.
- Github-CI action for catching type errors using tools like Mypy

**Programming Languages**: Python and YAML

**Duration**: 175h

**Difficulty level:** Intermediate

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com


**References**: https://github.com/invesalius/invesalius3/issues/497, https://docs.python.org/3/library/typing.html and https://mypy-lang.org/

---

### Add logging and error catching tool
Tool that allows the user to activate the capture of logs and errors. It should be possible to save the sequence of events in a text file. It will be necessary to add logging capture to all functions and functionalities and their respective levels (debug, info, warn, error or critical).

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Graphic interface integrated to InVesalius that allows the user to activate the tool and save the logs.
- Log support to all InVesalius functions and functionalities.

**Programming Languages**:  Python

**Duration**: 350h 

**Difficulty level:** Hard

**Mentor:** Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/498, https://docs.python.org/3/library/logging.html and https://realpython.com/python-logging/

---


### Implement UX principles to improve InVesalius usability

The neuronavigation feature of InVesalius currently does not follow user experience (UX) principles in the user interface and workflow design. The software usability can be significantly improved by applying the basic UX design principles.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Description and documentation of the neuronavigation workflow
- Refactored neuronavigation user controls and settings

**Programming Languages**: Python

**Duration**: 350h

**Difficulty level:** Hard

**Mentor:** Victor Hugo Souza - vhosouza@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/506

---


### Performance optimization of real-time neuronavigation

The real-time neuronavigation feature of InVesalius currently works based on multi-threading using Queues, Events, and Jobs (look at [#242](https://github.com/invesalius/invesalius3/pull/242)). Optimization (utilizing the least memory, minimizing its CPU time, and offering high speed) is needed to improve neuronavigation performance.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Characterize step-by-step code execution time for neuronavigation
- Improve threads’ sleep times
- Investigate: WX GUI becomes slower when navigation is on
- Optimize 3D rendering/updating scene


**Programming Languages**: Python

**Duration**: 350h

**Difficulty level:** Hard

**Mentor:** Victor Hugo Souza - vhosouza@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/529 and https://github.com/invesalius/invesalius3/pull/242

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

### Harmonize and revamp the cross-platform user interface over MacOS, Linux, and Windows

Currently, the InVesalius interface is not properly designed for different modes (Light and Dark) mode, especially on MacOS, for example.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables:**
- Unify the color scheme to different modes (light and dark)
- Apply standard and default colors to UI components
- Adjust component sizing that are disrupted across platforms
- Introduce modern icons

**Programming Languages**: Python

**Duration**: 175h

**Difficulty level:** Intermediate

**Mentor:** Petrus Kirsten - petrus.kirsten@gmail.com / Victor Malheiro - victorhugomalheiro@gmail.com

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

### Convert from Pytorch to ONNX or Tinygrad

InVesalius uses Pytorch framework to create machine learning based segmentation. The problem is Pytorch is a very large library which makes InVesalius installer and packages very large too. Also, Pytorch has some features not used by InVesalius.
ONNX is a format to export machine learning models and a library too. Tinygrad is simple library alternative to Pytorch. Both ONNX and Tinygrad are smaller and enough to InVesalius use.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of Machine Learning and AI.

**Deliverables**:
- Conversion of tool using Pytorch to ONNX or Tinygrad.

**Programming Languages**: Python

**Duration**: 175h

**Difficulty level:** Intermediate

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com and Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

**References**: https://github.com/tinygrad/tinygrad and https://onnx.ai/

---


### Convert from Pip and Conda to UV

InVesalius uses Pip with requirements.txt. There is also a Conda environment. UV is a fast modern alternative that uses pyproject.toml and other modern Python standards and also can manage Python versions.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Conversion to UV and using documentation
- Conversion of Cython compilation to use pyproject.toml

**Programming Languages**: Python

**Duration**: 90h

**Difficulty level:** Easy

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com and Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

**References**: https://github.com/astral-sh/uv

---


### Segment brain in its subparts

Use Machine Learning (like https://deep-mi.org/research/fastsurfer/) or an atlas (like https://yalebrainatlas.github.io/YaleBrainAtlas/) or both to segment brain subparts in MRI images.
Segmentation of brain subparts in MRIs is crucial for precise targeting in Transcranial Magnetic Stimulation (TMS). It enables accurate identification of specific brain regions, ensuring stimulation is applied to the correct areas for optimal effectiveness. Proper placement of the TMS coil is essential, and with segmented MRI data, the coil’s position can be precisely aligned with the target brain regions.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of Machine Learning and AI.

**Deliverables**:
- Tool to segment brain in its subparts.
- Model weights (if used AI).

**Programming Languages**: Python

**Duration**: 350h

**Difficulty level:** hard

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com and Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com and Renan Matsuda – renan_hiroshi@hotmail.com

**References**: https://yalebrainatlas.github.io/YaleBrainAtlas/ and https://deep-mi.org/research/fastsurfer/

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
