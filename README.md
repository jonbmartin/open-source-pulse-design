![banner](figures/VConference-Slider.jpg)

# Open Source RF Pulse Design Demos

This repository contains a series of interactive demos on RF Pulse Design in the form of Jupyter Notebooks. They supplement the lecture **"Open Source Pulse Design and Interactive Demonstraction"** from the ISMRM 2020 Annual Meeting's educational session **"Hands-On: Pulse Sequence & RF Pulse Design"** given by Jonathan Martin of the Grissom Lab at Vanderbilt University. 

## Exercises
This demo is split into four sets of exercises, each in their own python notebook:

1. [SLR Pulse Design](exercises/Ex1-SLR-Pulse-Design.ipynb): This notebook goes through the essentials of SLR pulse design with SigPy.
2. [Pulse Multibanding](exercises/Ex2-Multiband-Pulse-Design.ipynb): This notebook builds on the first by teaching how to multiband an SLR pulse to excite simultaneous slices and how to design a PINS multiband pulse.
3. [Adiabatic Pulse Design](exercises/Ex3-Adiabatic-Pulse-Design.ipynb): The third set of exercises focus on the design of adiabatic RF pulses for excitation and inversion.
4. [Parallel Transmission](exercises/Ex4-Parallel-Transmission.ipynb): The last notebook works through a small-tip spatial-domain pulse design for a parallel transmission system. It also provides information on some of the useful abstractions that SigPy includes, such as Linops and Algs. 


## Setup

The user has two options for running the demonstration Jupyter notebooks.

**1. Binder (recommended):** Binder is a service that provides software environments that can be opened and run in entirely in the cloud. To run the demos in the browser, click on this icon: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jonbmartin/open-source-pulse-design/master) The exercises can then be opened and run in the same manner as any other .ipynb file simply by clicking on their filenames once the environment is built, with no local installs.

**2. Locally:** To run the demos locally, the repository should be downloaded and its contents extracted. The following requirements will need to be satisfied on your device:
  - Python >= 3.5
  - sigpy >= 0.1.17 (and all dependencies e.g. scipy, numpy, installed with pip/conda). SigPy install guides are found [here](https://sigpy.readthedocs.io/en/latest/).
  - matplotlib (pip/conda)
  - jupyter notebook (pip/conda)
  
  Open the exercises in a notebook by navigating to the directory in which the repostory was installed and typing ``` jupyter notebook ``` into the terminal.
  
## Guide for the use of this notebook

The exercise folder in the repository contains four exercise .ipynb files, covering SLR, multiband, adiabatic, and pTx pulse design. These notebooks are primarily skeleton code, which the participant should fill in to complete the pulse design. Solutions are found in the solutions folder. 

The video lecture that introduces these exercises will be posted on the ISMRM website and linked to in this repository at a future date. It is recommended that you work through the exercises in parallel with the video lecture. 

The pulse designers used in this tutorial are a part of the SigPy python package. SigPy documentation is [here](https://sigpy.readthedocs.io/en/latest), the source code is [here](https://github.com/mikgroup/sigpy), and tutorials on the use of SigPy for image recon are [here](https://github.com/mikgroup/sigpy-mri-tutorial).

For additional background reading, we recommend the Handbook of MRI Pulse Sequences by Berstein, King, and Zhou (2004). It provides excellent coverage of SLR and adiabatic pulse design. 

## References 

[1] J. Martin, F. Ong, J. Ma, J. Tamir, M. Lustig, and W. Grissom, “SigPy.RF: Comprehensive Open-Source RF Pulse Design Tools for Reproducible Research”, in Proceedings of the ISMRM Annual Meeting and Exhibition, 2020, p. 1045.

