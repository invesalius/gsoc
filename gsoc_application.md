# InVesalius GSoC 2023: Guidelines and instructions #
# Before you apply #

* All projects assume familiarity with Python (and several packages). Aspiring applicants are encouraged to learn it and try to write some code.

* Carefully read the GSoC eligibility rules (see [section 7.1 of the GSoC rules](https://summerofcode.withgoogle.com/rules)).

* Choose one the [project ideas](https://github.com/invesalius/gsoc/blob/main/gsoc_2023_ideas.md). We are also open to new ideas. In this case write-to us at [invesalius@cti.gov.br](mailto:invesalius@cti.gov.br) with the subject "GSoC 2023 - New Idea".

* IMPORTANT: Remember to submit final proposals before **April 4th at 18:00 (UTC) deadline but it is important before that date to have contacted the mentor and followed the steps below**.

# Applying #

If you are interested in applying, follow these steps ASAP:

### 1. InVesalius development environment ###

1.1 - Fork InVesalius source code for your github;

1.2 - Install and run InVesalius from source code in your PC;

1.3 - Record a short video running InVesalius from source code.

* Display the terminal/command prompt by calling InVesalius and loading a sample image (there are some DICOM images here [https://invesalius.github.io/download.html](https://invesalius.github.io/download.html).

* Save in mp4 file format to upload in Google Drive (step 3).


### 2. Write a working code sample relevant for the proposed project. ###

Applicants are welcome to find and fix bugs in InVesalius core or related to some of the proposed projects. However, getting reviews can take a long time as code owners may be busy working on new features. So instead of requiring applicants to fix a good first bug, **we suggest that applicants write a working code sample relevant for the proposed project**.

The code sample can be attached to the application as a [secret gist](https://gist.github.com/) (please use secret gists, and do not share these with other applicants). Suggested ideas below include proposed "Good Sample Projects".

* Create a unit test to some methods or functions;

* Add type informations to some methods or functions;

* Create a simple plugin to apply [erosion](https://en.wikipedia.org/wiki/Erosion_(morphology)) or [dilation](https://en.wikipedia.org/wiki/Dilation_(morphology)) to the current mask;

    * [Sample plugins](https://github.com/tfmoraes/inv3_plugins_examples)

    * [Slides](https://github.com/tfmoraes/inv3_plugins_examples/blob/main/slides.html)

Do not spend too much energy on this piece of sample code, we just want to see that you can code something relevant -- and that this sample code can run and do something non-trivial. Be aware that we have a limited number of mentors available, and will only be able to accept a few applicants.



### 3. Write and share the draft proposal and other files ###

Applicants are encouraged to submit draft proposals, linking to Google Drive with permission for mentors to comment.

Introduce yourself and send the link to the mentor's email. Use as subject "GSoC 2023: Application". Use this email topic for futures discussions during the application.


The Google Drive folder should be named with the following pattern "GSoC2023_LastName_FistName" and must contain the following files:

* **proposal:** A google doc with the draft proposal;

* **resume.pdf:** A PDF file with your resume;

* **screenshot.mp4:** The screenshot video of item 1;

* **gist.txt:** A text file with a link to your secret gist of item 2.

The draft proposal should contain the topics below. Try to detail as much as possible.


* **Name and Contact Information**

* **Project Title**

* **Synopsis**

* **Benefits to Community**

* **Technical proposal**:  Provide a proposal of a technical solution with your methodology.

* **Schedule / Deliverables**: Create a schedule that you are sure you will be able to accomplish. Set checkpoints each two weeks.

* **Related Work**

* **Biographical Information**

See also the [contributor guide](https://google.github.io/gsocguides/student/writing-a-proposal) on writing a proposal.


### 4. Final submission ###

After following steps 1, 2 and 3 with your potential mentor, applications can be submitted through the [summerofcode.withgoogle.com](https://summerofcode.withgoogle.com) website starting March 20th until [April 4th at 18:00 (UTC).](https://developers.google.com/open-source/gsoc/timeline?hl=pt-br#april_4_-_1800_utc)


### 5. Cross the fingers ###

According to the [calendar](https://developers.google.com/open-source/gsoc/timeline?hl=pt-br#may_4_-_1800_utc), the result will be announced on May 4th.

Good luck!

# Questions? #

* Technical questions about running InVesalius should be asked via the [github discussions](https://github.com/invesalius/invesalius3/discussions). Remember that before starting a discussion check the previous comments and issues.

* Specific questions about your project should be addressed by email to your potential mentor.

