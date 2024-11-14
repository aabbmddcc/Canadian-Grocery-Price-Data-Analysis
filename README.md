# Canadian Grocery Price Data Analysis

## Overview

This repository contains the files and code used to analyze grocery price trends in Canada. The project utilizes data from Project Hammer, a publicly available dataset that compiles historical grocery prices from major Canadian vendors. The analysis explores product variety, price changes over time, and vendor-specific pricing trends, with the aim of identifying patterns and providing insights into market dynamics. SQL is used for data extraction and cleaning, while Python is employed for data analysis and visualization.

## File Structure

The repository is organized as follows:

- `data`:
    - `analysis_data`: Contains cleaned and processed datasets used for specific analyses.
        - `average_price_per_item.csv`: Contains average prices per product across all vendors.
        - `price_flow.csv`: Contains data on price changes over time for each product.
        - `vender_count.csv`: Shows the count of unique products available from each vendor.

-  `script`
    - `data_analysis.sqbpro`: SQL code used for extracting and processing data from the SQLite database. This file includes queries that filter, clean, and structure the data for analysis. Files in `analysis_data` gains from here.
- `paper`: Contains the files used to generate the final report.
    - `paper.qmd`: The Quarto document that includes the analysis, narrative, and visualizations.
    - `paper.pdf`: The compiled version of the report in PDF format.
    - `references.bib`: Bibliography file with references cited in the paper.
- `llm_usage.txt`: Documents any assistance from ChatGPT-4o.

## Statement on LLM usage

Aspects of the code were written with the help of the auto-complete tool. Some conceptual clarifications and coding assistance were provided by ChatGPT, and the relevant conversation logs are documented in `llm_usage.txt`. However, the core analysis and modeling were designed and executed by the author.

## Methodology

### Data Source

The raw dataset is too large to include in this repository. You can download it from the link provided in the following line:

The data was sourced from Project Hammer, an initiative to improve transparency and competition in the Canadian grocery sector. For more information, visit [Project Hammer](https://jacobfilipp.com/hammer/).

### Key Steps

1. **Data Extraction and Cleaning**: SQL was used to query and clean the dataset, preparing it for analysis. The raw data includes time-series price information and product metadata, which were filtered and organized into analysis-ready files.
2. **Analysis**: Python was used to analyze pricing trends and vendor-specific variations:
   - **Average Price per Item**: Calculated for each product across vendors to understand price distributions.
   - **Price Changes Over Time**: Examined the changes in product prices from the earliest to the latest records to identify notable price increases or decreases.
   - **Vendor Product Variety**: Counted the unique products offered by each vendor to assess the range of inventory across different retailers.
3. **Visualization**: Key findings were visualized using Python to help interpret the data patterns effectively.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/aabbmddcc/Canadian-Grocery-Price-Data-Analysis
