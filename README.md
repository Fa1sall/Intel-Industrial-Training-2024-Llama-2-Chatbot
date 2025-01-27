# Intel-Industrial-Training-2024-Finetuning-Llama-2-7b-hf

## Problem Statement
PS-4: “Introduction to GenAI and Simple LLM Inference on CPU and finetuning of 
LLM Model to create a Custom Chatbot” 

## Overview
This project focuses on creating a custom chatbot for Text Generation using pretrained Llama-2-7b-chat-hf model, finetuning with the standford alpaca dataset and performing simple inference on a CPU. 

## Project Details
- Model Used: [Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf)
- Dataset: [Stanford Alpaca](https://huggingface.co/datasets/tatsu-lab/alpaca)
- Building Chatbot: [build_chatbot_on_spr](Notebooks/build_chatbot_on_spr.ipynb)
- Finetuning Chatbot: [single_node_finetuning_on_spr](Notebooks/single_node_finetuning_on_spr.ipynb) 
- Documentation: [Project Report](Intel_Report_2024.pdf)

## Team Details
* **Team Name**: LogiCoders
* **Team Leader**: Faisal Irfan
* **Team Members**:
    * Ajmal Masood
    * Danusham  

## Running the project
Perform these operations on the [Intel Developer Cloud](https://www.intel.com/content/www/us/en/developer/tools/devcloud/services.html)
### Setup the environment
```
pip install intel-extension-for-transformers
```

### Install Requirements
```
git clone https://github.com/intel/intel-extension-for-transformers.git
%cd ./intel-extension-for-transformers/intel_extension_for_transformers/neural_chat/
pip install -r requirements_cpu.txt
pip install -r requirements.txt
```

### HuggingFace Login
- Create a HuggingFace Access token with permission to the preferred model
- Login using the following command:
```
huggingface-cli login
```

### Run the Notebooks
```
build_chatbot_on_spr.ipynb
single_node_finetuning_on_spr.ipynb
```
