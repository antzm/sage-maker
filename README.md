# AWS SageMaker Jupyter Notebooks

This repository contains Jupyter Notebooks that can be used on AWS's SageMaker.

The purpose of this repository is to include a few Jupyter Notebooks and some small datasets that can be used directly on the SageMaker platform.

When creating a new SameMaker notebook, you can simply provide the URL of this repository and the Jupyter Notebooks, as well as the datasets, will be loaded automatically.

Then, you can select which Jupyter Notebook you wish to run, and make any changes you wish to the provided code.

## Using smaller datasets

When using SageMaker for Machine Learning tasks, it takes a long to time prepare the data and to train a model. Thus, a mistake in training may take many hours before its outcome appears.

For this reason, instead of using big datasets, it more practical to create small datasets and perform all out task using those small datasets and only when we feel confident that our code works as expected, then we could load the full dataset and start creating our model.

## Starting with Amazon SageMaker

For someone new to the Amazon SageMaker, here are the neccesary steps to get you started:

Create an AWS Account

From the AWS management console, type "SageMaker" in the search box to find the SageMaker

Before using the SageMaker for the first time, you will need a valid IAM role which you can create using the following steps:

## Running a SageMaker Notebook

The easiest way to start a SageMaker Notebook is to store your notebook on a GitHub repo and then provide the address of the repo while creting the SageMeker Notebook.

## AWS EC2 Instances

To run a Jupyter Notebook using SageMaker, you will need to select the instance that it will be used to run the notebook. There are noumerous instances available but to run a Notebook, usually one of the small instances is more than adequate, like a t2 or a t3 instance.

Only wile training a model, you will need to run a more powerful instance that it will be used exclusively for the training, while the Notebook itself will continue to run on the t2 or t3 instance that we had already selected.




