An overview of the main target simulators for models in OSB
-----------------------------------------------------------

**Note: not all simulators will be able to execute all models.** See [here](/status) for more information.

For more tools (e.g. for visualization, analysis of models) which can handle the NeuroML elements of the models on OSB see [here](http://www.neuroml.org/tool_support.php).

### Brian

Brian is available for download [here](http://briansimulator.org).

Brian is currently supported through conversion of NeuroML models to [PyNN](http://neuralensemble.org/trac/PyNN).

Greater native support for Brian is in development in [NeuroML v2.0](http:///www.neuroml.org/neuroml2).

### GENESIS 2

GENESIS 2 is available for download [here](http://genesis-sim.org/project/genesis).

Support for running NeuroML models on GENESIS 2 is mainly enabled through generation of scripts by [neuroConstruct](http://www.opensourcebrain.org/projects/neuroconstructprojects/wiki/Wiki), but see also [here](http://www.neuroml.org/tool_support.php#GENESIS).

### GENESIS 3/Neurospaces

GENESIS 3/Neurospaces are available [here](http://neurospaces.sourceforge.net).

GENESIS 3 currently supports native reading of passive models in NeuroML format (morphology + passive parameters).

Participants at the recent [Workshop on Multi-Scale Modeling in Computational Neuroscience with GENESIS 3](http://www.gradschool.uni-luebeck.de/index.php?id=377) reported some success running neuroConstruct generated GENESIS 2 scripts on GENESIS 3.

### MOOSE

MOOSE is available [here](http://moose.sourceforge.net).

Native support for NeuroML in MOOSE is in active development, but [neuroConstruct](http://www.opensourcebrain.org/projects/neuroconstructprojects/wiki/Wiki) can also be used to generate MOOSE code from NeuroML models.

Follow the latest developments in MOOSE [here](http://moose.svn.sourceforge.net/viewvc/moose/moose).

[Moogli](http://moose.ncbs.res.in/moogli/) is a sister project of MOOSE and is a simulator independent OpenGL based visualization tool for neural simulations.

### NEURON

NEURON is available [here](http://www.neuron.yale.edu/neuron).

There is native support for reading/writing NeuroML cells in NEURON, see [here](http://www.neuroml.org/neuron_tools.php).

[neuroConstruct](http://www.opensourcebrain.org/projects/neuroconstructprojects/wiki/Wiki) can also be used to generate NEURON code (including Parallel NEURON) from NeuroML models.

### NEST

NEST is available for download [here](http://www.nest-initiative.org).

NEST is currently supported through conversion of NeuroML models to [PyNN](http://neuralensemble.org/trac/PyNN). Greater native support for NEST is planned in [NeuroML v2.0](http:///www.neuroml.org/neuroml2).

### PSICS

PSICS is available [here](http://www.psics.org).

There is some [native support](http://www.psics.org/neuroml/index.html) for NeuroML in PSICS, but [neuroConstruct](http://www.opensourcebrain.org/projects/neuroconstructprojects/wiki/Wiki) can also be used to generate PSICS code from NeuroML models.
