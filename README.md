# Reproduction of "De-Identification of Free-Text Medical Records Using Pre-Trained Bidirectional Transformers"

This project reproduces the experiments from the paper **"De-Identification of Free-Text Medical Records Using Pre-Trained Bidirectional Transformers"**.  
It fine-tunes a BERT-based model for the de-identification task on a medical dataset, following the methods described in the original research.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Notes](#notes)

## Installation

1. Ensure you have **Python 3.8+** installed.
2. Install the required Python packages:

```bash
pip install torch transformers datasets scikit-learn seqeval
```

If you are missing Jupyter Notebook:

```bash
pip install notebook
```

Alternatively, you can run the notebook directly in **Google Colab**.

## Usage

1. Clone this repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. Open the Jupyter Notebook:

```bash
jupyter notebook
```

3. Run the notebook `project_report_implementation.ipynb` step-by-step:
   - Load and preprocess the data
   - Fine-tune the BERT model
   - Evaluate precision, recall, F1-score, and accuracy

Alternatively, you can upload the notebook to **Google Colab** and run it there.

## Project Structure

- `project_report_implementation.ipynb` — Main notebook containing all preprocessing, model fine-tuning, and evaluation steps
- (Optional) `requirements.txt` — List of Python dependencies (can be added if needed)

## Notes

- **Hardware**: It is recommended to use a **GPU** for training if running locally. Training on CPU may be slow.
- **Data**: This notebook assumes that the required de-identification dataset has been preprocessed or made available.
- **Model**: Fine-tuning uses pre-trained BERT models via HuggingFace's `transformers` library.
- **Metrics**: Evaluation is based on precision, recall, F1-score, and accuracy computed using the `seqeval` package.
