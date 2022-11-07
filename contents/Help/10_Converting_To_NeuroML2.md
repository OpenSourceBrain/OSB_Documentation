## Note: OSB documentation has been moved! Please see latest documentation (covering both OSBv1 and OSBv2) at: https://docs.opensourcebrain.org

### Why should you convert your model to NeuroML 2?

Converting models to the simulator independent format [NeuroML 2](https://www.neuroml.org/neuromlv2) enables conversion of the model to [many different formats](https://www.neuroml.org/mappings), as well as enables many of the advanced features of OSB to be used with your model (e.g. [3D visualisation of cells](http://www.opensourcebrain.org/projects/l5bpyrcellhayetal2011?explorer=https%3A%2F%2Fraw.github.com%2FOpenSourceBrain%2FL5bPyrCellHayEtAl2011%2Fmaster%2FneuroConstruct%2FgeneratedNeuroML2%2FL5PC.cell.nml) & [networks](http://www.opensourcebrain.org/projects/acnet2?explorer=https%3A%2F%2Fraw.github.com%2FOpenSourceBrain%2FACnet2%2Fmaster%2FneuroConstruct%2FgeneratedNeuroML2%2FMediumNet.net.nml) and extracting information on [channel kinetics](http://www.opensourcebrain.org/projects/acnet2?explorer=https%3A%2F%2Fraw.github.com%2FOpenSourceBrain%2FACnet2%2Fmaster%2FneuroConstruct%2FgeneratedNeuroML2%2FNa_pyr.channel.nml)).

![OSB features](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/OSBfeatures.jpg)

At the moment, there is no "magic button" to press in simulators to export your model into valid NeuroML 2. Presently the best approach is to look at some of the [core examples of NeuroML 2](https://github.com/NeuroML/NeuroML2/tree/master/examples), the [OSB projects being converted to NeuroML 2](https://github.com/OpenSourceBrain/redmine/issues/125), look at the XML examples there and start manual conversion of the models based on these.

**There is a step by step guide: _Converting conductance based cell models to NeuroML2_ under development [here](https://docs.google.com/document/d/12x-iAIKJuW4P3OY46Kj15eckWO61_iBwlJ3Kmzxd5VU/edit)!**

There are some suggestions below for tools to use in this process.

**Use jNeuroML to validate/execute/convert/view the NeuroML 2 files**

[jNeuroML](https://github.com/NeuroML/jNeuroML) can be used to validate NeuroML2 files:

     jnml -validate MyNeuroML2.nml

This will validate the file against the latest XSD Schema document, as well as perfom a number of other checks on the structure of the model.

Creating a LEMS simulation file to specify how long to run the simulation, timestep, what to plot/save etc. allows the model to be run with jNeuroML. See examples [here](https://github.com/NeuroML/NeuroML2/tree/master/LEMSexamples) and most of [these OSB projects](https://github.com/OpenSourceBrain/redmine/issues/125) have at least one LEMS simulation file too.

To quickly visualise cells and networks in NeuroML 2 (as opposed to loading them in neuroConstruct or viewing on OSB), models can be converted to SVG format (for viewing in a web browser etc.):

     jnml MyNeuron.cell.nml -svg
     jnml MyCircuit.net.nml -svg

Installing the **latest development version from source** as outlined [here](https://github.com/NeuroML/jNeuroML/blob/master/README.md) is **highly recommended** to get the latest features of jNeuroML.

**Use pyNeuroML to export NeuroML2 morphologies from NEURON**

Work in progress: [pyNeuroML](https://github.com/NeuroML/pyNeuroML) is a Python package which makes many of the features of [jNeuroML](https://github.com/NeuroML/jNeuroML) accessible in Python scrips by bundling the jNeuroML jar file and using the functionality of that package.

In addition to jNeuroML features, pyNeuroML adds a number of Python specific features, including an updated exporter from NEURON into NeuroML2. This is currently limited to exporting just neuronal morphologies (see example [here](https://github.com/NeuroML/pyNeuroML/blob/master/examples/export_neuroml2.py)) but will be developed further to allow extraction of other features such as connectivity (and generation of templates in NeuroML2 for channels, synapses etc.).

This feature was used to extract a number of cell models from the original NEURON code in a [3D olfactory bulb model](http://www.opensourcebrain.org/projects/miglioreetal14_olfactorybulb3d) (see [this script](https://github.com/OpenSourceBrain/MiglioreEtAl14_OlfactoryBulb3D/blob/master/NeuroML2/export_mitral.py)).

![30 cells](https://raw.githubusercontent.com/OpenSourceBrain/MiglioreEtAl14_OlfactoryBulb3D/master/images/30cells.jpg)

**Use pyNeuroML to help convert channels to NeuroML 2**

Another feature being worked on is a set of scripts to help conversion of ion channel models (e.g. in NEURON's NMODL format) to NeuroML 2. These scripts can be accessed after pyNeuroML is installed using:

    pynml-channelanalysis NaConductance.channel.nml   # Analyse a NeuroML 2 channel
    pynml-modchananalysis NaConductance               # Analyse a NEURON channel e.g. from NaConductance.mod

These scripts, while they take different approaches to generating the traces for activation/inactivation variables, produce comparable plots:

![pynml](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/pynml_analyse.png)

On the left are the plots produced from the NeuroML file (e.g. see [here](https://github.com/NeuroML/pyNeuroML/blob/master/examples/analyseNaNml2.sh)) and on the right from the NMODL version (see [here](https://github.com/NeuroML/pyNeuroML/blob/master/examples/analyseNaMod.sh)).

To be clear, these scripts don't (currently) help you extract the equations from the NMODL file and put them in the correct place in the NeuroML file, they just help comparing the behaviour of the 2 channel formats to check for errors in a manual conversion.


**Use neuroConstruct to help conversion to NeuroML v1/2**

Many projects on OSB were originally converted from the original format (NEURON, GENESIS, etc.) to NeuroML v1.8.1 using neuroConstruct (see [here](http://www.opensourcebrain.org/search_custom_field?f[]=43&op[43]=~&v[43][]=neuroConstruct) for a list of these), and from there the conversion to NeuroML2 inside neuroConstruct was straightforward. More on using neuroConstruct [here](http://www.opensourcebrain.org/docs#Using_neuroConstruct_Based_Projects) and details on conversion of models to NeuroML v1 [here](http://www.neuroconstruct.org/docs/importneuron.html#Converting+mod+file%2FGENESIS+script+channels+into+ChannelML).
