## Note: OSB documentation has been moved! Please see latest documentation (covering both OSBv1 and OSBv2) at: https://docs.opensourcebrain.org

### Towards community developed cerebellar granule cell models

This project was started following the [2013 OSB kickoff meeting](http://www.opensourcebrain.org/projects/osb/wiki/Meetings). At that meeting it was decided that the development of individual cell models from the cerebellum would be a good test case for exploring the requirements on technical infrastructure and the social aspects of collaborative model development. Due to the many independent granule cell layer networks being developed by participants at the OSB meeting, the cerebellar granule cell was identified as a good first cell model to focus on.

This wiki is intended to help gather the following information/requirements:

-   ***What granule cell models are out there?***
-   ***What electrophysiological properties do labs wish to reproduce in their models?***
-   ***What experimental data is publicly available on the behaviour of the granule cell?***
-   ***How well do existing models reproduce these behaviours?***

### Models of the cerebellar granule cell

#### Models currently available on OSB

| **Model** | **Summary** |
|:---|:---|
| project:granulecell | Single compartment, conductance based |
| project:grancellsolinasetal10 | Single compartment, conductance based |
| project:granulecellvscs | Single compartment, conductance based |
| project:multicompgrc | Multcompartmental, conductance based |
| project:grancellrothmanif | Integrate and fire model |
| project:cerebellargainandtiming | Integrate and fire cell in network model |

#### Other known granule cell models

*Links to entries on ModelDB or PubMed articles…*

Simões de Souza F, De Schutter E (2011) **Robustness effect of gap junctions between Golgi cells on cerebellar cortex oscillations** Neural Systems & Circuits 1:7:1-19 ([ModelDB](http://senselab.med.yale.edu/modeldb/ShowModel.asp?model=139656), reuses project:grancellsolinasetal10 ?)

### Target electrophysiological properties of granule cells

To facilitate comparison between granule cell models it would be good to quantify certain properties of the cell activity which labs find **in their experimental data** and which should be reproduced in models. An initial list of properties is:

-   Resting Potential
-   Input Resistance
-   Reversal potential of Na
-   Reversal potential of K
-   AP max depolarisation
-   Firing rate at ?? Hz
-   Total cell capacitance
-   Soma radius
-   More…

Different species, drugs, experimental conditions will lead to different values for these between labs. Nevertheless, it would be good to get input from as many labs as possible.

#### D’Angelo lab

*Species: …
Experimental setup summary: …
Resting potential: …*

#### Silver lab

These figures are mainly based on data obtained by Jason Rothman for the paper: [Synaptic depression enables neuronal gain control](http://www.nature.com/nature/journal/v457/n7232/full/nature07604.html) Nature 2009.

Species: **Sprague-Dawley rats**
Region: **Cerebellar vermis**
Method: **Whole-cell recordings \*
Full methods [here](http://www.nature.com/nature/journal/v457/n7232/full/nature07604.html#online-methods).
AP threshold:**~~38mV to~~42 mV\*
AP height (from threshold to peak): **72 mV**
AHP depth (from threshold to AHP minimum) **21 mV**
Time of AP threshold to time of AHP minimum: **0.9 ms**

![](http://www.opensourcebrain.org/attachments/download/81/JasonAPstats2.png)
…

### Publicly accessible data on granule cell behaviour

#### Links to electrophysiological data in public repositories

\_(Wishful thinking I know…)\_

#### NeuroElectro properties of granule cells

http://www.neuroelectro.org/neuron/21/

### How well do existing models reproduce these behaviours?

Information on construction of tests for comparing model behaviour to experimental data

Much of this will be based on [NeuroUnit/SciUnit](http://www.opensourcebrain.org/projects/neuroelectrosciunit) and existing test scripts in neuroConstruct projects (e.g. [here](https://github.com/OpenSourceBrain/GranuleCell/blob/master/neuroConstruct/pythonScripts/RunTests.py)). What kinds of tests would constitute a good start, e.g. “Properties X, Y, and Z from dataset A should be matched to within 0.5 SD of their mean”?
