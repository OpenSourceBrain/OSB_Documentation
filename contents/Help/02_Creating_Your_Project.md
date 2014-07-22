### On ModelDB?

First of all, if the model is published, please submit the original scripts to [ModelDB](http://senselab.med.yale.edu/ModelDB/default.asp*). This is the correct place for depositing models at the time of publication and should be the first port of call for anyone looking for scripts related to a publication in computational neuroscience.

Placing a model on OSB in addition to ModelDB is an indication that you wish to develop your (or other modellers’ publicly shared) models in an open source collaborative environment, to get help debugging/improving them, to convert them to simulator independent formats, and generally encourage wider reuse.

### Sign up to OSB

Register as a user of OSB [here](/account/register). Add your GitHub username and [INCF user profile](http://incf.org/community/people) if you have one.

You should also add the URL of your project, software or lab. In the latter case, if the PI is in agreement, we can add the group to the list of [labs taking part in the OSB initiative](/about#who_about).

### Share your code

Create a new repository for your code on GitHub (see [here](/doc/Help/Some_Extra_Information) if want to know more about Source Code tecnologies and Git/GitHub). See the introduction to this on [GitHub help](https://help.github.com/articles/create-a-repo). You can use the short project name above for the repository name.

This can be hosted on the [OpenSourceBrain GitHub organisation](https://github.com/OpenSourceBrain), but there is no problem having it under your personal account. If you would like us to host the repository, <a href="mailto:info@opensourcebrain.org">let us know</a> and we’ll add the repository and give your GitHub user full access to it.

### Create a new OSB project

Go to http://www.opensourcebrain.org when you’re logged in. There should be a green button on the top right for adding a new project.

![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/NewProject.png)

Enter the long name of the project (can be edited later), the short ID, a description of the project and the path to the GitHub repository. If the code is not on GitHub yet, or if you host it elsewhere leave this blank. The repository URL can be added manually at a later point.

### Write your documentation/wiki

OSB documentation may be generated using [Markdown format syntax](https://daringfireball.net/projects/markdown/basics) and some further Redmine and OSB clauses (See bellow for further information). Note Markdown allows using most html syntax (i.e. videos...). In order to be as compatible as possible with GitHub wikis OSB uses [GitHub Flavored Markdown](https://help.github.com/articles/markdown-basics). You can find a cheatsheet [here](http://127.0.0.1:3000/help/en/wiki_markdown_syntax.html).  

We describe briefly some OSB/Redmine functions to facilitate the doc generation process

#### Reference to a Repository file. 

You can point to any file (markdown or plain text) in your GitHub or Bitbucket repository (the repository set in your project). We will retrieve the file content and display in OSB.

<code>github:[path]
bitbucket:[path]</code>

###### Example: 
<code>github:help/readme.md
bitbucket:help.txt
</code>


#### Reference to pubmed publication: 

<code>pubmed:[publicationID]
</code>

###### Example: 

<code>pubmed:17442244
</code> 

This syntax will generate a reference link like this:
pubmed:17442244

and a bibliography section will be automatically generated at the bottom of the page. This section will summarize all the references using the following format:

Gleeson P,			Steuber V and 			Silver RA,
<i><a href="http://www.ncbi.nlm.nih.gov/pubmed/17442244">neuroConstruct: a tool for modeling networks of neurons in 3D space.</a></i> Neuron, 2007, 54(2): 219-35 

#### Create a formula

You can wrte formulas in your documentation using the latex syntax. You only need to enclose you formula like this:

<code>{{latex(formula)}}
</code>

###### Example:

<code>{{latex(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a})}}
</code>

This will automatically generate the following image using the [google chart API](https://developers.google.com/chart/infographics/docs/formulas): 
![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/formula.png)

#### Link to Wiki page

If you want to link to other wiki page:

<code>[[Wiki page]]
</code>

<a href="#">Wiki page</a>

#### Link to an Issue

If you want to link to an issue in your project:

<code>Issue #12
</code>

Issue <a href="#">#12</a>

#### Link to a Commit

If you want to link to a commit in your repository:

<code>commit:f30e13e43
</code>

<a href="#">f30e13e4</a>


### Say hello…

Now is a good time to drop us a line on info@opensourcebrain.org, and let us know your plans for what you’d like to get out of OSB. We’re always happy to hear from new users.

**Note, you can also get in contact on info@opensourcebrain.org to discuss with us about setting up the project for you.**