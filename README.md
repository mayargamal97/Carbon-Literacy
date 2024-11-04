# Carbon Literacy Training Analysis in Kenya's Hospitality Sector

This repository contains data analysis and visualization work for assessing the impact of carbon literacy training in Kenya’s hospitality sector. The project aims to demonstrate how sustainability initiatives influence energy savings, carbon reduction, and revenue impact.

## Project Overview

This analysis focuses on:
- **Estimated Carbon Reduction** and **Energy Savings** due to training.
- The **impact of pre- and post-training initiatives** on sustainability KPIs.
- The **revenue impact** from eco-conscious practices.

The **data cleaning and transformation** was performed using Python, while the **visualizations** were developed in Power BI.

## Repository Contents

- **`pph.ipynb`**: Jupyter notebook containing the Python code for data cleaning and transformation.
- **`carbon.png`**: Power BI dashboard visualizing the insights from the cleaned data.
- **`final_dataframe.csv`**: Cleaned dataset in CSV format, ready for analysis and visualization.

## Data Cleaning Techniques

The data cleaning process involved the following steps:

1. **Standardizing Text**:
   - Converted text in relevant columns (e.g., `KPI_Area`, `Global_Benchmark`, `Pre_Training`, `Post_Training`, `Estimated_Carbon_Reduction`, `Revenue_Impact`) to lowercase and removed any leading or trailing whitespace for consistency.

2. **Removing Parenthetical Information**:
   - Used regular expressions to remove any text within parentheses across several columns, keeping only the essential information.

3. **Extracting Percentage Values**:
   - Defined a custom function, `extract_percentage`, to capture and extract percentage values from text in the `Global_Benchmark`, `Post_Training`, and `Estimated_Carbon_Reduction` columns.
   - Extracted percentages were stored in new columns like `Post_Training_Percentage` and `Estimated_Carbon_Reduction_percentage`.

4. **Splitting Columns**:
   - Split the `Post_Training` column into separate columns for text and percentages, creating `Post_Training_Percentage`.
   - A similar approach was applied to the `Estimated_Carbon_Reduction` column.

5. **Refining Revenue Impact Data**:
   - Removed any text after a colon (":") in the `Revenue_Impact` column to retain only the primary revenue impact description.

6. **Removing Periods**:
   - Removed periods from all columns to maintain consistency across the dataset.

## Instructions to Set Up the Repository

1. **Initialize the Repository on GitHub**:
   - Go to your GitHub account, create a new repository, and name it (e.g., `Carbon_Literacy_Analysis`).
   - Add a description and select "Add a README file".

2. **Clone the Repository**:
   - Clone the repository to your local machine:
     ```bash
     git clone https://github.com/yourusername/Carbon_Literacy_Analysis.git
     ```

3. **Add Files to the Repository**:
   - Copy `pph.ipynb`, `carbon.png`, and `final_dataframe.csv` to your cloned repository folder.

4. **Commit and Push Files**:
   - Use the following commands to upload your files to GitHub:
     ```bash
     git add .
     git commit -m "Initial commit with data cleaning notebook, Power BI dashboard, and cleaned data"
     git push origin main
     ```

## Viewing the Power BI Dashboard

The Power BI dashboard provides a comprehensive view of the project's key insights. It visualizes metrics such as:
- Estimated Carbon Reduction and Energy Savings.
- Post-training energy savings and carbon reduction by KPI area.
- Revenue impact from sustainability initiatives.
  
![carbon](https://github.com/user-attachments/assets/7fdab0cb-f77e-4715-9350-b1dc34d3adc6)

## License

This project is licensed under the MIT License.

---

Feel free to reach out if you have any questions or suggestions.
