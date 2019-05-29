# Machine Learning Workshop For OU
To Launch a remote session click the binder button below.
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cnpennin/OU_Machine_Learning_Workshop/master)

# Introduction   

This folder will contain the material for the machine learning workshop for OU. It is a combination of the Machine Learning workshop that was offered at SSA 2019 and the seismoDL101 Tutorial. The documentation for both of these can be found below. 

## SSA Machine Learning Workshop Information
### Structure of the repo

The folder is structured as:
* notebooks - folder contains all the Jupyter notebooks
* data - folder contains data used for examples
* figs - folder contains images used in the notebooks
* presentations - folder contains the presentation slides

Note that this workshop aims to give you a sense of how machine learning works using Python and seismological examples. We assume you have basic working knowledge of Python. All the dependencies are listed in the *environment.yml* file with the versions specified. If you want to install the packages and run a local version on your own machine, the easiest way is to use [Anaconda](https://www.anaconda.com/distribution/) or [miniconda](https://docs.conda.io/en/latest/miniconda.html), and use either conda or pip to install all the dependencies. 

### Content of the workshop

In this workshop, we will cover:  
* Introduction of machine learning (Karianne)
* Clustering (Daniel)
* Feature selection and engineering (Maruti)
* Classification (Qingkai)
* Regression (Zefeng)
* Deep learning (Youzuo)

### Running the code
If you just want to run the code in the cloud, press the 'launch Binder' badge on the top left corner of the page. 

Currently it contains un-finished work, use at your own risk. It will be fully ready before April 23rd. 

### Instructors: 
(alphabetical order)
* Karianne J. Bergen
* [Qingkai Kong](http://seismo.berkeley.edu/qingkaikong/)
* Zefeng Li
* Youzuo Lin
* [Maruti K. Mudunuru](https://www.lanl.gov/expertise/profiles/view/maruti-mudunuru)
* [Daniel T. Trugman](https://www.lanl.gov/expertise/profiles/view/daniel-trugman)

## seismoDL101
Tutorial on seismic signal/noise classification; from linear to deep classifiers

This jupyter notebook tutorial is meant to be a general introduction to machine
and deep learning. We use seismic time series data from i) real earthquakes and
ii) nuisance signals to train a suite of supervised keras classifiers to
discriminate between the two signal classes. We start from linear classifiers
and gradually increase their complexity, to demonstrate to what extent deep
convnet classifiers outperform shallower and linear ones. We also explore how
to evaluate binary classifiers, and how much data we actually need to train
deep classifiers.

No prior knowldedge on seismology or machine learning is required; much of the
tutorial builds on concepts from undergraduate-level applied mathematics
(calculus, linear algebra, optimization). No GPUs or other special hardware is
required, your laptop should work just fine. The repository contains training
and testing data set files that together are ~100Mb in size, so it may take a
minute or two for downloading.

I recommend you use the
[Anaconda Python distribution](https://www.anaconda.com/distribution/) to
set up a working environment with TensorFlow (I used version 1.5.0) and keras
(2.2.4). If you are using unix and have installed conda you can set everything
up by typing the following line in the terminal:

    $ conda create -c conda-forge -n seismoDL101 python=3.6\
      jupyter numpy scipy obspy keras tensorflow scikit-learn\
      seaborn pandas h5py

Then activate the environment (type `conda activate seismoDL101` in
terminal), and open the notebook (type `jupyter notebook` in terminal), and you
should be ready to ... explore machine and deep learning!

I hope you enjoy the tutorial (\_/) For comments and questions please email
mmeier@caltech.edu; last update: April 29, 2019; v1.0
