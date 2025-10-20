# Project: Generative AI for Synthetic Data Generation

## Objective
Create realistic synthetic datasets to augment limited real-world data for training machine learning models.

## Tools
Python, GANs (Generative Adversarial Networks - specifically CTGAN used here), pandas, scikit-learn, matplotlib, seaborn, Google Generative AI (for narrative report)

## Steps
1.  **Load and explore real data**: Load the Iris dataset and perform initial exploratory data analysis (descriptive statistics, distributions, PCA).
2.  **Choose and set up GAN model**: Set up the CTGAN library for tabular data synthesis.
3.  **Train the GAN model**: Train the CTGAN model on the real Iris data.
4.  **Generate synthetic data**: Generate synthetic data samples using the trained CTGAN model.
5.  **Validate synthetic data**: Assess the quality and similarity of the generated synthetic data to the real data using descriptive statistics, visualizations (histograms, PCA), and correlation matrices.
6.  **Use synthetic data for model training**: Train a machine learning model (RandomForestClassifier) on both the real data alone and a combination of real and synthetic data to evaluate the impact of synthetic data on performance.
7.  **Refine and iterate**: (Optional) Refine GAN parameters and re-evaluate synthetic data quality and model performance.

## Outcome
This project demonstrates the process of generating synthetic data using a GAN model and evaluating its effectiveness in augmenting real data for machine learning tasks. The analysis includes a comparison of real and synthetic data characteristics and the impact of synthetic data on model performance.

## Application
Synthetic data generation can be applied in various domains like healthcare, finance, and autonomous vehicles where real data is scarce, sensitive, or imbalanced, to improve AI model robustness and performance.

## Setup and Running
1.  Clone this repository.
2.  Install the required libraries (see `requirements.txt`).
3.  If you want to run the narrative report generation part using Google Gemini, you need to:
    *   Obtain a Google AI Studio API key.
    *   Add the API key to your Google Colab secrets manager with the name `GOOGLE_API_KEY`.
4.  Open and run the Jupyter Notebook (`<your_notebook_name>.ipynb`) in a Python environment (like Google Colab or your local machine with Jupyter installed).

## Files in this Repository
*   `<your_notebook_name>.ipynb`: The main Jupyter Notebook with all the code and analysis.
*   `README.md`: This file.
*   `requirements.txt`: Lists the Python dependencies.

## Notes
*   The Iris dataset is loaded directly from `sklearn.datasets` within the notebook, so no separate dataset file is needed.
*   The effectiveness of synthetic data can vary significantly depending on the dataset and the generative model used. This project serves as an example workflow.
