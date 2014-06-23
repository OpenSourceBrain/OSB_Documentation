![](/attachments/download/106/OSBHackathon1.png)
 (Illustration courtesy of [Matteo Farinella](/users/34))

### OSB Hackathon 2013

(Looking for details on the [Open Source Brain kick off meeting](http://www.opensourcebrain.org/projects/osb/wiki/Sardinia2013) in Sardinia?)

Dates: **9am Wednesday 6th - 5pm Thursday 7th November, 2013**

Location: University College London, UK.

Local organisers: [Matteo Cantarelli](/users/43), [Padraig Gleeson](/users/4), [Eugenio Piasini](/users/3), [Angus Silver](/users/6), [Boris Marin](/users/67)

#### Focus of meeting

The focus of this meeting was on **open source multicompartmental, conductance based cortical cell & network models**.

There are an increasing number of multicompartmental, conductance based (thalamo)cortical cell models being made available and reused/modified by interested parties to address different scientific questions. An example is the [Traub et al 2005 thalamocortical network model](http://www.opensourcebrain.org/projects/thalamocortical) for which Fortran, NEURON, MOOSE and NeuroML versions have been developed in various labs. This meeting was to look at the range of models out there from the neocortex and thalamus which are interesting for multiple parties and work towards getting these onto public, open source repositories, in standardised formats (NeuroML & potentially PyNN) and get them well tested, annotated and ready for use as research tools by the attendees and the wider community.

#### Aims

There were 3 specific aims of the meeting:

1) Consolidate the versions of the Traub network model **which aim to reproduce the results of the 2005 paper**; document what stage these versions are at and what the issues are with each implementation.

2) Create plans for **a new network model at this level of detail**, with updated cells and connectivity, initially based on a refined Traub model; this model *should be open source from the start* and as simulator independent as possible; gather requirements on the experimental data needed for this updated model and the electrical properties they should display; create a framework for optimising these models against the data.

3) Look at the range of **other multicompartmental, conductance based cortical models** which could benefit from this process too (and potentially could be candidates for modification for use in the model of 2)

#### Attendees

