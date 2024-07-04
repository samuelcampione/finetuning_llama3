
# Llama3 Personalized Email Writing

While large language models hold potential to automate many time consuming day-to-day tasks, general LLM responses tend to lack personality and are often easily detected as being "AI-generated." By scraping personal sent emails using GMail's API and fine-tuning Meta's Llama3-8B model, this project aims to create an email chatbot that captures the unique voice of the user.

## Introduction

The goal of this project is to create a personalized chatbot for email generation. We achieve this by scraping emails from a Gmail account and fine-tuning a pre-trained LLaMA 3 language model to generate responses that mimic the user's writing style.

## Features

- **Email Scraping:** Collect emails from a Gmail account using the Gmail API.
- **Data Cleaning:** Clean and preprocess the collected email data.
- **Fine-Tuning:** Employ QLoRA and utilize adapters to fine-tune the LLaMA 3 model on the user's email data.
- **Email Generation:** Generate personalized email responses.

## Installation

1. Clone the repository:
   ```bash
   https://github.com/samuelcampione/personalized_llama3.git
   cd personalized_llama3
   ```

2. Set up Gmail API credentials by following [this guide](https://developers.google.com/gmail/api/quickstart/python).

## Usage

### Email Collection and Cleaning

1. Navigate to the `email_collection_and_cleaning` directory and open the Jupyter notebook:
   ```bash
   cd email_collection_and_cleaning
   jupyter notebook email_collection_and_cleaning.ipynb
   ```

2. Follow the steps in the notebook to authenticate with Gmail, collect emails, and preprocess the data.

### Model Fine-Tuning

1. Navigate to the `llama_finetuning` directory and open the notebook in Google CoLab:
   ```bash
   cd ../llama_finetuning
   jupyter notebook llama_finetuning.ipynb
   ```

2. Follow the steps in the notebook to fine-tune the LLaMA 3 model using QLoRA on the preprocessed email data.

## Results

The fine-tuned LLaMA 3 model can generate personalized email responses that closely mimic the user's writing style.
