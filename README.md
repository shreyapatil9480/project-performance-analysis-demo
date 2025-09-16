# Project Performance Analysis

## Overview

This project provides an end-to-end analysis pipeline for a synthetic project performance dataset. The goal is to help prospective employers understand your ability to work as a Business Analyst, Program Manager, or Data Analyst.

The dataset simulates typical project attributes (team size, estimated duration, budget, complexity, scope changes, client priority, methodology, risk level) along with calculated fields for actual duration and on-time delivery. Such an analysis is valuable for understanding factors that influence project success and for demonstrating data-driven decision-making.

## Repository Structure

- `project_data.csv` — Synthetic dataset containing 300 project records with descriptive features and outcomes.
- `analysis.ipynb` — Jupyter notebook that loads the dataset, performs exploratory data analysis (EDA), visualizes relationships, and builds predictive models (logistic and linear regression).
- `requirements.txt` — Python dependencies needed to run the notebook.

## Usage

1. **Clone the repository**:

   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   cd YOUR-REPO-NAME
   ```

2. **Create a virtual environment and install dependencies**:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

3. **Run the notebook**:

   Use Jupyter Notebook or JupyterLab:

   ```bash
   jupyter notebook analysis.ipynb
   ```

   or

   ```bash
   jupyter lab analysis.ipynb
   ```

## Dataset Details

The dataset (`project_data.csv`) includes the following columns:

| Column | Description |
|-------|-------------|
| `project_id` | Unique identifier for each project. |
| `team_size` | Number of team members assigned to the project. |
| `estimated_duration_weeks` | Estimated duration in weeks. |
| `budget_kusd` | Project budget in thousands of USD. |
| `complexity_score` | Difficulty score (1–10). |
| `scope_changes` | Number of change requests during the project. |
| `client_priority` | Priority level assigned by the client (`Low`, `Medium`, `High`). |
| `methodology` | Project management methodology (`Agile`, `Waterfall`, `Hybrid`). |
| `risk_level` | Risk assessment score (1–5). |
| `actual_duration_weeks` | Actual duration after completion. |
| `delivery_on_time` | Binary indicator (1 = delivered within 10% of estimate). |

## Notebook Contents

The `analysis.ipynb` notebook walks through the following steps:

1. **Data Loading & Summary**: Displays the first few rows and summary statistics.
2. **Exploratory Data Analysis (EDA)**: Histograms and bar charts to understand distributions of numeric and categorical variables.
3. **Correlation Analysis**: Heatmap of correlations among numeric variables and the actual duration.
4. **Feature Relationships**: Boxplots comparing numeric features across on-time and late deliveries.
5. **Predictive Modeling**:
   - Logistic Regression predicting on-time delivery.
   - Linear Regression predicting actual duration.
   - Evaluation metrics such as accuracy, confusion matrix, MAE, and RMSE.
6. **Conclusions & Next Steps**: Suggestions for further analysis and model improvement.

## How This Demonstrates Your Skills

This project demonstrates your ability to:

- Generate and work with realistic datasets.
- Perform thorough exploratory data analysis.
- Visualize and interpret key insights.
- Build and evaluate basic predictive models.
- Document your work clearly for stakeholders.

These skills align with the responsibilities of Business Analysts, Program Managers, and Data Analysts who need to make data-driven recommendations and communicate findings effectively.

## Contributing

Since this is a demonstration project created for job search purposes, further contributions are not currently being accepted. Feel free to fork the repository for your own learning or adaptation.
