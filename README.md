# FakeNewsDetection-FCA-ML

![R](https://img.shields.io/badge/built%20with-RStudio-blue?logo=rstudio&logoColor=white)
![Machine Learning](https://img.shields.io/badge/tech-Machine%20Learning-blueviolet)
![Formal Concept Analysis](https://img.shields.io/badge/tech-FCA-orange)
![Shiny App](https://img.shields.io/badge/frontend-Shiny-5ec962)

<p align="center">
  <img src="images/university-of-malaga-logo.png" alt="University of Málaga Logo" width="500"/>
</p>

---

## Overview
This repository contains the source code and materials for my Final Degree Project in Software Engineering, aimed at detecting fake news by combining **Formal Concept Analysis (FCA)** and **Machine Learning (ML)** techniques.  
The goal is to improve the classification and understanding of fake news by enhancing traditional machine learning models with FCA, providing greater interpretability and pattern discovery.

---

## Project Goals

- **Detect fake news** by analyzing Facebook engagement metrics.
- **Combine** Machine Learning techniques with Formal Concept Analysis (FCA) for better interpretability.
- **Create new features** based on user interaction data (likes, comments, shares).
- **Build and train predictive models** (Random Forest, SVM, etc.).
- **Develop an interactive Shiny App** to allow users to test the models with new input data.
- **Document the full workflow** with reproducible research using QuartoBook.

---

## Features

- **Dataset**: Based on Facebook engagement metrics from the **Evons dataset**.
- **Preprocessing**: Cleaning, normalization, and feature engineering for engagement indicators.
- **Modeling**: Implementation of machine learning algorithms (Random Forest, SVM, etc.).
- **Formal Concept Analysis (FCA)**: Discovery of hidden patterns and formal structures to assist in classification.
- **Evaluation**: Using Accuracy, Precision, Recall, and F1-score as metrics.
- **Shiny App**: An interactive web application allowing users to visualize predictions and use the models directly.

---

## Dataset: Evons

This project uses the **Evons dataset**, introduced in the paper:  
**"Evons: A Dataset for Fake and Real News Virality Analysis and Prediction"**  
- *Authors*: Kriste Krstovski, Angela Soomin Ryu, and Bruce Kogut  
- *Conference*: COLING 2022

The dataset focuses on **Facebook engagement characteristics** (likes, shares, comments) linked to fake and real news articles.

**Key information about Evons:**
- **Source of real news articles**: "All the News 2.0" dataset ([link](https://components.one/datasets/all-the-news-articles-dataset))
- **Source of fake news articles**: Specific fake media outlets, available for download ([link](https://www.dropbox.com/scl/fi/ywe7qjunwfoewuhsovdwu/articles.tar.gz?rlkey=szj6v3g4m3bdrj264ftzs0xxh&dl=0))
- **Facebook Engagement Data**: Includes number of comments, likes, shares, and total engagements.
- **Labeling**: Each article is labeled (`is_fake`) as fake (`1`) or real (`0`).
- **Images**: Thumbnail images linked to the articles, available separately ([link](https://www.dropbox.com/scl/fi/4ssdoi78civwhn6fxweld/images.tar.gz?rlkey=0n8pd8j5s4x327foztyami4en&dl=0)).

The dataset CSV (`evons.csv`) can be accessed here:  
[Download evons.csv](https://www.dropbox.com/scl/fi/k05g7rr5wiqccay7xope6/evons.csv?rlkey=9riao2g3uz3iaktijfgaheplf&dl=0)

---

## Project Structure
/data/
- Raw and cleaned data (e.g., evons.csv, evons_clean.csv, evons_features.csv)

/scripts/
- R scripts for loading, cleaning, feature engineering, and model building - Example: 01_librerias.R, 02_formacion_dataset.R, 03_modelado_ml.R

/fca/
- Formal Concept Analysis methods and scripts - Example: FCA lattice generation, FCA feature extraction

/models/
- Saved trained Machine Learning models - Example: random_forest_model.rds, svm_model.rds

/app/
- Shiny App files (UI and Server scripts) - Example: app_ui.R, app_server.R, app.R

/docs/
- QuartoBook project documenting the full process - Example: index.qmd, 02_dataset.qmd, 03_modeling.qmd


---

## References

- Kriste Krstovski, Angela Soomin Ryu, Bruce Kogut (2022). *Evons: A Dataset for Fake and Real News Virality Analysis and Prediction*. COLING 2022.  
- [All the News 2.0 Dataset](https://components.one/datasets/all-the-news-articles-dataset)

---

✅ *This project aims to combine the power of machine learning and formal concept structures to detect and understand fake news behavior through engagement metrics.*

## License

This project was developed as part of the Final Degree Project in Software Engineering at University of Málaga.
All rights are reserved by University of Málaga.