[Laszlo Bicskei](/users/229), Andrew Brown ([Southampton](http://www.ecs.soton.ac.uk/people/adb)), [Matteo Cantarelli](/users/43), [Chaitanya Chintaluri](/users/75), [Thomas Greg Corcoran](/users/228), [Helena Głąbska](/users/69), [Padraig Gleeson](/users/4), [Lea Goetz](/users/188), [Boris Marin](/users/67), [Philipe Mendonca](/users/195), [Simon O’Connor](/users/92), [Paola Perin](/users/210), [Eugenio Piasini](/users/3), [Subhasis Ray](/users/39), [Martina Rizza](/users/132), [Arnd Roth](/users/108), [Angus Silver](/users/6), [Richard Tomsett](/users/198), [Mike Vella](/users/50)

#### Agenda

##### Wednesday 6th November

Overall theme: [Thalamocortical modelling](http://www.opensourcebrain.org/projects/corticalmodelling/wiki/Wiki), specifically project:thalamocortical

**Topics for discussion**

* Traub’s model logistic issues and known fixes [FORTRAN (parallel) versus NEURON (parallel) versus NeuroML versus MOOSE]
* Reproducibility of results from Traub’s paper
* Shortcomings/flaws/updates of Traub’s model - Cell level and Network level
* What can Traub’s model tell us?
* Is it worth fixing?
* Research interests for modelling a detailed compartmental TC columnar loop [Compartmental modelling versus spiking neurons].
* A consensus on a good TC loop model - benchmark sorts. [other existing alternate models]
* Can we match (any) experiments? If so which kind?

| |**Morning Session** | |
|:---|:---|:---|
|9:00| [Angus Silver](/users/6) | Welcome |
|9:05| [Padraig Gleeson](/users/4) | Introduction & goals of Hackathon; introduction to Traub model ([Slides](http://www.opensourcebrain.org/attachments/download/117/Hackathon2013_Gleeson_IntroToHachathonAndTraub05.odp)) |
|09:30| [Matteo Cantarelli](/users/43) | Introduction to the latest features on Open Source Brain ([Slides](http://www.opensourcebrain.org/attachments/download/121/Hackathon2013_Cantarelli_OSBIntro.pdf)) |
|10:00| [Chaitanya Chintaluri](/users/75) & [Helena Głąbska](/users/69) | Experiences with Traub model in Parallel NEURON ([WIKI](http://www.opensourcebrain.org/projects/thalamocortical/wiki/Known_issues), [Slides](http://www.opensourcebrain.org/attachments/download/123/Hackathon2013_Glabska_NrnTraub.pdf)) |
|10:30| [Subhasis Ray](/users/39) | Experiences with Traub model in MOOSE ([WIKI](http://www.opensourcebrain.org/projects/thalamocortical/wiki/Known_issues), [Slides](http://www.opensourcebrain.org/attachments/download/122/Hackathon2013_Ray_MooseTraub.pdf)) |
|11:00| | **Coffee break** |
|11:15| [Padraig Gleeson](/users/4) | Experiences converting Traub model to NeuroML ([WIKI](http://www.opensourcebrain.org/projects/thalamocortical/wiki/Known_issues), [Slides](http://www.opensourcebrain.org/attachments/download/117/Hackathon2013_Gleeson_IntroToHachathonAndTraub05.odp)) |
|11:45| [Richard Tomsett](/users/198) | Large scale modelling of the cortex using reduced cell models ([Slides](http://www.opensourcebrain.org/attachments/download/129/Hackathon2013_Tomsett_CortexModel.ppt)) |
|12:15| [Arnd Roth](/users/108) | Optimization and testing of a reduced model of pyramidal neurons ([Paper](http://senselab.med.yale.edu/modeldb/ShowModel.asp?model=146026), [Slides](http://www.opensourcebrain.org/attachments/download/119/Hackathon2013_Roth_OptimisingReducedModels.ppt)) |
|12:45| | General discussion on Cortical modelling ([WIKI](http://www.opensourcebrain.org/projects/corticalmodelling/wiki/Wiki)) and issues with Traub model ([WIKI](http://www.opensourcebrain.org/projects/thalamocortical/wiki/Known_issues)) |
|13:00| | **Lunch** |

| |**Afternoon Session** | |
|:---|:---|:---|
|14:00| | **Hacking session I**: installing, testing & documenting one another’s models; running network models on high performance computing infrastructure |
|15:30| | **Coffee break** |
|15:45| | Continued: General discussion on Cortical modelling ([WIKI](http://www.opensourcebrain.org/projects/corticalmodelling/wiki/Wiki)) and issues with Traub model ([WIKI](http://www.opensourcebrain.org/projects/thalamocortical/wiki/Known_issues)|)
|16:15| | A consensus on a good TC loop model ([WIKI](http://www.opensourcebrain.org/projects/corticalmodelling/wiki/Modelling_the_thalamocortical_loop)) |
|17:30| | **Close of day** |
|19:30| | **Dinner** |

##### Thursday 7th November

Overall theme: [Layer 5 pyramidal cell models](http://www.opensourcebrain.org/projects/l5pyramidalcellmodels/wiki)

**Topics for discussion**

* Inconsistencies in existing L5 Pyramidal cell models - a comparison.
* A consensus on a good model on L5Py cell.
* Nomenclature consensus for single cells - essential for interchangeability and testing.
* Milestones for the next meeting and commitments for parties towards development.
* Essential tools and requirements. [Data sharing, interoperability, testing etc]
* Debate on “columnar structure” of cortex - if this is the right way to think about cortex?
* Auditory cortex versus somatosensory barrel cortex
* Automated testing tools - fortnightly tests depending on participation.

| |**Morning Session** | |
|:---|:---|:---|
|9:00| [Chaitanya Chintaluri](/users/75) & [Helena Głąbska](/users/69) | Incorporating project:l5bpyrcellhayetal2011 biophysical properties into Traub model ([Slides](http://www.opensourcebrain.org/attachments/download/128/Hackathon2013_Chintaluri_HayL5.pdf)) |
|9:30| [Mike Vella](/users/50) | L5 Pyramidal cell modelling & [Neurotune](https://github.com/vellamike/neurotune) ([Slides](http://www.opensourcebrain.org/attachments/download/124/Hackathon2013_Vella_ShapeModulation.pdf)) |
|10:00| [Simon O’Connor](/users/92) | Piriform cortex pyramidal cell model of Vanier ([OSB project](http://www.opensourcebrain.org/projects/piriformcortexvanier), [Slides](http://www.opensourcebrain.org/attachments/download/120/Hackathon2013_OConnor_VanierPiriformCortexModel.pptx)) |
| 10:30 | [Angus Silver](/users/6) | Background network activity extends spatial and temporal integration in a L5 cortical pyramidal cell model |
|11:00| | **Coffee break** |
|11:30| | General discussion on L5 cell modelling ([WIKI](http://www.opensourcebrain.org/projects/l5pyramidalcellmodels/wiki)) |
|13:00| | **Lunch** |

| |**Afternoon Session** | |
|:---|:---|:---|
|14:00| | **Hacking session II**: installing, testing pyramidal cell models; testing packages for model optimisation |
|15:00| | Pipeline for testing realistic models ([WIKI](http://www.opensourcebrain.org/projects/model-tuning/wiki/Wiki)) |
|15:30| | **Coffee break** |
|15:45| Next steps | How do we proceed ([WIKI](http://www.opensourcebrain.org/projects/corticalmodelling/wiki/Priorities)?) Planning for OSB 2014 |
|17:30| | **Close of meeting** |

#### Next steps

##### Some ideas/suggestions for improving OSB interface

Add a search box beside tree view ([issue](https://github.com/epiasini/redmine/issues/63)). Related to [this](https://github.com/epiasini/redmine/issues/57)

Make themes more obvious ([issue](https://github.com/epiasini/redmine/issues/64))

Link to GitHub issues/stars/forks ([issue](https://github.com/epiasini/redmine/issues/65))

List of contributors to the wiki more prominent ([issue](https://github.com/epiasini/redmine/issues/66))

##### Thalamocortical modelling

A list of the priorities/agreed action points from the meeting are [here](http://www.opensourcebrain.org/projects/corticalmodelling/wiki/Priorities).

#### Practicalities

The meeting was held on the main UCL campus: http://www.ucl.ac.uk/maps. Room for both days was: [Foster Court 243](http://www.ucl.ac.uk/estates/roombooking/building-location/?id=040).

Suggestions for accommodation in the vicinity:
http://www.gowerhousehotel.co.uk
http://www.jenkinshotel.demon.co.uk

#### Enquiries

If you have any enquiries about this meeting, please don’t hesitate to contact: [p.gleeson@ucl.ac.uk](mailto:p.gleeson@ucl.ac.uk).
