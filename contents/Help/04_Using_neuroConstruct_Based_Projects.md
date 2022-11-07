## Note: OSB documentation has been moved! Please see latest documentation (covering both OSBv1 and OSBv2) at: https://docs.opensourcebrain.org

A number of the projects on the OSB are based on [neuroConstruct](http://www.neuroconstruct.org/) projects (see [here](http://opensourcebrain.org/search_custom_field?f[]=43&op[43]=~&v[43][]=neuroConstruct)). neuroConstruct is used to import model elements in NeuroML (e.g. exported from a simulator or other application), can generate code for multiple simulators, and can export NeuroML in various formats.

### Install the latest version of neuroConstruct

First, get the latest version of neuroConstruct. While there are binary installers available on the neuroConstruct download page, it's best to **use the latest version of this application from GitHub**, as this will most likely be the version in which the projects on OSB were last saved.

Get the latest version of Git (see [here](http://www.opensourcebrain.org/projects/gitintro/wiki/Wiki) for more about Git). Detailed instructions for installing neuroConstruct from source can be found [here](https://github.com/NeuralEnsemble/neuroConstruct/blob/master/INSTALL.md).

### Install your simulator(s) of choice

More details on the simulators supported by OSB can be found <a href="/docs#Simulators">here</a>.

### Get a local copy of one of the neuroConstruct based projects

Check out a local copy of one of the projects, e.g. project:granulecell

    git clone https://github.com/OpenSourceBrain/GranuleCell.git

Run neuroConstruct as outlined in the installation instructions.

Go to **File**, then **Open Project…**, go to the folder you installed the project in and select **GranuleCell/neuroConstruct/GranuleCell.ncx**.
Go to tab **Generate** and press **Generate Cell Positions and Connections**.
Go to tab **Export** and then the tab for your chosen simulator (e.g. NEURON), press **Create XXX files**, then **Run XXX simulation**.
For more details on the interaction of neuroConstruct with these simulators see [here](http://www.neuroconstruct.org/docs/interact.html).

### Get all neuroConstruct based projects on OSB

To clone all of the projects on OSB which contain neuroConstruct projects (and many others) use the **checkOSB** script in the **osb** subfolder of the neuroConstruct home directory:

    cd osb
    ./checkOsb.sh -u (Linux/Mac)
    checkOsb.bat -u  (Windows)

This will clone \~70 projects with \~20 containing neuroConstruct projects, which will be accessible under the File - Open Source Brain Project:

![](/attachments/download/51/nCmenu.png)
