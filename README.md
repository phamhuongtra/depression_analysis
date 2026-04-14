# depression_analysis

## How to run (normal)
1. Open terminal in project folder.
2. Install dependencies:
	pip install -r requirement.txt
3. Start Jupyter:
	jupyter notebook
4. Run notebooks in order:
	exploring.ipynb -> preprocess.ipynb -> question3.ipynb

## How to run (venv - Windows)
1. Create virtual environment:
	python -m venv .venv
2. Activate virtual environment (PowerShell):
	.\.venv\Scripts\Activate.ps1
3. Install dependencies:
	pip install -r requirement.txt
4. Install the notebook kernel for this venv:
	python -m ipykernel install --user --name depression_venv --display-name "Python (.venv)"
5. Start Jupyter:
	jupyter notebook
6. Open any .ipynb file and choose the kernel named "Python (.venv)".
7. Run notebooks in order:
	exploring.ipynb -> preprocess.ipynb -> question3.ipynb