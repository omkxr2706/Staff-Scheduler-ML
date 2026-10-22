# Staff Scheduler for Part-Time Jobs

An **Machine Learning-based Staff Scheduler** project designed to support restaurant workforce planning by analyzing workload, traffic, and employee-related factors. The project uses a neural-network-based regression model to estimate employee satisfaction and provides a foundation for data-driven staff scheduling decisions.

## 📌 Project Overview

Managing part-time staff in restaurants can be challenging due to changing customer traffic, varying workloads, and employee satisfaction. This project explores how machine learning can help analyze these factors and support better scheduling decisions.

The project uses a Multi-Layer Perceptron (MLP) regression model to learn patterns from restaurant scheduling data and predict employee satisfaction.

## ✨ Features

- Machine learning-based employee satisfaction prediction.
- Analysis of restaurant traffic and workload.
- Dataset-driven model training and evaluation.
- Saved model and scaler files for reuse.
- Streamlit-based interface for interactive usage, if configured in the application.
- Restaurant staff scheduling dataset for experimentation.

## 🛠️ Technologies Used

- **Python** — Core programming language.
- **Pandas** — Data handling and analysis.
- **NumPy** — Numerical operations.
- **Scikit-learn** — Machine learning model and preprocessing.
- **Joblib** — Saving and loading trained model artifacts.
- **Streamlit** — Interactive web application, if supported by the selected entry point.

## 📁 Project Structure

```text
Staff-Scheduler-ML/
├── app.py
├── streamlit_app.py
├── model.py
├── dataset.py
├── restaurant_staff_schedule.csv
├── mlp_model.joblib
├── scaler.joblib
├── MIS_Report.xlsx
├── requirements.txt
└── README.md
```

**File descriptions**

- `app.py` — Application entry point; check the file to confirm its exact functionality.
- `streamlit_app.py` — Streamlit interface, if configured for interactive use.
- `model.py` — Machine learning model implementation.
- `dataset.py` — Dataset-related processing or loading logic.
- `restaurant_staff_schedule.csv` — Restaurant staff scheduling dataset.
- `mlp_model.joblib` — Saved machine learning model.
- `scaler.joblib` — Saved preprocessing scaler.
- `MIS_Report.xlsx` — Project report or supporting documentation.
- `requirements.txt` — Python dependencies.

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Staff-Scheduler-ML.git
cd Staff-Scheduler-ML
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Create a virtual environment

**Windows (Command Prompt):**

```bash
python -m venv venv
venv\Scripts\activate
```

**Windows (PowerShell):**

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

**macOS/Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If installation fails, check that you are using a compatible Python version and that the required packages are listed in `requirements.txt`.

## ▶️ How to Run

### Option 1: Run the Streamlit interface

If `streamlit_app.py` contains the application's Streamlit interface, run:

```bash
streamlit run streamlit_app.py
```

### Option 2: Run the main application

If `app.py` is the intended entry point, run:

```bash
python app.py
```

Use the entry point that matches the application's implementation. These commands are alternatives; you do not necessarily need to run both.

## 🧠 Machine Learning Approach

The project uses a **Multi-Layer Perceptron Regressor (MLPRegressor)**, a neural-network-based model for regression tasks.

The model implementation uses hidden layers of 64 and 32 neurons, as configured in the model code.

The documented input features include:

- `restaurant_id`
- `avg_traffic`
- `workload`
- `burnout`

The target described for the model is employee satisfaction.

The saved model and scaler can be reused for predictions when the input features and preprocessing match those used during training.

## 📊 Dataset

The project includes `restaurant_staff_schedule.csv`, which contains the data used for the machine learning workflow.

Before training or making predictions, verify the dataset's column names, data types, missing values, and target variable against the implementation in `model.py` and `dataset.py`.

## 📈 Model Evaluation

Model performance should be assessed using metrics appropriate for regression, such as:

- **Mean Squared Error (MSE)** — Measures the average squared prediction error.
- **R² Score** — Indicates how much variation in the target is explained by the model.

Actual evaluation results should be added here after running the model and verifying the output. No performance figures are claimed in this README.

## 🚀 Future Improvements

- Develop an automated staff scheduling optimizer.
- Account for employee availability and shift preferences.
- Add constraints for working hours, rest periods, and staffing requirements.
- Improve the interface with schedule visualizations.
- Evaluate the model on additional restaurant scheduling data.
- Compare multiple machine learning models.

## 🎓 Project Purpose

This project explores the use of machine learning in restaurant workforce planning and employee satisfaction analysis. It can serve as a starting point for developing more comprehensive staff scheduling and optimization solutions.

## 📄 License and Attribution

Check the original repository's license before redistributing or modifying its code. Add the appropriate license and attribution information here.

If this project builds on another developer's work, acknowledge the original author and repository.

---

**Repository:** `Staff-Scheduler-ML`
