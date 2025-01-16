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

### Real time neuronavigation motor mapping visualization

The process of transcranial magnetic stimulation neuronavigation involves the generation of motor evoked potentials (MEP), which are detected and measured using electromyography. These MEP signals can be effectively represented through a color map projected onto the brain surface. This innovative approach enables real-time visualization of brain motor mapping, offering a dynamic and comprehensive understanding of neural activity during the procedure.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. 

**Deliverables:**
- Develop pipeline to receive motor mapping data using websocket
- Projection of motor mapping data, based on the neuronavigation position, in the brain surface
- GUI to define the color map preferences and customize the number of stimuli
- Coordinate communication between the websocket data receiver, projection module, and GUI.

**Programming Languages**: Python

**Duration**: 350h

**Difficulty level:** Hard

**Mentor:** Thais Marchetti - thaismarchetti123@gmail.com / Lucas Betioli - lucasantoniobetioli@gmail.com

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

### Use Github Actions to create installers for Windows and macOS

[Github Actions](https://docs.github.com/en/actions) is used for various softwares to run tests when a commit or pull request is submitted.
Also, it can be used to compile software and create binaries ready to be used by the users.
The idea in this task is to use Github Actions to create nightly and release InVesalius installers for Windows and macOS.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Github action to create nightly and release installers for InVesalius for Windows and macOS.

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
