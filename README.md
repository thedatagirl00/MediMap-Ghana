# MediMap Ghana: AI-Powered Hospital Bed Management System

## Project Overview

MediMap Ghana is an AI-driven solution designed to optimize hospital bed management in Ghana. This project leverages machine learning to predict bed availability in real-time, assisting healthcare providers in making informed decisions regarding patient admissions, transfers, and resource allocation. The system aims to improve efficiency, reduce patient wait times, and enhance overall hospital operational flow.

## Features

*   **Synthetic Data Generation**: Creation of a simulated hospital operations dataset to mimic real-world scenarios for model training and testing.
*   **Data Preprocessing & Feature Engineering**: Robust handling of raw data, including datetime conversions, extraction of temporal features (hour, day of week), and one-hot encoding of categorical hospital identifiers.
*   **Machine Learning Model**: Implementation and training of a Random Forest Regressor to predict the probability of bed availability based on various hospital metrics (e.g., current occupancy, staff on duty, emergency incoming).
*   **Interactive Streamlit Dashboard**: A user-friendly web application built with Streamlit, providing:
    *   Real-time input controls for hospital metrics.
    *   Instant AI-driven predictions of bed availability.
    *   Visual status indicators (High, Limited, Critical) and recommendations.
    *   Geospatial visualization using `pydeck` to display hospital locations with color-coded availability.
    *   A simulated security audit log for tracking system interactions.
*   **Model Persistence**: Saving the trained machine learning model using `joblib` for easy integration into the Streamlit application.
*   **Deployment Readiness**: Preparation of `requirements.txt` for easy deployment to platforms like Hugging Face Spaces.

## Technologies Used

*   **Python**: Primary programming language.
*   **Pandas**: For data manipulation and analysis.
*   **NumPy**: For numerical operations.
*   **Scikit-learn**: For machine learning model (Random Forest Regressor).
*   **Streamlit**: For building the interactive web dashboard.
*   **Pydeck**: For geospatial data visualization on the dashboard.
*   **Joblib**: For saving and loading the machine learning model.
*   **localtunnel**: For exposing the local Streamlit application to a public URL (for demonstration/testing).
*   **Hugging Face Spaces**: Target platform for sharing and deploying the Streamlit application.
