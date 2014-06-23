Using neuroConstruct based projects
-----------------------------------

A number of the projects on the OSB are based on [neuroConstruct](http://www.neuroconstruct.org/) projects. neuroConstruct is used to import model elements in NeuroML (e.g. exported from a simulator or other application), can generate code for multiple simulators, and can export NeuroML in various formats.

### Install the latest version of neuroConstruct

First, get the latest version of neuroConstruct. While there are binary installers available on the neuroConstruct download page, it’s best to use the latest version of this application from GitHub, as this will most likely be the version in which the projects on OSB were last saved.

Get the latest version of Git (see [here](http://www.opensourcebrain.org/projects/gitintro/wiki/Wiki)). The main neuroConstruct code can be cloned locally with the command:

git clone https://github.com/NeuralEnsemble/neuroConstruct.git

After the first successful checkout, run

./updatenC.sh

on Linux/Mac, or for Windows:

updatenC.bat

in the neuroConstruct directory, as there are some NeuroML files needed that reside at the NeuroML SourceForge repository.

Running the `updatenC` command in future (as opposed to just `git pull`) will ensure a consistent set of neuroConstruct source, NeuroML files and example models.

The Java code needs to be compiled and run with the command

ant run

so install Ant too: http://ant.apache.org.

Alternatively you should be able to compile and run neuroConstruct using:

./nC.sh ~~make
./nC.sh
on Linux/Mac, or for Windows:
 nC.bat~~make
nC.bat

without Ant.

### Install your simulator(s) of choice

More details on the simulators supported by OSB can be found here: osbDoc:07_simulators.

### Get a local copy of one of the neuroConstruct based projects

Check out a local copy of one of the projects, e.g. project:granulecell

git clone https://github.com/OpenSourceBrain/GranuleCell.git

Run neuroConstruct as outlined above.

Go to **File** ~~\> **Open Project…** and select **GranuleCell/neuroConstruct/GranuleCell.ncx**.
Go to tab **Generate** and press **Generate Cell Positions and Connections**.
Go to tab **Export** and then the tab for your chosen simulator, press **Create XXX files**, then **Run XXX simulation**.
For more details on the interaction of neuroConstruct with these simulators see [here](http://www.neuroconstruct.org/docs/interact.html).

h3. Get all of the neuroConstruct based projects on OSB
To clone all of the projects on OSB which contain neuroConstruct projects use the **checkOSB** script in the **osb** subfolder of the neuroConstruct home directory:
 cd osb
./checkOsb.sh~~u (Linux/Mac)
checkOsb.bat ~~u
This will clone \~15 projects, which will be accessible under the File~~\> Open Source Brain Project:

![](/attachments/download/51/nCmenu.png)
