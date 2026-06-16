# AI Model Quantisation

This repository contains scripts and configurations for quantizing AI models, featuring dedicated tools for working with Qwen models[cite: 1].

## 📁 Project Structure

The project consists of the following core files and configuration documents[cite: 1]:

*   **`main.py`**: The primary entry script for the application[cite: 1].
*   **`quantise_qwen.py`**: A specialized Python script designed specifically to handle the quantization of Qwen models[cite: 1].
*   **`run_quantised_model.py`**: A script used to execute and interact with the model after the quantization process is complete[cite: 1].
*   **`requirements.txt`**: A standard text file listing the required Python packages[cite: 1].
*   **`pyproject.toml` & `uv.lock`**: Modern Python package configuration and dependency lock files, indicating the use of `uv` or similar modern dependency management[cite: 1].
*   **`env-example`**: A template file illustrating the required environment variables[cite: 1].

## ⚙️ Prerequisites & Setup

*   **Python Version**: The project is configured to use Python version `3.14`, as defined in the `.python-version` file[cite: 1].
*   **Hugging Face Token**: Authentication is required to download or interact with Hugging Face models[cite: 1]. 
*   To configure your token, you must set up an environment file containing your token in the format `HF_TOKEN="your-hugging-face-access-token"`[cite: 1]. You can use the provided `env-example` file as a starting point[cite: 1].
*   **Version Control**: The repository's `.gitignore` file is configured to exclude local environment files (`.env`), Python virtual environments (`.venv`), and the output directory for the resulting models (`quantised-model`)[cite: 1].

## 🚀 Usage Workflow

Based on the provided repository structure, the standard operational workflow is as follows[cite: 1]:

1.  **Configure Environment**: Copy `env-example` to `.env` and insert your active Hugging Face token[cite: 1].
2.  **Install Dependencies**: Install the necessary packages using `requirements.txt` or via the `pyproject.toml` configuration[cite: 1].
3.  **Quantize the Model**: Execute `quantise_qwen.py` to process and quantize the target Qwen model[cite: 1]. The resulting files will likely be saved in the `quantised-model` directory[cite: 1].
4.  **Run the Model**: Use the `run_quantised_model.py` script to test and run inference on your newly quantized model[cite: 1].
