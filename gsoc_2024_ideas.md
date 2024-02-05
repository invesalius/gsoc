# GSoC 2024 Ideas for InVesalius

See also the instructions for applying [here](https://github.com/invesalius/gsoc/blob/main/gsoc_application.md).

All the current ideas for GSoC 2024 are listed bellow:


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

**Mentor:** TBA

**References**: https://github.com/invesalius/invesalius3/issues/529 and https://github.com/invesalius/invesalius3/pull/242

---

### 3D edition of masks

User can edit a mask in InVesalius slice by slice. That is a very repetitive and error prone job. Since InVesalius has 3D visualizations, it's possible to draw over the rendering area and remove the voxels projected in the painted areas.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. Good background of computer graphics.

**Deliverables**:
- Tool to edit masks using projections.

**Programming Languages**: Python

**Duration**: 350h

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

**Mentor:** TBA

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

**Mentor:** TBA

