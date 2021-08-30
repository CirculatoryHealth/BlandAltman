# Mapping _SCARF1_ expression in atherosclerotic plaques to plaques characteristics.

**Collaborators**

Yaw Asare,
Marios Georgakis,
Martin Dichgans

*Athero-Express Team*

Sander W. van der Laan, 
Arjan Boltjes, 
Michal Mokry, 
Hester den Ruijter, 
Folkert W. Asselbergs, 
Gert Jan de Borst, 
Gerard Pasterkamp.

**Project ID**

AE_20210218_YAW_SWVANDERLAAN_SCARF1


## Background

We recently identified 22 novel risk loci for stroke (Malik et al., Nat Genet, 2018). Most of these reside in intronic and intergenic regions with gene regulatory function. Analysis of expression quantitative trait loci (eQTL) and protein quantitative trait loci (pQTL) suggested that the effects of risk alleles in the _SCARF1_ gene region on atherogenesis are mediated through elevated _SCARF1_ expression (unpublished data). However, the suspected link between altered _SCARF1_ expression and atherosclerosis remains to be established as do the specific mechanisms underlying this relationship. _SCARF1_ was first described to bind and internalize modified LDL (Brown et al., 1979; Brown et al., 1979) and to be critical in recognizing apoptotic cells (Ramirez-Ortiz et al., 2013; Murshid et al., 2015). On professional phagocytes, such as macrophages and dendritic cells, SCARF1 recognizes C1q bound to phosphatidylserine (PS) – a marker for apoptotic cells – and subsequently internalizes and degrades their cell remnants (Ramirez-Ortiz et al., 2013). 


### Objectives

Against this background, we now aim to make use of the data from Athero-Express Biobank Study to explore the associations of _SCARF1_ expression levels in the atherosclerotic plaques from patients undergoing carotid endarterectomy with phenotypes of plaque vulnerability and secondary vascular events over a follow-up of three years. 

To assess the cellular expression, we will use the available single-cell RNAseq data. 


### Study population

We will include data from patients with available plaque SCARF1 expression levels in Athero-Express Biobank Study (n ± 600 individuals). 


### Exposure

SCARF1 expression in the plaque, as assessed by bulk and single-cell RNA sequencing. As part of the regular quality control of RNA sequencing data, the expression is normalized.


### Outcomes

We will examine cross-sectional associations between plaque _SCARF1_ expression and the following plaque vulnerability phenotypes as well as the composite plaque vulnerability index:

