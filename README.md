# Research Code of Conduct

[![Project Status: WIP - Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](http://www.repostatus.org/badges/latest/wip.svg)](http://www.repostatus.org/#wip)
[![Last updated](https://img.shields.io/badge/Date-2017/02/23-brightgreen.svg)]()

### Why?

With the code of conduct we set standards, that should **help*** increase the 
reproducibility and reusability of the departmental research. 

Reproducibility is the ability of an entire experiment or study to be duplicated,
either by the same researcher or by someone else working independently.
Reproducing an experiment is called replicating it. 
Reproducibility is one of the main principles of the scientific method 
([wikipedia](https://en.wikipedia.org/wiki/Reproducibility)).

Reusability boils down to *not invent the wheel over and over again*. For
a less sloppy wording, see e.g. (https://en.wikipedia.org/wiki/Reusability).

As agreed by the steering group of the RDWD department, applying this Code of
conduct should be standard for new research staff, and is recommended for 
existing staff.


---
### Version control

The core of reproducibility for a modern scientist working with electronic 
reports and computerized simulation/experiments is a working version control.
This is quite different from using file endings such as *almostFinalDraft.doc*.
Version control (aka git for us) should be implemented right from the start.
If you don't know what git is, check the [git basics](https://git-scm.com/videos).
A version control system also works as a kind of lab book, which you can use to
document what you did to get to the results.

Recommendations:

- public repos should be stored on the [KNMI github](https://github.com/KNMI) account
    * consider using repo status badges to indicate the status of your project, e.g. [![Project Status: WIP - Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](http://www.repostatus.org/badges/latest/wip.svg)](http://www.repostatus.org/#wip)
    * use only if your project has official status: [![Status](https://img.shields.io/badge/Status-KNMI--official-brightgreen.svg)]()
- private repos (for a limited amount of users) can be obtained for free at
  [bitbucket](https://bitbucket.org/product)
- if your supervisor does not use git yet get a git buddy, e.g. any 
  [member](https://github.com/orgs/KNMI/people) of the KNMI github account


### Writing

You might think that git is something that programmers use, but that you are not
focused on programming.
Be aware that the process to a report or published paper is long and that many
changes will be made to the initial document.
If this process is not reproducible a lot of knowledge will disappear.

We encourage the use of traceable files, e.g. Latex or (variants of) markdown.
Modern Latex online editors allow to track document history and collaborative
writing (e.g., https://www.sharelatex.com/).
Word files can be set under version control, but changes between different
versions can not be shown. 
Annotations can be made also in a pdf document, e.g using Adobe Acrobat.

### Data management

If the research involves data from extern parties we advise to create a data 
management plan, see e.g. (http://www.wur.nl/nl/show/What-is-a-Data-Management-Plan.htm) 

If not, the following rules still apply:

- never copy and paste data
- use scripts to obtain data (and keep those scripts under version control)

We know that it will not be easy to follow these simple rules, but help us to
make this easier instead of fiddling with your own work arounds. 
Also feel free to consult [us](https://github.com/orgs/KNMI/teams/rrr) if you experience difficulties. 

### Repository management

Try to structure your repository, aka research project folder.
Within a repository you will encounter frequently:

 - data (for all the data)
 - figures (for your plots)
 - R (for your functions)
 - src (for source code)
 - scripts 
 - ...

### Coding standards

If you do program functions or scripts, it is very useful to use some consitent
coding style: 

- Python: [PEP8](https://www.python.org/dev/peps/pep-0008/)
- R: [tidyverse](http://adv-r.had.co.nz/Style.html) or [google](https://google.github.io/styleguide/Rguide.xml)

More generally we think it is useful to write functions, that can be used as a
module or package within several scripts. 
This increases the reusability and decreases the number of potential errors.

### Sugar on top?

If you want to do even more to increase the reproducibility and reusability of 
your project. 
Have a look at the following links:

- [docker](https://www.docker.com/) for even more reproducibility
- [provenance](https://www.w3.org/TR/prov-dm/) Introduction to the concept of provenance and traceability according to W3C.
- [dispel4py](https://github.com/dispel4py/dispel4py) processing library and workflows (https://github.com/aspinuso/wps_workflow)
- [jupyter](https://jupyter.org/) for live notebooks
- [travis CI](https://travis-ci.org/) for automatic checking
- [doxygen](https://en.wikipedia.org/wiki/Doxygen) for easy documentation
  / R-users should have a look at [roxygen2](https://cran.r-project.org/web/packages/roxygen2/index.html) 

***
*if you doubt this and require some changes feel free to contact [us](https://github.com/orgs/KNMI/teams/rrr)
