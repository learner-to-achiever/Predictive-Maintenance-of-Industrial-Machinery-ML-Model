# ⚙️ Predictive Maintenance of Industrial Machinery

A machine learning project developed for an **IBM internship capstone**. This model analyzes sensor data from industrial machinery to predict potential failures before they occur, helping to prevent costly downtime.

*Analogy: This system acts like a health monitor for machinery. It continuously checks vital signs (sensor data) to predict a potential breakdown, much like a fitness tracker predicts health issues based on a person's heart rate and activity.*

---

## 🎯 Project Overview

This project aims to build and deploy a classification model that can predict the type of failure in a machine based on real-time operational data. The primary goal is to shift from a reactive "fix-it-when-it-breaks" approach to a proactive, predictive maintenance strategy.

### Key Objectives:
* Analyze sensor data to identify patterns that precede failures.
* Build a robust classification model to predict failure types.
* Deploy the model using IBM Cloud services for real-world application.

---

## 🛠️ Technology Stack

* **Languages & Libraries**: Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Plotly
* **Platform**: IBM Cloud
* **Development Environment**: Jupyter Notebook on IBM Watson Studio

---

## 📊 Dataset

The model is trained on the **AI4I 2020 Predictive Maintenance Dataset**.

* **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/AI4I+2020+Predictive+Maintenance+Dataset)
* **Instances**: 10,000 data points
* **Features**: 14 features, including:
    * `Air temperature [K]`
    * `Process temperature [K]`
    * `Rotational speed [rpm]`
    * `Torque [Nm]`
    * `Tool wear [min]`
* **Target Variable**: `Failure Type` (e.g., Tool Wear Failure, Heat Dissipation Failure, Power Failure)

---

## 🚀 Project Workflow

1.  **Data Preprocessing**: The dataset was cleaned by handling missing values and removing irrelevant columns (`UDI` and `Product ID`).
2.  **Exploratory Data Analysis (EDA)**: Extensive EDA was performed using visualizations like histograms, heatmaps, and count plots to uncover insights and correlations between sensor readings and machine failures.
3.  **Feature Engineering**: The categorical `Type` feature was converted into numerical format using one-hot encoding.
4.  **Model Building**: The data was split (80% train, 20% test). A **Random Forest Classifier** was selected after evaluating its performance against other models.
5.  **Model Evaluation**: The model was assessed using key metrics:
    * **Accuracy**: 98.6%
    * **Precision**: High precision across all failure types.
    * **Recall & F1-Score**: Strong scores indicating a balanced model.
    * **Confusion Matrix**: Visualized to confirm the model's predictive accuracy for each class.
6.  **Deployment**: The trained model was successfully deployed on the **IBM Cloud** platform, making it accessible for real-time predictions via an API endpoint.

---

## 📈 Key Results & Visualizations

The Random Forest model demonstrated excellent performance in identifying potential machine failures.

*A key finding from EDA was the strong correlation between `Torque`, `Rotational Speed`, and machine failure, which became important features for the model.*

---

## 🔧 How To Use

To get this project running locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/learner-to-achiever/Predictive-Maintenance-of-Industrial-Machinery-ML-Model.git](https://github.com/learner-to-achiever/Predictive-Maintenance-of-Industrial-Machinery-ML-Model.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Jupyter Notebook:**
    Launch the `Predictive-Maintenance-of-Industrial-Machinery.ipynb` notebook to see the step-by-step process.

---

## 📜 License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.
