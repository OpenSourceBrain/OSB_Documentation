It is possible to run simulations on OSB directly from your browser

### Introduction

TODO...

### Supported simulations

Neuron on OSB, jNeuroML on OSB, and NetPyNE on OSB simulation options run on the OSB platform's own server. Limitations on the size and duration of simulations apply.

Neuron on NSG and NetPyNE on NSG run on the Neuroscience Gateway Portal. NetPyNE on NSG simulations can be run on up to 64 processors.

### Connect to Dropbox

Simulation results in HDF5 format can be automatically sent to a Dropbox App folder.

To enable this, click the "Link Dropbox…" button in the Run Experiment dialog.

You will be asked to give Geppetto access to its own folder within Dropbox. Copy and paste the code into the dialog on OSB.

![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/dropbox-auth.png)

![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/dropbox-auth2.png)

After completing this configuration, the "Upload results to Dropbox on completion" option will be checked by default in the run dialog, and results files should appear automatically in your Apps/Geppetto folder.
