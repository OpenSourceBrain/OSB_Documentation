
### What is the motivation behind the Open Source Brain repository?

There are an increasing number of detailed single neuron and network models from various brain regions becoming available which encapsulate the latest data on anatomical and electrophysiological properties of the systems being investigated (e.g. on [ModelDB](http://senselab.med.yale.edu/ModelDB/default.asp*)). These complex models take a long time to develop and are normally only available in one of many incompatible, simulator specific formats.

The Open Source Brain repository (OSB) is a public repository for detailed neuronal models in standardised formats, with curated, stable releases which will evolve in line with new experimental findings, the latest modelling paradigms and simulator technology development. Anyone can contribute to any of the models on OSB, either through fixing a bug, adding new features or improving documentation for published models.

While the models can be collaboratively developed in any simulator format, the ultimate aim is to get as much of the model as possible into simulator independent formats like [NeuroML](http://www.neuroml.org) and [PyNN](http://neuralensemble.org/trac/PyNN) to ensure modularity, accessibility and cross simulator portability.

![](http://www.neuroml.org/images/neuroml_logo/neuroml_small.png)


### Who’s behind OSB?

This project was started in the [Silver Lab](http://www.ucl.ac.uk/silverlab) at UCL as part of a [Wellcome Trust](http://www.wellcome.ac.uk) funded project to encourage collaborative development of models in computational neuroscience.

![](http://www.neuroconstruct.org/images/wct.png)

The Principal Investigator for the OSB project is [Angus Silver](/users/6) and the core team at UCL consists of [Padraig Gleeson](/users/4) (Project Manager), [Adrian Quintan](/users311), [Boris Marin](/users/67), [Eugenio Piasini](/users/3). A special thanks to [Matteo Cantarelli](/users/43) for his significant contributions to OSB while at UCL.

A number of international research groups and organizations are currently involved in the Open Source Brain Initiative. See [here](/about) for more details.


### How is this related to other neuroinformatics initiatives?

We are very keen to have close links with other databases and repositories for neuroinformatics and computational neuroscience. Many of these will be enabled through common use of NeuroML, as is used by [NeuroMorpho.org](http://neuromorpho.org/neuroMorpho/index.jsp), and a number of other tools and resources. [NeuralEnsemble](http://neuralensemble.org) hosts a number of software tools which will play a key part in simulating and analysing the models in the OSB.

We are also planning deep links to databases such as [ModelDB](http://senselab.med.yale.edu/modeldb) for original model scripts and [NIF/NeuroLex](/projects/nifshowcase) for definitions of model components.

See [here](http://www.opensourcebrain.org/projects/neuroinformatics/wiki/Wiki) for more details on interactions with other Neuroinformatics resources.

A number of the contributors to this initiative are involved with the various national nodes of the [INCF](http://www.incf.org).

![](/images/incf.png)

### What types of models can be developed?

Models of information processing in the nervous system are created at many levels, from high level models of cognitive processes and consciousness to low level models of signal transduction at synapses. In the short to medium term **OSB will focus on spiking neuron models**, i.e. networks of individual neurons which communicate through sending events to synapses on target cells. The core set of models currently under development in the OSB are conductance based models of (often multicompartmental) neurons. This class of neuronal model is particularly suited to collaborative development, as models of channels and synapses, or whole cell models, are often reused between studies, and the models themselves are complex software entities. The focus of [NeuroML v1.x](http://www.neuroml.org/introduction.php) was on this type of model, but with [version 2.0](http://www.neuroml.org/neuroml2.php), support has been extended to more abstract neuron models (e.g. leaky integrate and fire, adaptive threshold models).

While converting the model components to NeuroML will be a key step towards increasing model transparency and accessibility and making them available for use on multiple simulators, other cross platform technologies will be used to assist model portability. Python is a scripting language commonly used in computational neuroscience and has been adopted by a number of the target simulators for OSB models. [PyNN](http://neuralensemble.org/PyNN) is a Python package for simulator independent specification of neuronal network models, and will be useful for procedural specification of complex network structures. The Simulation Experiment Description Markup Language ([SED-ML](http://sed-ml.org/)) will be used for specifying settings for running simulations of the models. Mappings of the model components in OSB to other structured languages in computational biology will be supported too where appropriate, such as [SBML](http://www.sbml.org), [CellML](http://www.cellml.org/) and [NineML](http://software.incf.org/software/nineml).

### My model’s only available in simulator X, not NeuroML/PyNN. Can I still share it on OSB?

Yes! **If the model is already published, please submit to [ModelDB](http://senselab.med.yale.edu/modeldb) first**. On OSB we are happy to point to public repositories with the latest version of the code in any format, and have a link to the version on ModelDB. However, some of the advanced features of OSB will only be available if (parts of) the model are converted to NeuroML.

If your model is not yet published but it still public (we salute you; you are [the future](http://www.openworm.org)) we’re very happy to have it, but would ask that you make sure the versions used in publications are archived in ModelDB.

### I don't have my model in a public repository. Can I still create a project for my model?

Yes! In order to create a project you only need a name. The more you add to your OSB project the more tools you can use in OSB. For instance by publish your model in a [repository](/docs/Help/Some_Extra_Information) and link it to your OSB projects you may look at it with the OSB Explorer or use some of the validation tools.

### Do I have to be registered for accessing OSB projects and tools?

No. You can browse the OSB projects and use most of the OSB tools. However, if you would like to create your own project you should sign up. 

### How can I contribute?

We are happy to hear from anyone interested in helping out with this initiative. We are particularly keen to get modellers or software developers in computational neuroscience involved.

**There is a central list for projects in OSB (and related NeuroML tools) which require help from volunteers. See [here](http://opensourcebrain.org/docs#Contribute_to_OSB).**

Please sign up [here](/account/register) to be part of OSB or [contact us directly](mailto:info@opensourcebrain.org) for more information. You can also sign up to the **[OSB Announce mailing list](https://groups.google.com/forum/#!forum/osb-announce)** to get updates of progress, or the **[OSB Discuss mailing list](https://groups.google.com/forum/#!forum/osb-discuss)** for more detailed discussions on the various projects on OSB. If you find an issue or you would like to request a feature, you can create a [new issue](https://github.com/OpenSourceBrain/redmine/issues/new) our [GitHub repository](https://github.com/OpenSourceBrain/redmine).

Follow us on Twitter at [@OSBTeam](https://twitter.com/OSBTeam).

