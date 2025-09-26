# Data Analyst Internship - Task 2


# Task_2_Data_Visualization

**Contents**
- `superstore.csv` - Synthetic Superstore sales dataset (n=1200 rows)
- `visualization.ipynb` - Notebook that loads the CSV and recreates key charts
- `dashboard.png` - Combined dashboard screenshot (4 charts)
- `README.md` - This file

**Summary**
I generated a realistic Superstore-style dataset and created a simple dashboard to show:
- Sales by Region
- Monthly Sales trend (2018-2020)
- Sales by Category
- Profit vs Discount relationship

**How the data was generated**
- 2018-01-01 to 2020-12-31 order dates
- Regions, categories, sub-categories and products were synthesized
- Sales, Discount and Profit computed with plausible margins and random variation for realism

**How to run**
1. Open `visualization.ipynb` in Jupyter (it expects `superstore.csv` in the same directory).
2. Run all cells to reproduce the charts and adapt them for Tableau/Power BI if needed.

**Notes & Next steps (if you want enhancements)**
- Add interactive dashboard using Tableau or Power BI and save PDF screenshots to `dashboard.pdf`.
- Add filters (Region, Category, Ship Mode) and highlight actions for storytelling.
- Improve product naming and add more customer-level segmentation for deeper analysis.

---

## Tableau / Power BI Instructions

### Tableau
1. Open Tableau Desktop or Tableau Public.
2. Connect to `superstore.csv`.
3. Create the following views:
   - **Sales by Region**: Drag `Region` to Columns, `Sales` to Rows, change to Bar Chart.
   - **Monthly Sales Trend**: Drag `Order Date` to Columns (set to Month), `Sales` to Rows, Line Chart.
   - **Sales by Category**: Drag `Category` to Columns, `Sales` to Rows, Bar Chart.
   - **Profit vs Discount**: Scatter Plot with `Discount` on X-axis, `Profit` on Y-axis.
4. Arrange all four into a Dashboard layout and export as image/PDF.

### Power BI
1. Open Power BI Desktop.
2. Load `superstore.csv`.
3. Create visuals:
   - Clustered Bar: Region vs Sales.
   - Line Chart: Order Date (month) vs Sales.
   - Bar Chart: Category vs Sales.
   - Scatter Plot: Discount vs Profit.
4. Arrange them in the report view, export report as PDF or PNG.

---

## GitHub Repository Setup

To prepare a GitHub-ready repository:

1. Create a folder named `Task_2_Data_Visualization`.
2. Place these files inside:
   - `superstore.csv`
   - `visualization.ipynb`
   - `dashboard.png`
   - `dashboard.pdf`
   - `README.md`
3. (Optional) Add a `.gitignore` file to exclude temporary files:
   ```gitignore
   .ipynb_checkpoints/
   __pycache__/
   *.pyc
   *.pyo
   *.pyd
   *.DS_Store
   ```
4. Initialize git and push to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Add Task 2 Data Visualization project"
   git branch -M main
   git remote add origin <https://github.com/chauhanlokender5-dotcom/Task-2-Data-Visualization>
   git push -u origin main
   ```

This setup makes the project reproducible and shareable.
