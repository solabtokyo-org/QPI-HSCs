# Prediction of hematopoietic stem cell diversity using quantitative phase imaging driven machine learning


Yogo Takao<sup>1,2</sup><sup>*</sup>, Yuichiro Iwamoto<sup>3</sup>, Hans Jiro Becker<sup>1,2</sup>,Takaharu Kimura <sup>1,2</sup>, Ayano Sugiyama-Finnis<sup>1.2</sup>,Tomomasa Yokomizo<sup>4</sup>,Toshio Suda<sup>5,6</sup>, Sadao Ota<sup>3</sup> and Satoshi Yamazaki<sup>1,2,7</sup><sup>\*</sup></br>

<sup>1</sup>Division of Cell Regulation, Center for Experimental Medicine and Systems Biology, The Institute of Medical Science, The University of Tokyo, Tokyo, Japan.<br>
<sup>2</sup>Division of Cell Engineering, Center for Stem Cell Biology and Regenerative Medicine, The Institute of Medical Science, The University of Tokyo, Tokyo, Japan.<br>
<sup>3</sup>Research Center for Advanced Science and Technology, The University of Tokyo, Tokyo, Japan.<br>
<sup>4</sup>Department of Microscopic and Developmental Anatomy, Tokyo Women's Medical University, Tokyo, Japan.<br>
<sup>5</sup>International Research Center for Medical Sciences, Kumamoto University, Tokyo, Japan.<br>
<sup>6</sup>Cancer Science Institute of Singapore, Centre for Translation Medicine, National University of Singapore, Singapore, Singapore.<br>
<sup>7</sup>Laboratory for Stem Cell Therapy, Faculty of Medicine, Tsukuba University, Ibaraki, Japan.<br>

<sup>*</sup>Corresponding author. Email: takayogo0430@g.ecc.u-tokyo.ac.jp (T.Y.) y-sato4@ims.u-tokyo.ac.jp (S.Y.)

Innovative identification technologies for hematopoietic stem cells (HSCs) have advanced the frontiers of stem cell biology. However, most analytical techniques capture only a single snapshot, disregarding the temporal context. A comprehensive understanding of the temporal heterogeneity of HSCs necessitates live-cell, real-time and non-invasive analysis. Here, we developed a prediction system for HSC diversity by integrating single-HSC ex vivo expansion technology with quantitative phase imaging (QPI)-driven machine learning. By analyzing single-cell kinetics with QPI, we discovered previously undetectable diversity among HSCs that snapshot analysis fails to capture. Our QPI-driven algorithm quantitatively evaluates the stemness of individual HSCs and incorporates temporal information to significantly improve prediction accuracy. This platform marks a paradigm shift from "identification" to "prediction", enabling us to forecast HSC status by analyzing their past temporal dynamics.


### Information

Code for the publication Prediction of hematopoietic stem cell diversity using quantitative phase imaging driven machine learning

### Dependencies
We recommend installing the dependencies in a conda environment. If you haven't already, install miniconda on your system by following this [link](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html).<br>
Once conda is installed, create and activate an environment by entering these lines into a command line interface:<br>
1. `conda create --name QPI-HSCs`
2. `conda activate QPI-HSCs`


Next, install PyTorch and torchvision for your system by following this [link](https://pytorch.org/get-started/locally/).<br> 
After that, you're ready to install the dependencies for this repository:<br>
`pip install lightning jupyterlab matplotlib tifffile scikit-image tensorboard pandas seaborn scikit-learn`

Tested on:<br> Windows 11(23H2), Python 3.11.5 (lightning 2.2.1, jupyterlab 3.6.4, matplotlib 3.7.2, tifffile 2023.4.12, scikit-image 0.22.0 ,tensorboard 2.16.2)<br>
The installation process should only take a few minutes.

### Getting Started
The 'examples' directory contains notebooks for segmenting cells from sample QPI images, predicting gene expression, and running the analyses in the paper. These outputs are expected and will take about an hour total to run.
