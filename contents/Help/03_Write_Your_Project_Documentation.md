There are 2 main options for adding documentation to an OSB project:

  1) Add Wiki pages on the OSB project
  2) Add README files in your GitHub (or other VCS) repository and point to these from the OSB project

## 1) Adding Wiki pages to OSB projects

To add a new Wiki page to your OSB project click on the "Wiki" link on the project option bar (when logged in) and start editing the wiki page.

OSB documentation is written in [Markdown format syntax](https://daringfireball.net/projects/markdown/basics), together with some further Redmine and OSB specific additions (See below for further information). Note Markdown allows you to include most HTML syntax (i.e. videos...). In order to be as compatible as possible with GitHub wikis, OSB uses [GitHub Flavored Markdown](https://help.github.com/articles/markdown-basics). You can find a cheatsheet [here](/help/en/wiki_markdown_syntax.html).  

We describe briefly below some OSB/Redmine features to enhance Wiki pages on OSB.

#### Reference to a Repository file. 

You can point to any file (markdown or plain text) in your GitHub or Bitbucket repository (the repository used in your project).

<code>github:[path]</code>
<code>bitbucket:[path]</code> 

This will retrieve the file content and display it in the OSB wiki page. This allows a single file in your repo (e.g. the main README) to be the master copy of the documentation for your project, and to make that accessible to someone browsing the project on OSB.

###### Example: 
<code>github:help/readme.md</code>
<code>bitbucket:help.txt</code>


#### Reference to pubmed publication: 

<code>pubmed:[publicationID]</code>

###### Example: 

<code>pubmed:17442244</code> 

This syntax will generate a reference link like this:
pubmed:17442244

and a bibliography section will be automatically generated at the bottom of the page. This section will summarize all the references using the following format:

Gleeson P,			Steuber V and 			Silver RA,
<i><a href="http://www.ncbi.nlm.nih.gov/pubmed/17442244">neuroConstruct: a tool for modeling networks of neurons in 3D space.</a></i> Neuron, 2007, 54(2): 219-35 

#### Create a formula

You can wrte formulas in your documentation using the LaTeX syntax. You only need to enclose you formula like this:

<code>{{latex(formula)}}</code>

###### Example:

<code>{{latex(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a})}}
</code>

This will automatically generate the following image using the [google chart API](https://developers.google.com/chart/infographics/docs/formulas): 
![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/formula.png)

#### Link to Wiki page

If you want to link to other Wiki page:

<code>[[Wiki page]]</code>

<a href="#">Wiki page</a>

#### Link to an Issue

If you want to link to an issue in your project:

<code>Issue #12</code>

Issue <a href="#">#12</a>

#### Link to a Commit

If you want to link to a commit in your repository:

<code>commit:f30e13e43</code>

<a href="#">f30e13e4</a>

### 2) Add README files in your GitHub

Instead of adding Wiki pages on OSB, you can simply add [Markdown format](https://daringfireball.net/projects/markdown/basics) files to your GitHub repo (e.g. README.md) and point to these from an OSB Wiki page (or the main project description) using:

<code>github:README.md</code>
