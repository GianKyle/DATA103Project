# Titanic Survival Prediction Dashboard

This project is an interactive web dashboard built with Streamlit that uses machine learning to predict passenger survival on the Titanic. It allows users to input passenger features, receive a survival prediction, and explore the data and model performance with a focus on fairness and explainability.

## 🚢 Features

*   **Interactive Prediction**: Input passenger features (age, class, sex, etc.) and get a real-time survival prediction.
*   **Model Comparison**: Switch between a Logistic Regression and a Random Forest model to compare their predictions.
*   **Survival Scenarios**: View pre-defined scenarios to quickly see how different profiles (e.g., "Wealthy Woman," "Poor Man") fare.
*   **Fairness & Bias Audit**: Analyze the model's fairness using metrics like Selection Rate and Demographic Parity Difference from the `fairlearn` library.
*   **Exploratory Data Analysis**: Interactive charts and plots to explore the underlying Titanic dataset.
*   **Model Performance**: View key performance metrics for the selected model, including Accuracy, Precision, Recall, and ROC-AUC.

## 🛠️ Technology Stack

*   **Python**: Core programming language.
*   **Streamlit**: For building the interactive web application.
*   **Pandas**: For data manipulation and analysis.
*   **Scikit-learn**: For building and evaluating machine learning models.
*   **Matplotlib & Seaborn**: For data visualization.
*   **Fairlearn**: For fairness and bias auditing.
*   **Jupyter Notebook**: For data exploration, model training, and experimentation.

## 📂 Project Structure

```
.
├── app.py                  # The main Streamlit application script
├── P1_Code.ipynb           # Jupyter Notebook for data cleaning, EDA, and model training
├── requirements.txt        # Python dependencies
├── logistic_model.pkl      # Saved Logistic Regression model
├── rf_model.pkl            # Saved Random Forest model
├── titanic_cleaned.csv     # The cleaned and feature-engineered dataset
├── figures/                # Directory for saved plots and charts
└── README.md               # This file
```

## 🚀 Local Setup Instructions

To run this project on your local machine, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/GianKyle09/DATA103Project.git
    cd DATA103Project
    ```

2.  **Create and activate a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Streamlit application:**
    ```bash
    streamlit run app.py
    ```
    This will open the dashboard in your default web browser.

## ☁️ Deployment Instructions

You can deploy this application for free using Streamlit Community Cloud.

1.  **Push your project to a GitHub repository.** Make sure your repository includes:
    *   `app.py`
    *   `requirements.txt`
    *   All necessary data and model files (`.pkl`, `.csv`).

2.  **Sign up for Streamlit Community Cloud:**
    *   Go to [share.streamlit.io](https://share.streamlit.io) and sign up using your GitHub account.

3.  **Deploy the app:**
    *   From your Streamlit Community Cloud dashboard, click "**New app**".
    *   Select your GitHub repository and the correct branch.
    *   Ensure the "**Main file path**" is set to `app.py`.
    *   Click "**Deploy!**".

Streamlit will handle the rest, and your application will be live in a few minutes.
