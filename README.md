# Personalized Mental Health Assistance: Benchmarking LLM Performance for Optimal Care 🧠

This project implements and evaluates a fine-tuned LLM for mental health counseling applications. Follow the instructions below to run the experiments.

## Prerequisites

- Python 3.12+
- CUDA-capable GPU (recommended)
- Virtual environment (recommended)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/devshafi/llm-benchmarking
cd <project-folder>
```

Please follow the instruction given below to successfully run all the sections of this project.

> **Important:** Please follow run files below as the serial given, otherwise the project might not work.

> 🔑 **Note:** Please download the environment variables from OnQ and save them .env file in the root of this project. The project has two environment variables dependencies; One for OpenAI API key and another is MongoDB Database URI.  PLEASE MAKE SURE NOT TO MISUSE THE SECRETS.


## Dataset Preparation for fine-tuning
For the fine-tuning of the base model, at first dataset must be prepared. To prepare the dataset, please go to the [dataset-preparation.ipynb](/dataset/dataset-preparation.ipynb) file and follow the instructions provided before each cell.


### Fine-tune the base model
The fine tuning of the base LLM model is done in the [fine_tune_model.ipynb](/fine_tune_model.ipynb) file. Go to this file and follow the instructions given before each of the cell.

### Fine-tuning analysis
The analysis of the fine-tuning of the llama 3.2 1B model is provided in the [fine-tune-analysis.ipynb](/fine-tune-analysis.ipynb) file. As the progress of the fine-tuning of the model cannot be persisted, I stored them and later use them for the graph.

## Benchmarking LLM
The benchmarking of the fine-tuned LLM with the base model and GPT3.5 turbo is done in [benchmarking.ipynb](/benchmarking.ipynb) file. The details of the benchmarking is given before each cell.

## Function calling 

### Dataset Preparation for function-calling
As synthetic dataset is used for the purpose of function calling, the dataset is prepared in [dataset-preparation.ipynb](/dataset//EHR_dataset/dataset-preparation.ipynb).

### Function calling Experiment
Experiment of function calling is done in [/function-calling.ipynb](/function-calling.ipynb). Details of the experiment can be found while opening the file.


## Contact

If any issue arises during the project testing, feel free to reach out: 📧 Email: [f.shafi@queensu.ca](mailto:f.shafi@queensu.ca)
