# AI Model Quantisation

This repository contains scripts and configurations for quantizing AI models, featuring dedicated tools for working with any AI models.

## 📁 Project Structure

The project consists of the following core files and configuration documents:

*   **`main.py`**: The primary entry script for the application.
*   **`quantise_qwen.py`**: A specialized Python script designed specifically to handle the quantization of Qwen models.
*   **`run_quantised_model.py`**: A script used to execute and interact with the model after the quantization process is complete.
*   **`requirements.txt`**: A standard text file listing the required Python packages.
*   **`pyproject.toml` & `uv.lock`**: Modern Python package configuration and dependency lock files, indicating the use of `uv` or similar modern dependency management.
*   **`env-example`**: A template file illustrating the required environment variables.

## ⚙️ Prerequisites & Setup

*   **Python Version**: The project is configured to use Python version `3.14`, as defined in the `.python-version` file.
*   **Hugging Face Token**: Authentication is required to download or interact with Hugging Face models. 
*   To configure your token, you must set up an environment file containing your token in the format `HF_TOKEN="your-hugging-face-access-token"`. You can use the provided `env-example` file as a starting point.
*   **Version Control**: The repository's `.gitignore` file is configured to exclude local environment files (`.env`), Python virtual environments (`.venv`), and the output directory for the resulting models (`quantised-model`).

## 🚀 Usage Workflow

Based on the provided repository structure, the standard operational workflow is as follows :

1.  **Configure Environment**: Copy `env-example` to `.env` and insert your active Hugging Face token.
2.  **Install Dependencies**: Install the necessary packages using `requirements.txt` or via the `pyproject.toml` configuration.
3.  **Quantize the Model**: Execute `quantise_qwen.py` to process and quantize the target Qwen model . The resulting files will likely be saved in the `quantised-model` directory.
4.  **Run the Model**: Use the `run_quantised_model.py` script to test and run inference on your newly quantized model.
