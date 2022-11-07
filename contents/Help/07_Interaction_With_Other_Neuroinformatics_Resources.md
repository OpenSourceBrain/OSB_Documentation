## Note: OSB documentation has been moved! Please see latest documentation (covering both OSBv1 and OSBv2) at: https://docs.opensourcebrain.org

Below is a list of some important resources in the neuroinformatics, computational neuroscience and systems biology fields and how the Open Source Brian Repository is planning to interact with them.

### ModelDB

[ModelDB](http://senselab.med.yale.edu/ModelDB/) is a curated database of published models in computational neuroscience. This has been the primary source for most of the original simulator scripts on which the models in OSB are based. Where appropriate, OSB models will link back to the original published models on ModelDB.

Greater links are planned between these resources in the future to facilitate finding original model scripts (in a simulator specific format) and updated versions (in a standardized format) which have been extended/improved/used in other modeling studies.

### NeuralEnsemble

![](/images/neuralensemble.png):http://neuralensemble.org

[NeuralEnsemble](http://neuralensemble.org/) is an effort to coordinate a number of projects developing software for computational neuroscience to create an interoperable set of tools for addressing complex questions about neuronal function.

Many of the tools developed as part of the NeuralEnsemble initiative will be target applications for models developed on OSB.

### NeuroLex & NIF

![](http://www.opensourcebrain.org/attachments/download/85/nifneurolex.png)

[NeuroLex](http://neurolex.org/wiki/Main_Page) is the neuroscience lexicon. Many key elements in OSB models (cells, ion channels, brain regions) have unique entries in the NeuroLex lexicon, and this identifier can be used to identify the elements in OSB.

These references are currently used in many of the Theme Wiki pages (e.g. [here](http://www.opensourcebrain.org/projects/cerebellarmodelling/wiki)) and will become more widely used for identifying cells, cellular elements, channels, etc. since **neuroLexId** is a new attribute in NeuroML v2.0 model elements (see example [here](http://sourceforge.net/apps/trac/neuroml/browser/NeuroML2/examples/NML2_FullCell.nml#L65)).

See the [NIF and NeuroLex Showcase project](http://www.opensourcebrain.org/projects/nifshowcase) for more details.

### BioModels

The [BioModels](http://www.ebi.ac.uk/biomodels-main/) database is a repository of peer-reviewed, published, computational models. We are working with the developers of this database to allow greater linking between models in these repositories.

This work is chiefly taking place in the framework of the [COMBINE Network](http://co.mbine.org).

### NeuroElectro

![](/images/neuroelectro_logo.png):http://neuroelectro.org

[NeuroElectro](http://neuroelectro.org/) is a structured database of information on the electrophysiological properties of neurons. This type of information will be very useful for comparing the electrical properties of model neurons with real experimental data.

An API to the NeuroElectro database will allow retrieval of this data and the [SciUnit](https://github.com/cyrus-/sciunit) package will be used to create tests for models against these properties.

See the [NeuroElectro & SciUnit Showcase project](http://www.opensourcebrain.org/projects/neuroelectrosciunit) for more details.
