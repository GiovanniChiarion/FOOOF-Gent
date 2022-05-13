# FOOOF-Gent
This repository is about exploiting the potentiality of FOOOF algorithm. It is organized in 2 folders: PAC and notebooks.

- PAC is about Phase Amplitude Coupling analysis. Inside this folder, the Jupyter Notebook PAC_reconstruction is a simulation of a chirp signal modulated in amplitude with a sine function (periodic component) and overlapped with a gaussian pink noise (aperiodic component). The goal is to reconstruct the original sine freuency and modulating amplitude removing the aperiodic part of the signal. For this, it is necessary to go from time domain to frequency domain (to apply FOOOF) and then going back in the time domain.

- notebooks is about modifications in the eegnb notebooks of neurotechx. In the pushed subfolder, there is the modifications I proposed and pushed in their repository. In the n170 script, in the last section I applied the FOOOF algorithm to their data and removed the aperiodic component of the power spectra. It can be seen that without FOOOF the two power peaks can be wrongly supposed to be higher for "Face" condition rather than "House", due to the aperiodic contribution. Outside the pushed folder, there are some modifications I tried to analyze data with FOOOF using FOOOFGroup  

This repository requires Python (>=3.6) and many different packages (in the list.txt there is the list of required packages)
