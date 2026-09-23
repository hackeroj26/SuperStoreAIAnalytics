# AI-Powered Superstore Sales Analysis

## Project Overview
This project analyzes the Sample Superstore sales dataset using Python and adds an AI-assisted business analysis layer using Google Gemini.

The project focuses on:
- Sales and profit performance
- Category-level performance
- Regional performance
- Discount and profitability relationships
- Product-level performance
- AI-generated business insights and recommendations

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Google Gemini API
- Google Colab / Jupyter Notebook
- Excel dataset

## Dataset
The project uses the Sample Superstore dataset supplied for the internship project.

Dataset filename used in the notebook:
`sample_-_superstore.xls`

If your submission portal requires an external dataset URL, use the official/public dataset source specified by your internship instructions or the source from which you originally obtained the dataset. The dataset itself is not embedded in the notebook.

## How to Run

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Open the notebook
Open:
`Ojas_Singh_AI_Superstore_Analysis.ipynb`

Google Colab is recommended.

### 3. Upload the dataset
Run the upload cell and select:
`sample_-_superstore.xls`

### 4. Configure Gemini API key
In Google Colab:
1. Open the **Secrets** panel.
2. Add a secret named `GEMINI_API_KEY`.
3. Paste your Gemini API key.
4. Enable notebook access for the secret.

Do **not** put the API key directly inside the notebook.

### 5. Run all cells
The notebook will:
1. Load and inspect the dataset.
2. Calculate KPIs.
3. Analyze categories and regions.
4. Analyze discounts and profit margins.
5. Show interactive charts.
6. Connect to Gemini.
7. Generate AI-assisted business insights.
8. Print a final project summary.

## Key Project Outputs
The analysis produces:
- Total Sales
- Total Profit
- Number of Orders
- Overall Profit Margin
- Sales by Category
- Profit by Region
- Profit Margin vs Discount
- Top products by sales/profit
- AI-generated observations and recommendations

## AI Component
Gemini is used only after the numerical analysis is performed. The notebook sends aggregated metrics and summary tables to the model and asks it to identify business observations and practical recommendations.

The notebook includes retry handling for temporary Gemini service errors.

## Security
The API key is retrieved from Colab Secrets using:
`userdata.get("GEMINI_API_KEY")`

No API key should be written into the source code or submitted files.

## Project Structure
```text
Ojas_Singh_AI_Superstore_Analysis.ipynb
requirements.txt
README.md
Ojas_Singh_AI_Superstore_Analysis.docx
```

## Author
**Ojas Singh**

## Academic Project
IBM SkillsBuild Data Analytics with AI Academic Internship Program
