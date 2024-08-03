# 🤖 Building AI Agents with Llama 3.1 🚀

This repository contains code from my colab.research.google.com and instructions for building AI agents using the new Llama 3.1 model, including the 405 billion parameter version 🤯. This guide is designed to be accessible even for those with limited programming knowledge 📚.

## 📝 Overview

* Demonstrates how to use Llama 3.1 models, including the 405B version 📊
* Uses Google Colab for easy, installation-free Python execution 💻
* Covers API usage for Groq and Together.ai 🤝
* Provides step-by-step instructions for setting up and running the models 📝

## 📝 Prerequisites

* Google Colab account 📊
* API keys for Groq and Together.ai 🔑

## 🚀 Installation

Run the following commands in Google Colab to install the required packages:
```python
!pip install groq
!pip install together
```
## 🤔 Usage
* Set up API keys for Groq and Together.ai 🔑
* Create clients for both APIs 🤝
* Run models and handle errors 🚨
* Set system prompts and user prompts for model interaction 💬

## 📊 Model Sizes
* Smaller models: Faster and cheaper, but less capable ⏱️
* Larger models (e.g., 405B): Slower and more expensive, but more intelligent 💡

🙏 Acknowledgements
This guide is based on a [Youtube tutorial](https://www.youtube.com/watch?v=1SsPNc2zldM) by [David Andrej](https://www.skool.com/new-society/about) 🙏. Special thanks to [Groq](https://groq.com/) and [Together.ai](https://www.together.ai/) for providing access to their APIs 🤝.

# Step 1: Create a Google Colab Account
* Go to the [Google Colab website](https://colab.research.google.com/) 
* Click on the "Sign in" button in the top right corner
* If you don't have a Google account, create one by following the prompts
* If you already have a Google account, sign in with your credentials

# Step 2: Install Required Packages
* Open a new Google Colab notebook by clicking on the "New notebook" button
* In the first cell, paste the following code: !pip install groq
* Press Shift+Enter to run the cell
* Wait for the installation to complete
* In the next cell, paste the following code: !pip install together
* Press Shift+Enter to run the cell
* Wait for the installation to complete

# Step 3: Set up API Keys
* Go to the [Groq website](https://groq.com/) 
* Sign up for an account if you don't already have one
* Go to the dashboard and click on "API Keys"
* Create a new API key by following the prompts
* Copy the API key and paste it into a secure location (e.g. a text file)
* Repeat the same steps for [Together.ai](https://www.together.ai/) 

# Step 4: Create Clients for APIs
* In a new cell, paste the following code: import groq
* Press Shift+Enter to run the cell
* In the next cell, paste the following code: groq_client = groq.Client(api_key="YOUR_GROQ_API_KEY")
* Replace YOUR_GROQ_API_KEY with the actual API key you created in Step 3
* Press Shift+Enter to run the cell
* Repeat the same steps for Together.ai: import together and together_client = together.Client(api_key="YOUR_TOGETHER_API_KEY")

# Step 5: Run Models and Handle Errors
* In a new cell, paste the following code: model = groq_client.get_model("llama-3.1")
* Press Shift+Enter to run the cell
* Wait for the model to load
* In the next cell, paste the following code: output = model.generate(text="Hello, world!")
* Press Shift+Enter to run the cell
* Wait for the output to generate
* Repeat the same steps for Together.ai: model = together_client.get_model("llama-3.1") and output = model.generate(text="Hello, world!")

# Step 6: Set System Prompts and User Prompts
* In a new cell, paste the following code: system_prompt = "You are a helpful assistant."
* Press Shift+Enter to run the cell
* In the next cell, paste the following code: user_prompt = "What is the meaning of life?"
* Press Shift+Enter to run the cell
* Wait for the output to generate
