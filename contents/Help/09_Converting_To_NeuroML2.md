### Convert your model to NeuroML 2

Converting models to the simulator independent format [NeuroML 2](https://www.neuroml.org/neuromlv2) enables conversion of the model to [many different formats](https://www.neuroml.org/mappings), as well as enables many of the advanced features of OSB to be used with your model (e.g. [3D visualisation of cells](http://www.opensourcebrain.org/projects/l5bpyrcellhayetal2011?explorer=https%3A%2F%2Fraw.github.com%2FOpenSourceBrain%2FL5bPyrCellHayEtAl2011%2Fmaster%2FneuroConstruct%2FgeneratedNeuroML2%2FL5PC.cell.nml) & [networks](http://www.opensourcebrain.org/projects/acnet2?explorer=https%3A%2F%2Fraw.github.com%2FOpenSourceBrain%2FACnet2%2Fmaster%2FneuroConstruct%2FgeneratedNeuroML2%2FMediumNet.net.nml) and extracting information on [channel kinetics](http://www.opensourcebrain.org/projects/acnet2?explorer=https%3A%2F%2Fraw.github.com%2FOpenSourceBrain%2FACnet2%2Fmaster%2FneuroConstruct%2FgeneratedNeuroML2%2FNa_pyr.channel.nml)).

At the moment, there is no "magic button" to press in simulators to export your model into valid NeuroML 2. Presently the best approach is to look at some of the [core examples of NeuroML 2](https://github.com/NeuroML/NeuroML2/tree/master/examples), the [OSB projects being converted to NeuroML 2](https://github.com/OpenSourceBrain/redmine/issues/125), look at the XML examples there and start manual conversion of the models based on these. There are some suggestions below for work to help with this

**Use jNeuroML to validate/execute/convert the NeuroML 2 files**

[jNeuroML](https://github.com/NeuroML/jNeuroML) can be used to validate NeuroML2 files:
  
     jnml -validate MyNeuroML2.nml
     
This will validate the file against the latest XSD Schema document, as well as perfom a number of other checks on the structure of the model.
