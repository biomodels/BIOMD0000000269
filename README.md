# BIOMD0000000269: Model_1

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000269.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000269.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000269 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This is the single cell model for analysis of hormonal crosstalk in
Arabidopsis described in the article:  
**Modelling and experimental analysis of hormonal crosstalk in Arabidopsis.**   
Liu J, Mehdi S, Topping J, Tarkowski P and Lindsey K. Mol Syst Biol. 2010 Jun
8;6:373; PmID: [20531403](http://www.ncbi.nlm.nih.gov/pubmed/20531403) , DOI:
[10.1038/msb.2010.26](dx.doi.org/10.1038/msb.2010.26)  
Abstract:  
An important question in plant biology is how genes influence the crosstalk
between hormones to regulate growth. In this study, we model POLARIS (PLS)
gene function and crosstalk between auxin, ethylene and cytokinin in
Arabidopsis. Experimental evidence suggests that PLS acts on or close to the
ethylene receptor ETR1, and a mathematical model describing possible PLS-
ethylene pathway interactions is developed, and used to make quantitative
predictions about PLS-hormone interactions. Modelling correctly predicts
experimental results for the effect of the pls gene mutation on endogenous
cytokinin concentration. Modelling also reveals a role for PLS in auxin
biosynthesis in addition to a role in auxin transport. The model reproduces
available mutants, and with new experimental data provides new insights into
how PLS regulates auxin concentration, by controlling the relative
contribution of auxin transport and biosynthesis and by integrating auxin,
ethylene and cytokinin signalling. Modelling further reveals that a bell-
shaped dose-response relationship between endogenous auxin and root length is
established via PLS. This combined modelling and experimental analysis
provides new insights into the integration of hormonal signals in plants.

This model was originally created using Copasi and taken from the
supplementary materials of the MSB article. It uses equation 5 for the auxin
biosynthesis and was altered to also contain the reactions for ACC, IAA and
cytokinine import. Different from the supplementary material, the parameters
for the auxin synthesis, v2, are set to k2c = 0.01 uM and k2=0.2 uM_per_sec
and for the WT PLS transcription k6=0.3 . To obtain the model described in the
first table of the supplementary materials, set k2c=k2=0 and k6=0.9 . For the
pls and PLSox mutants, k6 should be set to 0 and 0.45, respectively.

This model originates from BioModels Database: A Database of Annotated
Published Models. It is copyright (c) 2005-2010 The BioModels Team.  
For more information see the [terms of
use](http://www.ebi.ac.uk/biomodels/legal.html) .  
To cite BioModels Database, please use [Le Novère N., Bornstein B., Broicher
A., Courtot M., Donizelli M., Dharuri H., Li L., Sauro H., Schilstra M.,
Shapiro B., Snoep J.L., Hucka M. (2006) BioModels Database: A Free,
Centralized Database of Curated, Published, Quantitative Kinetic Models of
Biochemical and Cellular Systems Nucleic Acids Res., 34: D689-D691.](http://ww
w.pubmedcentral.nih.gov/articlerender.fcgi?tool=pubmed&pubmedid=16381960)


