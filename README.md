# My-SageMaker-IT-Domain-Expert-Project
This repository contains a proof-of-concept (POC) project that demonstrates how to fine-tune a large language model (LLM) for the Information Technology (IT) domain using Amazon SageMaker.  This project was developed as part of the "Introducing Generative AI with AWS" course, with the goal of building a domain-specific expert model capable of generating relevant and accurate IT-related text.

## Project Overview

The core idea behind this project is to take a pre-trained LLM and specialize it for the IT domain. By training the model on a dataset of IT-focused text, we can significantly enhance its ability to understand and generate text related to IT concepts, challenges, and solutions.

This repository provides a practical example of how to:

* Select and prepare an appropriate dataset for fine-tuning.
* Configure the necessary AWS environment, including IAM roles, SageMaker notebook instances, and GPU instances.
* Fine-tune a foundation model (Meta Llama 2 7B) using Python and SageMaker.
* Deploy the fine-tuned model for inference.
* Evaluate the model's performance and compare it to the original base model.

## Dataset

The dataset used for fine-tuning focuses on the challenges of ubiquitous data management within the IT domain. It includes discussions on topics such as:

* Mobility support
* Context awareness
* Collaboration support
* Adaptivity
* User interaction in ubiquitous computing environments

This dataset helps the model learn the nuances of IT-specific language and concepts.

## Steps Involved

1. **Dataset Selection:**  An IT-relevant dataset focusing on ubiquitous data management challenges was chosen.
2. **Environment Setup:**
    * Configured an AWS IAM role with the necessary permissions for SageMaker.
    * Created a SageMaker notebook instance for development.
    * Provisioned a `ml.g5.2xlarge` GPU instance for the computationally intensive fine-tuning process.
3. **Fine-tuning:**
    * Deployed the Meta Llama 2 7B foundation model on AWS.
    * Used Python scripts to fine-tune the model on the IT dataset.
4. **Model Deployment:** Deployed the fine-tuned LLM on SageMaker for inference.
5. **Testing and Evaluation:**
    * Tested the deployed model's ability to generate IT-related text and answer domain-specific questions.
    * Conducted a comparative analysis between the fine-tuned model and the original model to assess the impact of fine-tuning.

## Technologies Used

* **Amazon SageMaker:** A fully managed service for building, training, and deploying machine learning models.
* **Meta Llama 2 7B Model:** A powerful foundation model pre-trained for text generation, serving as the base for fine-tuning.
* **Python:**  Used for scripting, data processing, and interacting with AWS services.
* **AWS Services:**  Leveraged various AWS services like IAM, EC2, and S3 for managing access, computing resources, and storage.

## Comparative Analysis

The project includes a comparative analysis to evaluate the performance difference between the original Llama 2 model and the fine-tuned IT domain expert model. This analysis demonstrates the effectiveness of fine-tuning in improving the model's ability to generate relevant and accurate IT-related content.

## Repository Contents

* **Notebooks:** Jupyter notebooks used for model fine-tuning and evaluation.
* **Code:** Python scripts for data processing and model training.
* **Data:**  The IT domain dataset used for fine-tuning (may be excluded due to size or licensing).
* **Documentation:** Project reports and documentation.

This project serves as a valuable resource for those interested in learning about LLM fine-tuning and its applications in specific domains.
