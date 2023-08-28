### Add functional MRI support to InVesalius

InVesalius currently does not support the simultaneous visualization of functional and structural MRI. This task will expand the support to processed functional MRI.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. 

**Deliverables**:
- User interface to support and control fMRI parameters
- Visualization features for fMRI

**Programming Languages**: Python

**Duration**: 350h

**References**: https://github.com/invesalius/invesalius3/issues/507 and https://www.hopkinsmedicine.org/radiology/patient-information/exams-procedures/functional-mri.html


**Selected Contributor:** [Michael Chan](https://github.com/miki998) (Switzerland)

**Mentors**: 

[Victor Hugo Souza](https://github.com/vhosouza) \
[Renan Matsuda](https://github.com/rmatsuda) \
[Thiago Franco de Moraes](https://github.com/tfmoraes/) \
[Paulo Henrique Junqueira Amorim](https://github.com/paulojamorim)

**Pull requests**: https://github.com/invesalius/invesalius3/pull/658



---

### Add PACS communication

InVesalius currently does not support loading DICOM images from a PACS server. The idea is to have a way to search for images in a PACS, download the images and load the images.

**Requirements**: Computer with Windows, Linux or Mac OS installed. A source code editor, Python language and InVesalius libraries dependencies. A PACS server like [Orthanc](https://www.orthanc-server.com/) or [DCM4CHE](https://www.dcm4che.org/).

**Deliverables**:
- Tool to communicate with PACS server
- Save the surfaces and masks in the PACS

**Programming Languages**: Python

**Duration**: 350h

**References**: https://github.com/invesalius/invesalius3/issues/101 , https://gdcm.sourceforge.net/html/classgdcm_1_1CompositeNetworkFunctions.html, https://en.wikipedia.org/wiki/Picture_archiving_and_communication_system

**Selected Contributor**: [Vinícius Cavalcanti](https://github.com/hvini) (Brazil)

**Mentors**: 

[Marc Gonzalez Capdevila](https://github.com/marcgc21) \
[Karine Pistili Rodrigues](https://github.com/KarinePistili)

**Pull requests**: https://github.com/invesalius/invesalius3/pull/644
