# GSoC 2023 Ideas for InVesalius

See also the instructions for applying [here](https://github.com/invesalius/gsoc/blob/main/gsoc_application.md).

All the current ideas for GSoC 2023 are listed bellow:


### Add unit tests to InVesalius to ease the process of adding new features

Use tools like unittest or pytest to add tests to InVesalius code. That way, when adding new features or bug fixes, you can verify that no previous code has been affected. Also run this code when committing and sending pull requests on Github.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Unit tests in InVesalius code
- Github-CI action for running tests when committing or posting a pull-request

**Programming Languages**: Python and YAML

**Duration**: 175h

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

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com


**References**: https://github.com/invesalius/invesalius3/issues/497, https://docs.python.org/3/library/typing.html and https://mypy-lang.org/

---

### Add logging and error catching tool
Tool that allows the user to activate the capture of logs and errors. It should be possible to save the sequence of events in a text file.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Graphic interface integrated to InVesalius that allows the user to activate the tool and save the logs.

**Programming Languages**:  Python

**Duration**: 350h 

**Mentor:** Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/498, https://docs.python.org/3/library/logging.html and https://realpython.com/python-logging/

---

### Support to custom shaders

Currently, InVesalius has fixed scene lighting options. Shaders allow you to manipulate part of the graphics pipeline, being able, for example, to change the color, lighting and camera of the scene. In the medical field this is useful as some regions can be better highlighted just by changing the lighting.	

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**: 
- Tool that allows loading and applying custom shaders in InVesalius rendering scenes. It is desirable that the tool displays the shader code and allows editing and applying for the user to see the changes.

**Programming Languages**: Python and GLSL

**Duration**: 175h

**Mentor:** Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/499, https://vtk.org/Wiki/Shaders_In_VTK and https://learnopengl.com/Getting-started/Shaders

---

### Implement UX principles to improve InVesalius usability

The neuronavigation feature of InVesalius currently does not follow user experience (UX) principles in the user interface and workflow design. The software usability can be significantly improved by applying the basic UX design principles.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies.

**Deliverables**:
- Description and documentation of the neuronavigation workflow
- Refactored neuronavigation user controls and settings

**Programming Languages**: Python

**Duration**: 350h

**Mentor:** Victor Hugo Souza - vhosouza@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/506

---

### Add functional MRI support to InVesalius

InVesalius currently does not support the simultaneous visualization of functional and structural MRI. This task will expand the support to processed functional MRI.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. 

**Deliverables**:
- User interface to support and control fMRI parameters
- Visualization features for fMRI

**Programming Languages**: Python

**Duration**: 350h

**Mentor:** Victor Hugo Souza - vhosouza@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/507 and https://www.hopkinsmedicine.org/radiology/patient-information/exams-procedures/functional-mri.html

---

### Add PACS communication

InVesalius currently does not support loading DICOM images from a PACS server. The idea is to have a way to search for images in a PACS, download the images and load the images.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. A PACS server like [Orthanc](https://www.orthanc-server.com/) or [DCM4CHE](https://www.dcm4che.org/).

**Deliverables**:
- Tool to communicate with PACS server
- Save the surfaces and masks in the PACS

**Programming Languages**: Python

**Duration**: 350h

**Mentor:** Thiago Franco de Moraes - totonixsame@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/101 , https://gdcm.sourceforge.net/html/classgdcm_1_1CompositeNetworkFunctions.html, https://en.wikipedia.org/wiki/Picture_archiving_and_communication_system

---

### Add scale in 2D/3D viewer

InVesalius does not have a scale on the window border of axial, coronal, sagittal and 3D/Volume views. This tool helps clinicians quickly visualize the scale of injury, organ, etc.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of geometry and computer graphics.

**Deliverables**:
- Scale in millimeters on one of the border of the four viewing windows;
- Scale numbers should change size when the user zoom in/out;

**Programming Languages**: Python

**Duration**: 175h

**Mentor:** Paulo Henrique Junqueira Amorim - paulojamorim@gmail.com

**References**: https://github.com/invesalius/invesalius3/issues/96

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

**Mentor:** Renan Matsuda – renan_hiroshi@hotmail.com

**References**: https://github.com/invesalius/invesalius3/issues/529 and https://github.com/invesalius/invesalius3/pull/242