- `calcification`, coded `Calc.bin` no/minor vs. moderate/heavy staining
- `collagen`, coded `Collagen.bin` no/minor vs. moderate/heavy staining
- `fat10`, coded `Fat.bin_10` no/<10% fat vs. >10% fat
- `fat40`, coded `Fat.bin_40` no/<40% fat vs. >40% fat
- `intraplaque hemorrhage`, coded `IPH.bin` no vs. yes
- `macrophages (CD68)`, coded `macmean0` mean of computer-assisted calculation CD68<sup>+</sup> region of interest
- `smooth muscle cells (alpha-actin)`, coded `smcmean0` mean of computer-assisted calculation SMA<sup>+</sup> region of interest
- `intraplaque vessel density (CD34)`, coded `vessel_density` manually counted CD34<sup>+</sup> cells per 3-4 hotspots
- `mast cells`, coded `Mast_cells_plaque` manually counted mast cell tryptase<sup>+</sup> cells (https://academic.oup.com/eurheartj/article/34/48/3699/484981)
- `neutrophils (CD66b)`, coded `neutrophils` manually counted CD66b<sup>+</sup> cells (https://pubmed.ncbi.nlm.nih.gov/20595650/)

Continuous variables were inverse-rank normal transformated, indicated by `_rankNorm`. 

Furthermore, we will examine in longitudinal analyses the associations between _SCARF1_ expression levels and secondary cardiovascular events over a three-year follow-up period. The primary outcome will be a composite of fatal or non-fatal myocardial infarction, fatal or non-fatal stroke, ruptured aortic aneurysm, fatal cardiac failure, coronary or peripheral interventions, leg amputation due to vascular causes, and cardiovascular death. The secondary outcomes will be incidence of fatal or non-fatal stroke, incidence of acute coronary events (fatal or non-fatal myocardial infarction, coronary interventions), and cardiovascular death.


Additional variables:

1.	Age (continuous in 1-year increment)
2.	Sex (male vs. female)
3.	Presence of hypertension at baseline (defined either as history of hypertension, SBP ≥140 mm Hg, DBP ≥90 mm Hg, or prescription of antihypertensive medications) 
4.	Presence of diabetes mellitus at baseline (defined either as a history of diabetes, administration of glucose lowering medication, HbA1c ≥6.5%, fasting glucose ≥126 mg/dl, or random glucose levels ≥200 mg/dl).
5.	Smoking (current, ex-, never)
6.	LDL-C levels (continuous) 
7.	Use of lipid-lowering drugs
8.	Use of antiplatelet drugs 
9.	eGFR (continuous)
10.	BMI (continuous) 
11.	History of cardiovascular disease (stroke, coronary artery disease, peripheral artery disease)
12.	Level of stenosis (50-70% vs. 70-99%)
13.	Presenting symptoms (asymptomatic, ocular, TIA, or stroke)


### Statistical analysis

We will first compare plaque expression levels of SCARF1 across categories of the variables presented in the list above. For continuous traits, we will compare the levels across the following categories: age (years), <55, 55-64, 65-74, 75-84, 85+; LDL-C (mg/dl), <100, 100-129, 130-159, 160-189, 190+; eGFR (ml/min/1.73m2), <30, 30-59, 60-89, 90+; BMI (kg/m2), <18.5, 18.5-24.9, 25-29.9, 30-34.9, 35+.

Comparisons will be done with the t-test for binary traits and with ANOVA for traits with >2 categories. 

Then we will explore cross-sectional associations between _SCARF1_ expression levels and the plaque vulnerability characteristics. Linear regression models will be used for continuous traits and logistic regression models for binary traits. SCARF1 expression levels in the plaque will be added as a continuous variable (per 1-SD increment) and in a secondary approach as a categorical variable in 4 quartiles, with baseline as reference, to test for potential non-linearity in the association. We will have four additive models:

- Model 1: adjusted for age and sex
- Model 2: adjusted for age, sex, hypertension, diabetes, smoking, LDL-C levels, lipid-lowering drugs, antiplatelet drugs, eGFR, BMI, history of CVD, level of stenosis, 

Next, we will explore in logistic regression models associations between SCARF1 expression levels in the plaque with symptomatic vs. asymptomatic plaque. As a symptomatic plaque, we will define plaques associated with an ipsilateral ischemic stroke, transient ischemic attach or central retinal artery occlusion. 
To explore the mechanisms underlying these associations we will further examine whether plaque _SCARF1_ expression levels are associated with plaque inflammation and matrix turnover. We will thus examine the age- and sex-adjusted associations of plaque _SCARF1_ expression levels with multiple cytokines and with metalloproteinase activity in carotid plaques. 

Finally, we will explore associations between plaque _SCARF1_ expression levels and secondary cardiovascular endpoints over follow-up (primary and secondary outcomes, as described in the section ‘outcomes’).  We will use Cox proportional hazard models for _SCARF1_ as continuous (per 1SD increment) and categorical trait (in quartiles) taking into account the time between surgery and the occurrence of the events, death, loss to follow-up or completion of follow-up. The same four multivariable models will be used as in the abovementioned analyses. 

We can present a Kaplan-Meier figure for the primary composite endpoints across the four _SCARF1_ quartiles and the results from the multivariable analyses in a Table. 

For all analyses, the statistical significance threshold is set at a two-sided p<0.05. 


### Athero-Express Biobank Study

We have bulk RNAseq (n = 635 samples) and single-cell RNAseq data with extensive histological plaque characterisation. 


### Whole-plaque RNAseq

For the expression analysis we used carotid plaque-derived bulk RNAseq data and queried it for the gene list. Below a graph showing the overall expression of the genes (not all are in the data) compared to the mean expression of 1,000 randomly picked genes. 

**Figure 1: Overall expression of target genes in carotid plaques from the Athero-Express Biobank Study**
![Overall expression of target genes in carotid plaques from the Athero-Express Biobank Study](bulkRNAseq/AERNA/PLOTS/20210608.TargetExpression_vs_1000genes.png)

We assessed the correlation with plaque characteristics (mentioned above) and secondary major adverse cardiovascular events (MACE [major]) at 30 days and 3 years after CEA. 


### Single cell RNAseq

We projected target genes to the single-cell RNAseq data derived from 37 carotid plaque samples. We identified cell communities (Figure 2), mapped and projected target gene expression to the cell communities (Figure 3). 

**Figure 2: Cell communities identified in carotid plaques from the Athero-Express Biobank Study**
![Cell communities identified in carotid plaques from the Athero-Express Biobank Study](scRNAseq/AESCRNA/PLOTS/20210608.UMAP.png)


**Figure 3: Dotplot showing expression of target genes per cell type in carotid plaques from the Athero-Express Biobank Study**
![Dotplot showing expression of target genes per cell type in carotid plaques from the Athero-Express Biobank Study](scRNAseq/AESCRNA/PLOTS/20210608.DotPlot.Targets.png)


## Where do I start?

You can load this project in RStudio by opening the file called 'AE_20210218_YAW_SWVANDERLAAN_SCARF1.Rproj'.

## Project structure

<!--  You can add rows to this table, using "|" to separate columns.         -->
File                       | Description                         | Usage         
-------------------------- | ----------------------------------- | --------------
README.md                  | Description of project              | Human editable
AE_20210218_YAW_SWVANDERLAAN_SCARF1.Rproj | Project file                        | Loads project
LICENSE                    | User permissions                    | Read only
.worcs                     | WORCS metadata YAML                 | Read only
renv.lock                  | Reproducible R environment          | Read only
AnalysisPlan               | Location of analysis plan           | Human editable
Results                    | Some results                        | Read only
Results                    | Some results                        | Read only

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

- Brown et al. (1979). Receptor-mediated endocytosis: insights from the lipoprotein receptor system. Proc Nat Acad Sci 76:3330–7.
- Brown et al. (1979). Reversible accumulation of cholesteryl esters in macrophages incubated with acetylated lipoproteins. J Cell Biol 82:597–613.
- Malik R,…(168 coauthors)…, Dichgans M (2018). Multi-ancestry genome-wide association study of 520,000 subjects identifies 32 loci associated with stroke and stroke subtypes. Nat Genet 50(4):524-537.
- Murshid et al. (2015) Emerging roles for scavenger receptor SREC-I in immunity. Cytokine 75(2):256-60.
- Ramirez-Ortiz et al. (2013). The scavenger receptor SCARF1 mediates the clearance of apoptotic cells and prevents autoimmunity. Nat immunol 14(9):917-26.


# Acknowledgements

Dr. Sander W. van der Laan is funded through grants from the Netherlands CardioVascular Research Initiative of the Netherlands Heart Foundation (CVON 2011/B019 and CVON 2017-20: Generating the best evidence-based pharmaceutical targets for atherosclerosis [GENIUS I&II]). We are thankful for the support of the ERA-CVD program ‘druggable-MI-targets’ (grant number: 01KL1802), the EU H2020 TO_AITION (grant number: 848146), and the Leducq Fondation ‘PlaqOmics’.

Plaque samples are derived from carotid endarterectomies as part of the [Athero-Express Biobank Study](http:www/atheroexpress.nl) which is an ongoing study in the UMC Utrecht.

The framework was based on the [`WORCS` package](https://osf.io/zcvbs/).

<a href='https://www.era-cvd.eu'><img src='images/ERA_CVD_Logo_CMYK.png' align="center" height="75" /></a> <a href='https://www.plaqomics.com'><img src='images/leducq-logo-large.png' align="center" height="75" /></a> <a href='https://www.fondationleducq.org'><img src='images/leducq-logo-small.png' align="center" height="75" /></a> <a href='https://osf.io/zcvbs/'><img src='images/worcs_icon.png' align="center" height="75" /></a> <a href='https://www.atheroexpress.nl'><img src='images/AE_Genomics_2010.png' align="center" height="100" /></a>

#### Changes log
    
    _Version:_      v1.0.8</br>
    _Last update:_  2021-06-08</br>
    _Written by:_   Sander W. van der Laan | s.w.vanderlaan-2[at]umcutrecht.nl.
    
    TO DO
    > add Model 1
    > add Model 2
    > add longitudinal analysis
    > add asymptomatic/symptomatic analysis
    
    * v1.0.8 Update to readme. Initial analyses. 
    * v1.0.7 Made WORCS project. 
    * v1.0.6 Small bug fixes. 
    * v1.0.5 Added png for overlap-figure.
    * v1.0.5 Removed obsolete references to objects.
    * v1.0.4 Fixed a mistake in the chr X sample-file creation. Now the order matches the chr X data.
    * v1.0.3 Fixed weight of files (limit of 10Mb per file for templates). Renamed entire repo.
    * v1.0.2 Added sex-specific .sample-files. Added GWASToolKit input-files.
    * v1.0.0 Initial version. Add 'plaque vulnerability index', Fixed baseline table, added codes, and results. Created sample-files. 

--------------

#### Creative Commons BY-NC-ND 4.0
##### Copyright (c) 1979-2021 Sander W. van der Laan | s.w.vanderlaan [at] gmail [dot] com.

This is a human-readable summary of (and not a substitute for) the [license](LICENSE). 

You are free to: 
Share — copy and redistribute the material in any medium or format. The licensor cannot revoke these freedoms as long as you follow the license terms.

Under the following terms: 
- Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use. 
- NonCommercial — You may not use the material for commercial purposes. 
- NoDerivatives — If you remix, transform, or build upon the material, you may not distribute the modified material. 
- No additional restrictions — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

Notices: 
You do not have to comply with the license for elements of the material in the public domain or where your use is permitted by an applicable exception or limitation.
No warranties are given. The license may not give you all of the permissions necessary for your intended use. For example, other rights such as publicity, privacy, or moral rights may limit how you use the material.


