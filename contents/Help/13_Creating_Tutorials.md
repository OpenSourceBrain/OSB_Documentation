## Note: OSB documentation has been moved! Please see latest documentation (covering both OSBv1 and OSBv2) at: https://docs.opensourcebrain.org

We encourage users to turn their OSB projects into new tutorials.

An example tutorial repository can be found [here](https://github.com/mattearnshaw/tutorials). We refer to this example below.

First, open the model you wish to use for a tutorial. There are two main components to building a tutorial: configuring the default session, and writing the main step-by-step guide.

#### Configuring the default session

Any changes made to the state of a project, such as open widgets, re-coloring of populations, zoom or model position etc. can be saved and reused as the default working environment for the tutorial.
For example, take a look at the [Blue Brain Project Showcase session](http://opensourcebrain.org/projects/blue-brain-project-showcase/models?explorer=https%3A%2F%2Fraw.githubusercontent.com%2FOpenSourceBrain%2FBlueBrainProjectShowcase%2Fsample%2FosbSessions%2Fsample%2FSample_Session.json). Immediately you are greeted with three popup widgets, the model description, tutorial, and an info box. This is achieved simply by creating these windows in your original project (i.e. clicking "Model Description" and using the Console to [add a popup widget](http://docs.geppetto.org/en/latest/usingwidgets.html), and then downloading the project using the ![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/download-project-button.png) button in the top-right toolbar.

The project.zip file contains an xmi file, a json file, a js file, and the results of any experiments you have run. Place the contents of the zip in a [subdirectory of your repo](https://github.com/OpenSourceBrain/BlueBrainProjectShowcase/tree/sample/osbSessions/sample). Then a link to the json file will appear on the models page of your project on OSB:

![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/curated.png)

If you wish to include a step-by-step tutorial component, ensure that you have the tutorial widget open as part of the default session state: you can open a tutorial widget by pressing the book icon in the left toolbar.

#### Writing a step-by-step guide

The main component of tutorials are plain html files, one per step, and a json file to tie them together, see [here](https://github.com/mattearnshaw/tutorials/tree/master/1_hh_practical) for an example.
To create interactive aspects, the `quickExperiment` javascript function can be used to add experiments with parameters set by the tutee, see [here](https://github.com/mattearnshaw/tutorials/blob/master/1_hh_practical/2.html) for an example. The json file should specify a `name` (tutorial title), default `height` and `width` of the tutorial widget, and a list of paths of the html files for each step, see [here](https://github.com/mattearnshaw/tutorials/blob/master/1_hh_practical/hh_practical.json) for an example.

Finally we need to add our tutorials to the tutorial widget by editing the json file downloaded in the step above (Configuring the default session). It may help to run this file through [a formatter](https://jsonformatter.org/json-pretty-print) before editing. To the data field of the tutorial widget, add URLs pointing to the json file(s) that you created above (see [here](https://github.com/mattearnshaw/tutorials/blob/master/models/hodgkinHuxley/GEPPETTO.json) for an example). You may also wish to change the `activeTutorial` field under `componentSpecific` to the title of tutorial you wish to be initially displayed. Tutees may switch between tutorials using the book icon at the top-left corner of tutorial widget.

#### Existing tutorials

You can explore our existing tutorials [here](http://www.opensourcebrain.org/tutorials). The synaptic integration tutorial is still under development.

#### Support

Please <b><a href="http://www.opensourcebrain.org/docs#How_To_Contact_Us" onclick="javascript:(function(event){ enableDocSection($(this).attr('href')); if(window.history.pushState) {window.history.pushState(null, null, $(this).attr('href'));} event.preventDefault(); })">get in contact</a></b> at any stage of preparing your tutorial.
