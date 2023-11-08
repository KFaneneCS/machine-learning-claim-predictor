# Auto Claims Probability Predictor

This project is a machine learning system developed in Jupyter Notebook and hosted on Google Colab.  It uses an auto policies claims dataset from Kaggle (found [here](https://www.kaggle.com/datasets/sagnik1511/car-insurance-data/data)) to predict the probability that a prospective policyholder will file a claim.

## Usage

1. **Please use the "Open in Colab" button at the top of the `Claim_Predictor.ipynb` file. Some of the functionality may not work as expected when viewed directly in GitHub.**

2. If not already signed into Google, sign in by clicking the blue “Sign in” button at the top right of the page.

3. On the top toolbar, click “Runtime” → “Run all”.

4. Under the orange/red Google Colab infinity symbol (looks like a sideways “8”), click the “Table of contents” icon. From here, you will be able to go directly to any portion of the machine learning system’s workflow, including viewing several visual representations of the data and the machine learning algorithms that were used.


## Project Workflow

The project's workflow is as follows:

1. **Data Importation:** The data is imported for analysis and modeling using the Pandas module
2. **Data Review:** An initial review of the data, including a number of visualizations, is performed to understand its contents and structure.
3. **Data Preprocessing:** The data is shuffled and split into train/test splits.  Missing data is imputed using the k-nearest neighbor method, and features are encoded depending on whether they are nominal or ordinal.
4. **Model Training and Testing:** The data is trained and tested on the following models:
   - LinearSVC
   - Random Forest
   - LightGBM
5. **Evaluation:** The results of the trained models are presented and analyzed.
6. **User Interface:** A simple UI using ipywidgets is provided for the user to predict claim probabilities on the LightGBM model.

## Much More To Do...
This project provides just the foundation - there is still much more work to be done.  For example, consider exploring feature importance, using a validation split for hyperparameter tuning, and implementing other advanced techniques to improve the model's performance.
