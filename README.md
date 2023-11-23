# Llamma-2Fine-Tune-New-Categorization
 
# 1. Generating Instruction Dataset using GPT-3.5

# Overview
News articles play a crucial role in advancing machine learning research, offering a vast and diverse dataset for training and evaluating models in natural language understanding. This blog explores an innovative solution for efficiently creating a labeled dataset for news classification. The goal is to organize this wealth of information into distinct categories, facilitating research and industry applications such as sentiment analysis and text summarization.

# Dataset Creation
Creating a well-categorized dataset manually or through keyword searches can be challenging. In this blog, we introduce an efficient method to generate an instruction dataset for news classification. The approach involves leveraging OpenAI's GPT 3.5, a powerful Large Language Model (LLM) that powers ChatGPT.

# Ways to Create an Instruction Dataset

**Convert Existing Dataset** : Transform an existing dataset into an instruction dataset tailored for the desired news classification task.

**Use Existing LLMs**: Employ existing Large Language Models to generate an instruction dataset based on the unique language constructs and domain-specific terminology found in news articles.

**Manual Creation**: Manually curate an instruction dataset, ensuring high quality but potentially time-consuming.

Given the need for a high-quality dataset within a limited timeframe and budget, we opt to use GPT 3.5 for dataset creation.

2. # Fine-Tuning Meta’s Llama 2 7B Model for News Article Categorization
Part 1: Setting up and Preparing for Fine-Tuning
1. Installing and Loading Required Modules
Ensure you have the necessary Python modules installed. You can use the requirements.txt file or install them manually.

**pip install -r requirements.txt**

# Approval for Meta’s Llama 2 Models
Below are the steps to request permission for the Llama-2–7B model:

Get approval from Hugging Face (https://huggingface.co/meta-llama/Llama-2-7b-hf).
Get approval from Meta (https://ai.meta.com/resources/models-and-libraries/llama-downloads/).
Create a WRITE access token on Hugging Face (https://huggingface.co/settings/tokens).
Execute !huggingface-cli login in Google Colab Notebook, enter the token, and enter "Y."

# Setting up Hugging Face CLI and User Authentication
Create a WRITE access token on Hugging Face (https://huggingface.co/settings/tokens).
Execute !huggingface-cli login in Google Colab Notebook, enter the token, and enter "Y."


# 3. Deployment to AWS Sagemaker

Aws_SageMaker_Deploy.ipynb is the script to run for sagemaker deployment

**Prequsites**
1. Need an AWS account with AWSSageMakerFullAccess Role configured
2. Derive AWS Credentials 
3. install boto3 and sagemaker









