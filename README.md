# Amazon ML Challenge 2025

This repository contains notebook experiments for predicting product prices from
catalog text:

- `ml-chall-3.ipynb` cleans catalog text, builds TF-IDF and numeric features,
  trains a LightGBM regressor, and writes `test_out.csv`.
- `final_notebook.ipynb` fine-tunes a BERT masked-language model with LoRA,
  generates text embeddings, and trains XGBoost and LightGBM regressors.

## Data

The notebooks expect the challenge's `train.csv` and `test.csv` files. Update
the dataset paths in the notebook to match your environment:

- `ml-chall-3.ipynb` currently uses `/kaggle/input/amazon-ml-challenge-25/`.
- `final_notebook.ipynb` currently uses `/content/`.

The training data is not included in this repository. Generated CSV files are
ignored by Git.

## Running

Open a notebook in Jupyter or the platform where the challenge data is mounted,
install the Python packages imported by that notebook, and run its cells.
`final_notebook.ipynb` additionally requires a compatible PyTorch environment
and access to the Hugging Face model used by the notebook.
