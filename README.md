# Domain Adaptation 
Course: Trends and Application of Computer Vision

The goal of this project was to explore the topic of Domain Adaptation, with an initial anaylis of the SOTA and then hands-on trying to improve DANN and ablation studies of self training

## Outline

| <a href="static/assets/presentations/TACV-I-milestone.pdf" target="_blank"><b>First presentation</b></a> | <a href="static/assets/report/report.pdf" target="_blank"><b>Report</b></a> | <a href="static/assets/presentations/TACV-final-presentation.pdf" target="_blank"><b>Final presentation</b></a> |
|--------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| [![](static/assets/images/thumbnails/first%20presentation.png)](docs/presentations/TACV-I-milestone.pdf)              | [![](static/assets/images/thumbnails/report.png)](docs/report/report.pdf)         | [![](assets/presentation-thumbnail.png)](docs/presentations/TACV-final-presentation)        |



## First presentation
The first presentation can be found [here](static/assets/presentations/TACV-I-milestone.pdf)

In the first presentation we focused on an overview of SOTA **Unsupervised Domain Adaptation**, trying to understand the different available methods and their differences
## Report
The report can be found here [here](docs/report/report.pdf).
This report aims to provide a synthetic overview of what we have found from an initial anaylis of the topic of **UDA**. Although not exhaustive, we exensively researched the field in order to provide a overall summary.
## Notebooks
The notebooks used for the test and analysis are [here](src/notebooks/)
The main ideas are two:
- [adversarial_architectures.ipynb](src/notebooks/adversarial_architectures.ipynb): try to **combine and merge** different approached, starting from **DANN** and building of top of that. 
- [aux_self_train.ipynb](src/notebooks/aux_self_train.ipynb): in depth analysis and ablation study on **self-training**, because the technique is very unique and we wanted to shed light on its mechanism. Also an official implementation was not available. 

| [adversarial_architectures.ipynb](src/notebooks/adversarial_architectures.ipynb) | [aux_self_train.ipynb](src/notebooks/aux_self_train.ipynb) |
| -------------------------------------------------------------------------------- | ---------------------------------------------------------- |
 <a target="_blank" href="https://colab.research.google.com/github/filippodaniotti/TACV-DA-project/blob/master/src/notebooks/adversarial_architectures.ipynb">  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> | <a target="_blank" href="https://colab.research.google.com/github/filippodaniotti/TACV-DA-project/blob/master/src/notebooks/aux_self_train.ipynb">  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> |

We also created a pipeline of standardized operations for testing, in order to speed up evaluation 

|<div style="width:200px"></div>| <div style="width:200px"></div>| <div style="width:200px"></div>|
|--------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| [![](static/assets/images/output.gif)](static/assets/images/output.gif)              | [![](static/assets/images/t-SNE.png)](static/assets/images/t-SNE.png)         | [![](static/assets/images/classification%20report.png)](static/assets/images/classification%20report.png)        |
|[![](static/assets/images/confusion%20matrixes.png)](static/assets/images/confusion%20matrixes.png)              | [![](static/assets/images/source_errors.png)](static/assets/images/source_errors.png)         | [![](static/assets/images/target_errors.png)](static/assets/images/target_errors.png)        |

## Second presentation
The second presentation can be found here [here](static/assets/presentations/TACV-final-presentation)
In here we discuss the results of both our research in combination of different techniques and our ablation study.

In the end a very brief summary is:
- Merging DA techniques may not always result in the expected perfomances of the single approaches
- Overlaying DA techniques may result in overly complicated architectures
- More often than not DA techniques need dataset and model specific tuning, making transferability not trivial
- Not all DA techniques may be applied to every dataset. In particular a preemptive dataset analysis to choose the best suited DA technique for the dataset can increase the results significantly