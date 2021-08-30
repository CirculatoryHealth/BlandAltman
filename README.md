# BlandAltman
[![DOI](https://zenodo.org/badge/256487385.svg)](https://zenodo.org/badge/latestdoi/256487385)

**Collaborators**

none

*Athero-Express Team*

Sander W. van der Laan, 
Arjan Boltjes, 
Michal Mokry, 
Hester den Ruijter, 
Folkert W. Asselbergs, 
Gert Jan de Borst, 
Gerard Pasterkamp.

**Project ID**

BlandAltman


## Background

Example code of the Bland-Altman test with some figures. This example also serves the purpose to show the some key-elements for a GitHub repository:

- a `readme`, like this one with some background information.
- a `scripts` folder which holds some additional scripts.
- an `images` folder for some images one can use anywhere, like in this `readme`.
- a proper `LICENSE` file.
- a proper `.gitignore` file.
- a `renv`-lock file to facilitate project-local R dependency management to projects. Refer to https://rstudio.github.io/renv/articles/renv.html for more information.

This example repository is further based on the `WORCS` package as described below which is a full featured package to facilitate and maximize the Open Science practices in project management.


### Objectives

To apply the Bland-Altman test.


### Study population

Randomly generated dataset.


### Statistical analysis

Regular Bland-Altman test.


## Where do I start?

You can load this project in RStudio by opening the file called 'BlandAltman.Rproj'.


## Project structure

<!--  You can add rows to this table, using "|" to separate columns.         -->
File              | Description                | Usage         
----------------- | -------------------------- | --------------
README.md         | Description of project     | Human editable
BlandAltman.Rproj | Project file               | Loads project 
LICENSE           | User permissions           | Read only     
.worcs            | WORCS metadata YAML        | Read only     
prepare_data.R    | Script to process raw data | Human editable
renv.lock         | Reproducible R environment | Read only     
File              | Description                | Usage         
----------------- | -------------------------- | --------------
README.md         | Description of project     | Human editable
BlandAltman.Rproj | Project file               | Loads project 
LICENSE           | User permissions           | Read only     
.worcs            | WORCS metadata YAML        | Read only     
prepare_data.R    | Script to process raw data | Human editable
renv.lock         | Reproducible R environment | Read only     
File              | Description                | Usage         
----------------- | -------------------------- | --------------
README.md         | Description of project     | Human editable
BlandAltman.Rproj | Project file               | Loads project 
LICENSE           | User permissions           | Read only     
.worcs            | WORCS metadata YAML        | Read only     
prepare_data.R    | Script to process raw data | Human editable
renv.lock         | Reproducible R environment | Read only     
File                       | Description                         | Usage         
-------------------------- | ----------------------------------- | --------------
README.md                  | Description of project              | Human editable
BlandAltman.Rproj          | Project file                        | Loads project
LICENSE                    | User permissions                    | Read only
.worcs                     | WORCS metadata YAML                 | Read only
renv.lock                  | Reproducible R environment          | Read only
bland_altman               | Location of output                  | Human editable
images                     | Location of images                  | Read only
scripts                    | Location of scripts                 | Read only

<!--  You can consider adding the following to this file:                    -->
<!--  * A citation reference for your project                                -->
<!--  * Contact information for questions/comments                           -->
<!--  * How people can offer to contribute to the project                    -->
<!--  * A contributor code of conduct, https://www.contributor-covenant.org/ -->


# Reproducibility

This project uses the Workflow for Open Reproducible Code in Science (WORCS) to
ensure transparency and reproducibility. The workflow is designed to meet the
principles of Open Science throughout a research project. 

To learn how WORCS helps researchers meet the TOP-guidelines and FAIR principles,
read the preprint at https://osf.io/zcvbs/


## WORCS: Advice for authors

* To get started with `worcs`, see the [setup vignette](https://cjvanlissa.github.io/worcs/articles/setup.html)
* For detailed information about the steps of the WORCS workflow, see the [workflow vignette](https://cjvanlissa.github.io/worcs/articles/workflow.html)


## WORCS: Advice for readers

Please refer to the vignette on [reproducing a WORCS project]() for step by step advice.
<!-- If your project deviates from the steps outlined in the vignette on     -->
<!-- reproducing a WORCS project, please provide your own advice for         -->
<!-- readers here.                                                           -->


# References


# Acknowledgements

Dr. Sander W. van der Laan is funded through grants from the Netherlands CardioVascular Research Initiative of the Netherlands Heart Foundation (CVON 2011/B019 and CVON 2017-20: Generating the best evidence-based pharmaceutical targets for atherosclerosis [GENIUS I&II]). We are thankful for the support of the ERA-CVD program ‘druggable-MI-targets’ (grant number: 01KL1802), the EU H2020 TO_AITION (grant number: 848146), and the Leducq Fondation ‘PlaqOmics’.

Plaque samples are derived from carotid endarterectomies as part of the [Athero-Express Biobank Study](http:www/atheroexpress.nl) which is an ongoing study in the UMC Utrecht.

The framework was based on the [`WORCS` package](https://osf.io/zcvbs/).

<a href='https://osf.io/zcvbs/'><img src='images/worcs_icon.png' align="center" height="75" /></a> 


#### Changes log

    Version:      v1.0.1
    Last update:  2021-08-30
    Written by:   Sander W. van der Laan (s.w.vanderlaan-2[at]umcutrecht.nl).
    Description:  Script to do a Bland-Altman test and make some figures.
    Minimum requirements: R version 3.4.3 (2017-06-30) -- 'Single Candle', Mac OS X El Capitan
    
    Changes log
    * v1.0.1 Added some information to this readme.
    * v1.0.0 Initial version. 
    
    
--------------

#### The MIT License (MIT)
##### Copyright (c) 1979-2021 Sander W. van der Laan | s.w.vanderlaan [at] gmail [dot] com.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:   

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Reference: http://opensource.org.
