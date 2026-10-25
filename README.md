
# Data Science-Based Ride Demand Prediction System

## Project Overview
This project focuses on predicting ride-hailing demand using historical trip data from New York City and Bangalore. Developed as part of the Data Science course, it applies data analysis and machine learning techniques to identify demand patterns, estimate passenger wait times, and support dynamic pricing decisions.

The system also explores cross-city transfer learning to adapt demand prediction models to new locations with limited training data.

## Key Features
- **Demand Forecasting:** Predicts ride demand using historical trip patterns.
- **Exploratory Data Analysis:** Identifies trends, relationships, and demand fluctuations through statistical analysis and visualizations.
- **Feature Engineering:** Extracts useful temporal and geographical patterns from raw data.
- **Cross-City Transfer Learning:** Adapts a model trained on one city to another using limited local data.
- **Surge Pricing Estimation:** Supports pricing decisions based on predicted demand.
- **Wait-Time Prediction:** Estimates passenger waiting times.
- **Interactive Dashboards:** Provides visual insights for riders, drivers, administrators, and developers.

## Dataset
The project uses ride-demand data from two cities:

- **New York City:** Historical trip records used to analyse demand trends and train prediction models.
- **Bangalore:** Trip data used to study local demand patterns and evaluate cross-city model adaptation.

The datasets undergo preprocessing and feature extraction to prepare them for analysis and machine learning.

## Machine Learning Approach
Multiple machine learning models are evaluated and compared to identify a suitable approach for demand prediction.

- **Exploratory Data Analysis (EDA):** Examines distributions, trends, and relationships within the datasets.
- **Data Preprocessing:** Handles missing values, transforms variables, and prepares features for modelling.
- **Feature Engineering:** Creates time-based and location-related features to improve predictive performance.
- **Model Evaluation:** Compares prediction errors and generalisation performance across candidate models.
- **Final Model:** Gradient Boosting is selected based on the project's model evaluation results.

## Transfer Learning Across Cities
A key component of the project is adapting demand prediction to different geographical locations. A model developed using data from one city is adapted to another city with limited local training data.

This approach explores how machine learning models can be reused across regions, reducing dependence on large datasets for every new deployment.

## Web Application
The project includes an interactive web interface for exploring predictions and analytics.

- **Frontend:** Streamlit
- **Backend:** FastAPI

The dashboard is organised around different user perspectives:

- **Riders:** Demand trends and estimated waiting times.
- **Drivers:** Demand patterns that may help identify busy areas.
- **Administrators:** Operational insights and pricing-related analytics.
- **Developers:** Model outputs and technical information.

## Technologies Used
- **Python** – Core programming language
- **Pandas & NumPy** – Data manipulation and numerical computation
- **Scikit-learn** – Machine learning and model evaluation
- **Matplotlib & Seaborn** – Data visualisation
- **Streamlit** – Interactive dashboard development
- **FastAPI** – Backend API development

## Installation and Execution

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <project-folder>
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the Application
```bash
streamlit run app.py
```

If the FastAPI backend is required, start it separately using the project's configured backend entry point.

## Project Objective
The goal is to apply data science and machine learning to improve ride-hailing operations through demand forecasting, wait-time estimation, cross-city model adaptation, and data-driven pricing decisions.
