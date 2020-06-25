# Sentiment Analysis through AWS Sagemaker and PyTorch

The tutorial notebook and Python files provided here, once completed, result in a simple web app which interacts with a deployed recurrent neural network performing sentiment analysis on movie reviews taken from IMDB. This project assumes some familiarity with PyTorch and AWS SageMaker.

---

## Setup Instructions

The project is intended to be carried out using Amazon Sagemaker. Below, a brief set of instructions on setting up a managed notebook instance using SageMaker, from which the notebooks can be completed and run.

### Log in to the AWS console and create a notebook instance

Log in to the AWS console > go to the SageMaker dashboard > click on 'Create notebook instance'. 
Name the instance as you please. Using the ml.t2.medium is a good idea as it belongs to the free tier. For the role, creating a new role works fine. Using the default options is also okay. Important to note that you need the notebook instance to have access to S3 resources, which it does by default.

### Use git to clone the repository into the notebook instance

Once the instance has been started and is accessible, click on 'open' to get to the Jupyter notebook main page. We will begin by cloning the SageMaker Deployment github repository into the notebook instance. Note that we want to make sure to clone this into the appropriate directory so that the data will be preserved between sessions.

Click on the 'new' dropdown menu and select 'terminal'. By default, the working directory of the terminal instance is the home directory, however, the Jupyter notebook hub's root directory is under 'SageMaker'. Enter the appropriate directory and clone the repository as follows.

```bash
cd SageMaker
git clone https://github.com/fradeleo/MLE_Sentiment_Analysis_Web_App
exit
```

After you have finished, close the terminal window.

### Open and run the notebook of your choice

Now that the repository has been cloned into the notebook instance you may navigate to any of the notebooks that you wish to complete or execute and work with them. Any additional instructions are contained in their respective notebooks.
