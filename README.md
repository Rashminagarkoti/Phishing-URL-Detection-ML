# Phishing URL Detection Using Machine Learning

## Project description
This student project builds a baseline machine-learning model to classify URL text as **potential phishing (label 0)** or **likely legitimate (label 1)**. It uses character-level TF–IDF features and Logistic Regression. The notebook includes data cleaning, exploratory analysis, a stratified train/test split, evaluation metrics, a confusion matrix, and a function for testing a URL string without visiting it.

This is an educational prototype, not a production anti-phishing product. Model predictions can be wrong and are not proof that a website is safe.

## Dataset
- **Repository:** https://github.com/RajaMuhammadAwais/phishing-url-dataset
- **CSV download used by notebook:** https://raw.githubusercontent.com/RajaMuhammadAwais/phishing-url-dataset/master/phishing_url_dataset.csv
- **Expected columns:** `URL`, `Label`
- **Labels:** `0 = phishing`, `1 = legitimate`
- The notebook cleans the data and uses a reproducible sample of up to 40,000 rows by default to make training more manageable on a student computer.

Please review the dataset repository's source notes and terms before reuse. Dataset availability and contents may change.

## Technologies used
- Python
- Jupyter Notebook
- pandas and NumPy
- Matplotlib
- scikit-learn (TF–IDF, Logistic Regression, model evaluation)

## Setup and run
1. Install Python 3.10 or newer.
2. Download or clone this project folder.
3. Open a terminal in the project folder and create a virtual environment (recommended):
   - Windows: `python -m venv .venv` then `.venv\\Scripts\\activate`
   - macOS/Linux: `python3 -m venv .venv` then `source .venv/bin/activate`
4. Install dependencies: `python -m pip install -r requirements.txt`
5. Start Jupyter: `jupyter notebook`
6. Open `Rashmi_PhishingURLDetection.ipynb` and run cells from top to bottom. An internet connection is needed to download the dataset.
7. Review the generated metrics and confusion matrix. Use only the values actually produced by your run in your final report.

## Project files
- `Rashmi_PhishingURLDetection.ipynb` — complete code and explanation
- `requirements.txt` — Python dependencies
- `Rashmi_ProjectReport.docx` — project report
- `README.md` — this file

## Safety and limitations
The notebook never opens or visits URLs. Do not open suspicious links for testing. The classifier analyses URL text only and can make false predictions; do not rely on it as the only security control.

## References
- Dataset repository: https://github.com/RajaMuhammadAwais/phishing-url-dataset
- scikit-learn: https://scikit-learn.org/stable/
- pandas: https://pandas.pydata.org/docs/
