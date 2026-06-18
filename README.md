Smart Farming Synthetic Data Generation using GAN & VAE
Overview

This project explores the use of Generative Artificial Intelligence techniques, specifically Variational Autoencoders (VAE) and Generative Adversarial Networks (GAN), for generating synthetic agricultural data. The objective is to address data scarcity in smart farming applications and support the development of more robust crop recommendation systems.

The project is based on the research paper:

A Comprehensive Review of Synthetic Data Generation in Smart Farming using Variational Autoencoders (VAEs) and Generative Adversarial Networks (GANs)

Objectives
Generate realistic synthetic crop datasets.
Preserve statistical characteristics of the original data.
Compare original and synthetic datasets using multiple evaluation techniques.
Demonstrate the applicability of generative AI in agriculture.
Dataset Features

The dataset contains the following attributes:

Feature	Description
Nitrogen (N)	Soil Nitrogen Content
Phosphorus (P)	Soil Phosphorus Content
Potassium (K)	Soil Potassium Content
Temperature	Environmental Temperature
Humidity	Relative Humidity
pH	Soil pH Level
Rainfall	Rainfall Amount
Crop Label	Recommended Crop
Methodology
Workflow
Crop Dataset
      ↓
Data Preprocessing
(Label Encoding & Scaling)
      ↓
VAE / GAN Training
      ↓
Synthetic Data Generation
      ↓
Evaluation & Validation
Models Used
Variational Autoencoder (VAE)
Learns latent representations of agricultural data.
Generates new realistic samples from latent space.
Useful for data augmentation and feature learning.
Generative Adversarial Network (GAN)
Consists of Generator and Discriminator networks.
Generator creates synthetic crop data.
Discriminator evaluates authenticity.
Produces realistic synthetic records through adversarial training.
Evaluation Techniques

The generated synthetic data is evaluated using:

1. Correlation Heatmaps

Compares relationships among features in original and synthetic datasets.

2. Scatter Plot Analysis

Visualizes distribution similarity between datasets.

3. Statistical Comparison
Mean Comparison
Standard Deviation Comparison
Absolute Log Mean Difference
4. Cumulative Sum Analysis

Examines feature-wise distribution trends.

Results

The generated synthetic data successfully reproduced key characteristics of the original agricultural dataset.

Generated Outputs
Original Dataset Heatmap
Synthetic Dataset Heatmap
Scatter Plot Comparison
Statistical Validation Plots
Cumulative Sum Comparison

These results indicate that the synthetic data maintains similar distribution and correlation structures to the original dataset.

Installation
Clone Repository
git clone <repository-url>
cd <repository-name>
Install Dependencies
pip install -r requirements.txt
Running the Project

Execute the main script:

python "smart farming synthetic data generation.py"

Or use:

run_project.bat

for one-click execution

Project Structure
├── smart farming synthetic data generation.py
├── dataset/
├── output/
│   ├── heatmaps
│   ├── scatterplots
│   ├── cumulative_plots
│   └── synthetic_dataset.csv
├── requirements.txt
├── run_project.bat
└── README.md
Future Work
Implement CTGAN for tabular data generation.
Explore Diffusion Models.
Hyperparameter optimization.
Larger agricultural datasets.
Crop recommendation model training using synthetic datasets.
Research Significance

Synthetic data generation can help overcome agricultural data scarcity, improve machine learning model performance, and support the development of intelligent decision-making systems for smart farming.

Author

Sakshi Singh
Computer Engineering
Research Project: Smart Farming Synthetic Data Generation using Generative AI

Acknowledgement

Special thanks to Dr. Golak Bihari Mahanta for guidance and mentorship throughout this research work.
