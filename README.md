# AWS SageMaker Jupyter Notebooks

This repository contains information about using Amazon SageMaker and additionaly, it also has some Jupyter Notebooks that can be used on Amazon SageMaker.

The purpose of this repository is to include a few Jupyter Notebooks and some small datasets that can be used directly on the SageMaker platform.

When creating a new SameMaker notebook, you can simply provide the URL of this repository and the Jupyter Notebooks, as well as the datasets, will be loaded automatically.

Then, you can select which Jupyter Notebook you wish to run, and make any changes you wish to the provided code.

Thus, the only purpose of this repository, it to help you run easily your first Jupyter Notebook on the Amazon SageMaker platform.

## Why learn how to use SageMaker?

If you have a powefull computer, with a state of the art graphing card, then obviously you could use your own computer for data analysis and machine learning, using jupyter notebboks.

If though you don't own, or in general you don't have access to such a computer, then by all means it would be beneficial to learn how to use the Amazon SageMaker platform, as you will be able to analyze vast amounts of data and to use them for training machine learning models.

## Using smaller datasets

When using SageMaker for Machine Learning tasks, it takes a long to time prepare the data and to train a model. Thus, a mistake in training may take many hours before its outcome appears.

For this reason, instead of using big datasets, it more practical to create small datasets and perform all out task using those small datasets and only when we feel confident that our code works as expected, then we could load the full dataset and start creating our model.

If you would like to make a smaller dataset from a dataset that is stored in a .tar.gz file i.e. a tar file that has been compressed with gzip, then you could follow the detailed instructions in the tar.gz.md [file](tar-gz.md) (in this repository) and build a smaller dataset.  
At the end, you should create a .tar.gz file that contains your smaller dataset. The instructions for that, can also be found in the same file as above.

As an example, a small dataset is included in this repository. It is the IMDB dataset which includes only 0,5% of the original dataset and the purpose is to easily examine the contents of the dataset and to experiment with it.

## Starting with Amazon SageMaker

For someone new to the Amazon SageMaker, here are the neccesary steps to get you started:

Create an AWS Account

From the AWS management console, type "SageMaker" in the search box to find the SageMaker

Before using the SageMaker for the first time, you will need a valid IAM role which you can create using the following steps:

## Running a SageMaker Notebook

The easiest way to start a SageMaker Notebook is to store your notebook on a GitHub repo and then provide the address of the repo while creting the SageMeker Notebook.

## AWS ML EC2 Instances

To run a Jupyter Notebook using SageMaker, you will need to select the ML instance that it will be used to run the notebook. There are noumerous instances available but to run a Notebook, usually one of the small instances is more than adequate, like a t2 or a t3 instance.

Only while training a model, you will need to run a more powerful instance that it will be used exclusively for the training, while the Notebook itself will continue to run on the t2 or t3 instance that we had already selected.

## Choosing an instance

While choosing an instance, we should aim to choose the most adequate instance based on our needs. Otherwise the instance won't be poweful enough to run our code or it may be too poweful which means spending more money than needed.

I would rather say that instances should be chosen wisely!

## SageMaker Instances and Pricing

Details of the SageMaker instances:
https://aws.amazon.com/sagemaker/pricing/instance-types/

Pricing of the SageMaker instances:
https://aws.amazon.com/sagemaker/pricing/

## SageMaker on the AWS Educate Starter Account

The AWS Educate Starter Account supports only the ml.t2 and the ml.t3 instances for the SageMaker. Thus, the SageMaker functionality, under this account, ise limited to the usage of small datasets, as the larger datasets will probably cause an error.

Details about the AWS Educate Starter Account:
https://s3.amazonaws.com/awseducate-starter-account-services/AWS_Educate_Starter_Accounts_and_AWS_Services.pdf

## Important Note:

When you start running a Jupyter Notebook on SageMaker, the notebook will continue running even if you log out from your AWS account. Thus, you should stop the notebook when you don't need it otherwise you will continue to getting charged even if you think that you are not using the AWS services.

As a general note, you should always pay attention to the AWS services that are running in your account and to make sure that anything that is not needed is stopped.

With some experince also, you will be able to select the most effient options for the projects you are running on the AWS platform, so to succesfully perfom the tasks you need and at the same time to save on the cost of the serivce.

## Writing in Markdown language

As a reminder, you can read a few tips for using the Markdown language in the [file](markdown.md) "markdown.md", which you can also find in this repository.

## Adding HTML code in your Jupyter Notebook

In a Jupyter Notebook, you can also add some parts using HTML code, like lists, or a small table of contents if the Jupyter Notebook is too big, so that you can navigate easily inside the Notebook.
