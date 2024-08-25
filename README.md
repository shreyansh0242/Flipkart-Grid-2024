# AI-Powered Size Chart Generator for Apparel Sellers

## Project Overview

This project focuses on building an AI-powered system to generate accurate size charts for apparel sellers. The system leverages machine learning to analyze limited or inaccurate size data, user body measurements, and purchase history to provide reliable size recommendations, reducing size-related returns and improving customer satisfaction.

---

## Team Information

- **Track Title:** AI-Powered Size Chart Generator for Apparel Sellers
- **Team Name:** U4C997VO
- **Team Member:** Shreyansh Agarwal
- **University:** Netaji Subhas University of Technology
- **Date:** 25th August 2024

---

## How to Run

1. **Download the Dataset**  
   Download the dataset from Kaggle: [Clothing Fit Dataset for Size Recommendation](https://www.kaggle.com/datasets/rmisra/clothing-fit-dataset-for-size-recommendation).

2. **Convert JSON to CSV**  
   The downloaded data is in JSON format. Convert it to CSV using a Python script, or use the pre-converted `cloth.csv` provided in this repository.

3. **Data Preprocessing**  
   Run the `01. Data Preprocessing and Cleaning.ipynb` file in Jupyter Notebook to preprocess the data. This will generate a refined `cloth.csv` file.

4. **Generate Size Charts**  
   Run the `02. model.ipynb` file to generate the size charts. The size charts will be saved as CSV files, organized by category.

---

## Executive Summary

### Problem Overview

Creating accurate size charts using limited data is a challenge faced by apparel sellers. The goal is to develop an AI system that uses body measurements and purchase history to generate size charts.

### Proposed Solution

Our AI model clusters similar body types and successful purchase data to create size charts, adaptable across different apparel categories.

### Impact

This solution is aimed at reducing returns and enhancing customer satisfaction by improving size accuracy.

---

## Technical Approach

### Methodology

1. **Data Preprocessing:** Handling missing values, encoding categorical variables.
2. **Clustering:** Using KMeans to group similar body types and generate size recommendations.
3. **Dynamic Adjustments:** Sizes are fine-tuned based on user feedback on fit and length.

### Tools and Technologies

- **Programming Language:** Python
- **Libraries:** pandas, numpy, scikit-learn

### Algorithm

- KMeans clustering based on user measurements.
- Confidence scores calculated by evaluating proximity to cluster centers.
- Sizes dynamically adjusted based on feedback.

### Setup and Configuration

- The code is run in a Python environment with the necessary libraries installed.
- The dataset is loaded, preprocessed, and size charts are generated for each category.

### Deployment

- The solution can be deployed on a cloud server or integrated into an e-commerce platform to provide real-time size recommendations.

---

## Challenges and Limitations

- **Challenges:** Sparse data for some categories, discrepancies in user feedback.
- **Limitations:** The model may not fully capture body shape variations; feedback-based adjustments may lead to overfitting.

---

## Recommendations and Future Work

- **Further Research:** Incorporate additional features like weight, gender, and age.
- **Future Development:** Build an interactive UI for sellers to manage size charts and allow real-time size adjustments.
