# 🛒 Superstore Data Analysis

This repository contains a Jupyter Notebook that demonstrates a complete workflow for analysing the [Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final/data) using Python. It includes data loading, basic exploration, and visual insights, all crafted to help understand the structure and trends in retail business data.

## 🧠 Skills Demonstrated
- Data Cleaning & Pre-processing
- Exploratory Data Analysis (EDA)
- Data Visualization
- Business Intelligence
- Customer Segmentation
- Python (Pandas, NumPy)
- Data Storytelling
- Jupyter Notebooks
- ZIP and CSV Data Ingestion
- Retail Sales Analysis

## 📁 Dataset

The dataset is sourced from Kaggle:
**Superstore Dataset (Final)** by [vivek468](https://www.kaggle.com/vivek468)

The dataset includes order-level retail data, including:
- Order IDs
- Customer demographics
- Sales, profit, and discount figures
- Regional and product-level segmentation

## 🔍 Notebook Overview

### Key Features:
- Load a CSV file directly from a ZIP archive using `zipfile.ZipFile`
- Handle character encoding with `latin1` to avoid Unicode errors
- Perform basic exploratory data analysis (EDA)
- Generate visualizations for profit, sales, and category insights
- Identify patterns by region, category, and shipping mode

### Code Snippet: Loading Data from ZIP
```python
with ZipFile(zip_file_path) as archive:
    with archive.open(csv_file_name) as f:
        df = pd.read_csv(f, encoding='latin1')
```

## 📊 Visualizations
The notebook contains various visualizations using `matplotlib` and `seaborn` to uncover insights such as:
- Profit trends by category and region
- Distribution of shipping modes
- Top-performing segments

## 🛠️ Technologies Used
- Python 3.x
- Pandas
- Seaborn
- Matplotlib
- Jupyter Notebook

## 🚀 Getting Started

1. Clone the repository
```bash
git clone https://github.com/yourusername/superstore-analysis.git
cd superstore-analysis
```

2. Install dependencies
```bash
each Jupyter Notebook installs its own requirements 
```

3. Run the notebook
Open `001_notebook_code.ipynb` in Jupyter and execute the cells.

> Note: You will need to download the dataset from [Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final/data) and place it in the appropriate `002_data_raw/` folder.

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).

## 🙌 Acknowledgements
Thanks to [Vivek468](https://www.kaggle.com/vivek468) for making the dataset publicly available.
