<img src="cimcb_logo.png" style="width: 160px; float: right;">

# README.md - `SI_Mendez_etal_2019`   

<br/>

<p align="justify">This repository contains the supplementary information for the journal article, "Functional Equivalence ...". There are two types of workflows included in this repository: a standardised visualisation and interrogation partial least squares (PLS) regression workflow, and an equivalent artificial neural network workflow.</p>

<p align="justify">Two previously published datasets are used as examples of the standardised PLS workflow and the proposed equivalent ANN workflow. The first, by <a href="https://www.nature.com/articles/bjc2015414">Chan et al. (2016)</a> is a urine NMR dataset comprised of 149 named metabolites, publicly available on Metabolomics Workbench (Study ID: <a href="http://dx.doi.org/DOI:10.21228/M8B10B">ST0001047</a>). Two classes were used: gastric cancer (n=43) vs. healthy controls (n=40). The second, by <a href="https://doi.org/10.1371/journal.pgen.1004801">Ganna et al. (2014)</a> and <a href="https://doi.org/10.1101/002782">Ganna et al. (2015)</a> is a plasma LC-MS with 189 named metabolites, publicly available on Metabolights (Study ID: <a href="https://www.ebi.ac.uk/metabolights/MTBLS90">MTBLS90</a>). Samples were split into two classes by sex: males (n=485) and females (n=483).</p>

<p align="justify">Due to the structural equivalence with PLS, a shallow (2-layer) ANN is used in this study. Provided the success of this approach towards visualisation and interrogation in shallow ANNs, it may then be possible to adapt this further to deeper ANN architectures. This shallow (2-layer) ANN architecture has a hidden layer consisting of multiple neurons (n = 2 to 6) with a sigmoidal activation, and an output layer consisting of a single neuron with a sigmoidal activation function.</p>

<p align="justify">The standardised PLS workflow and the proposed equivalent ANN workflow include the following steps: hyperparameter optimisation, building and training the model, bootstrap resampling of the model, model evaluation, and model visualisation. All steps and accompanying visualisation methods are described in detail above each corresponding code cell within the workflows. These workflows were implemented using the Python programming language, and are presented as Jupyter Notebooks. There are three ways to that these can be accessed: as a static HTML file, in the cloud (using Binder), or downloaded and run on a local machine.</p>

<br/>

### *To open notebooks as static HTML files:* 
-  [PLSDA_ST001047.html (Method: PLS-DA; Dataset: ST001047)](https://kevinmmendez.github.io/MetabViz/static/PLSDA_ST001047.html) 
-  [ANNSigSig_ST001047.html (Method: ANN-SS; Dataset: ST001047)](https://kevinmmendez.github.io/MetabViz/static/ANNSigSig_ST001047.html) 
-  [PLSDA_MTBLS90.html (Method: PLS-DA; Dataset: MTBLS90)](https://kevinmmendez.github.io/MetabViz/static/PLSDA_MTBLS90.html) 
-  [ANNSigSig_MTBLS90.html (Method: ANN-SS; Dataset: MTBLS90)](https://kevinmmendez.github.io/MetabViz/static/ANNSigSig_MTBLS90.html)

<br/>

### *To launch the notebooks in the cloud (using Binder):* 
-  [PLSDA_ST001047.ipynb (Method: PLS-DA; Dataset: ST001047)](https://mybinder.org/v2/gh/kevinmmendez/MetabViz/master?filepath=notebooks/PLSDA_ST001047.ipynb) 
-  [ANNSigSig_ST001047.ipynb (Method: ANN-SS; Dataset: ST001047)](https://mybinder.org/v2/gh/kevinmmendez/MetabViz/master?filepath=notebooks/ANNSigSig_ST001047.ipynb) 
-  [PLSDA_MTBLS90.ipynb (Method: PLS-DA; Dataset: MTBLS90)](https://mybinder.org/v2/gh/kevinmmendez/MetabViz/master?filepath=notebooks/PLSDA_MTBLS90.ipynb) 
-  [ANNSigSig_MTBLS90.ipynb (Method: ANN-SS; Dataset: MTBLS90)](https://mybinder.org/v2/gh/kevinmmendez/MetabViz/master?filepath=notebooks/ANNSigSig_MTBLS90.ipynb) 

<br/>

### *To download and run notebooks on a local machine*
<p align="justify">This requires Python 3.x and Jupyter to be installed on your local machine. We recommend using the Anaconda Distribution, which can be download from the Anaconda Webpage (<a href="https://www.anaconda.com/distribution/#download-section/">https://www.anaconda.com/distribution/</a>). For information on installing Python and using Jupyter Notebooks, refer to the tutorial, "Toward collaborative open data science in metabolomics using Jupyter Notebooks and cloud computing" by <a href="https://doi.org/10.1007/s11306-019-1588-0">Mendez et al. (2019)</a>.</p>

<i>Note: If you are using Windows, you need to install git using the following:<i/> [Git for Windows](https://gitforwindows.org/)

1. Open Terminal on Linux/MacOS or Command Prompt on Windows
2. Enter the following into the console (one line at a time)

```console
git clone https://github.com/kevinmmendez/MetabViz
cd MetabViz
conda env create -f environment.yml
conda activate MetabViz
jupyter notebook
```


<br/>
