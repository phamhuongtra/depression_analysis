# depression_analysis

This project studies survey data about depression to understand which lifestyle and personal factors are associated with depression risk, and then builds machine learning models to predict the `Depression` label.

## Project Overview
The dataset includes factors such as dietary habits, sleep duration, work/study hours, academic pressure, work pressure, profession, family history, and related interaction features. The project first explores how these factors relate to depression, then prepares the data, engineers new features, and finally compares several models to find the best approach for depression-risk prediction.

In short, this repository answers two questions:
1. Which lifestyle factors seem to be related to depression?
2. Which model performs best for predicting depression from survey data?

## Project Structure
- `data/`: input data files and prepared datasets used by the notebooks.
- [01.data_exploring.ipynb](01.data_exploring.ipynb): Phase 1, explore the survey data and understand the target label and key variables.
- [02.preprocessing.ipynb](02.preprocessing.ipynb): Phase 2, clean the raw data, handle missing values, and prepare the dataset for analysis.
- Phase 3, data mining experiments on depression-related lifestyle questions:
	- [03.datamining_question1.ipynb](03.datamining_question1.ipynb): check whether lifestyle habits such as diet, work/study hours, and sleep are linked to depression.
	- [03.datamining_question2.ipynb](03.datamining_question2.ipynb): compare depression patterns between students and working professionals, including gender, age, profession, pressure, and financial stress.
	- [03.datamining_question3.ipynb](03.datamining_question3.ipynb): analyze the role of family history and how it interacts with pressure in depression risk.
- [04.feature_engineering.ipynb](04.feature_engineering.ipynb): Phase 4, build the final modeling dataset by creating grouped features, interaction features, and habit-based features from the earlier analysis.
- [05.model.ipynb](05.model.ipynb): Phase 5, train and compare Random Forest, LightGBM, and CatBoost on train/validation/test splits, then tune thresholds and review feature importance for the best model.

## How to Run

### Local Python
1. Open a terminal in the project folder.
2. Install dependencies:
	`pip install -r requirement.txt`
3. Start Jupyter:
	`jupyter notebook`
4. Open the notebook you want to run and execute the cells.

### Windows Virtual Environment
1. Create a virtual environment:
	`python -m venv .venv`
2. Activate it in PowerShell:
	`.\.venv\Scripts\Activate.ps1`
3. Install dependencies:
	`pip install -r requirement.txt`
4. Register the kernel for Jupyter:
	`python -m ipykernel install --user --name depression_venv --display-name "Python (.venv)"`
5. Start Jupyter:
	`jupyter notebook`
6. Open any notebook and select the kernel named `Python (.venv)`.

### Google Colab
1. Upload the notebook to Colab or open it from GitHub.
2. Run the cells in order.
3. The notebooks are configured to load data from both local and remote sources, so they can run without local files if needed.

## Notes
The detailed analysis and notebooks are written in Vietnamese for local research purposes.