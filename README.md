# Customer Segmentation and Product Analysis

This repository contains a Jupyter Notebook (or Python script) and a summary of findings for a customer segmentation and product analysis project conducted. The goal of this project was to identify the most profitable customer segments and best-selling products to help the marketing department focus their efforts effectively.

## Question

The marketing department at iGnosis Tech needed assistance in identifying their most valuable customer segments and top-performing products. Instead of a broad marketing approach, they sought a data-driven strategy to target specific customer groups and optimize product promotion. This analysis aims to provide actionable insights based on transaction data.

## Dataset

The dataset used for this analysis was provided by iGnosis Tech and includes two CSV files:

*   `purchase_behaviour.csv`: Contains customer demographic information.
*   `transaction_data.csv`: Contains transaction details, including product purchases and sales values.

The data can be downloaded from [this link](https://drive.google.com/drive/folders/1JLHEIQp95b6Jo3iiXGYfIdKUrs8uWJn1?usp=sharing).

## Methodology

The analysis involved the following steps:

1.  **Data Loading and Exploration:** The CSV files were loaded using pandas, and basic information about the data was displayed to understand the structure and identify any missing values.
2.  **Data Cleaning and Preprocessing:** The `DATE` column in the transaction data was converted to datetime format. A `TOTAL_SPEND` feature was engineered by calculating the product of `QTY` and `SALES_VALUE`.
3.  **Data Merging:** The two datasets were merged based on the common key `LYLTY_CARD_NBR` to combine customer demographics with transaction details.
4.  **Top Product Identification:** The top 3 most profitable products were identified by grouping the data by `PROD_NAME` and summing the `TOTAL_SPEND`.
5.  **Loyal Customer Identification:** The top 10 most loyal customers were identified based on their total spend (`TOTAL_SPEND`).
6.  **Customer Segment Analysis:** Customer segments were analyzed by grouping the data by `LIFESTAGE` and `PREMIUM_CUSTOMER` and calculating the total spend for each segment. This was visualized using a bar plot.
7.  **Hypothesis Generation:** Hypotheses were formulated to explain the observed spending patterns of different customer segments.

## Findings

The key findings from the analysis include:

*   Older families are the highest spending customer segment.
*   Budget & Premium older families represent a particularly valuable target segment.
*   Younger customer segments show potential for increased spending over time.

Further details and hypotheses are provided in the Jupyter Notebook and the Summary File.

## Repository Contents

*   `main.ipynb`: The Jupyter Notebook containing the code for the analysis.
*   `README.md`: This file, providing an overview of the project.
*   `purchase_behaviour.csv`: Customer demographic data.
*   `transaction_data.csv`: Transaction data.

## How to Run the Code

1.  Clone the repository: `git clone https://github.com/UtkarshPrajapati/Customer-Segmentation.git`
2.  Navigate to the repository directory: `cd Customer-Segmentation`
3.  Download the datasets from the provided link and place them in the same directory as the notebook.
4.  Install the required libraries: `pip install pandas numpy matplotlib seaborn`
5.  Run the Jupyter Notebook: `jupyter notebook main.ipynb`.

## Contact

For any questions or inquiries, please contact [utkarshprap@gmail.com](mailto:utkarshprap@gmail.com).