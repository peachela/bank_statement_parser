# Bank Statement PDF Parser

> 🚧 Status: In Development

## Project Background
This project was developed as a practical self-learning exercise in Python, combining real-world financial data processing with programming fundamentals.

## Problem Statement
Bank statements are provided in PDF format. Manual verification of transactions against invoices and balance sheet items is time consuming
and error prone. This tool automates the extraction and structuring of transaction data to support financial control and audit processes.

## Approach
Before building the parser, an exploratory script is used to understand the PDF structure. This is a common professional practice in data work, sometimes referred to as Exploratory Data Analysis (EDA).

The pipeline follows these steps:

1. **Explore** — open and observe the PDF structure
2. **Identify** — locate the relevant tables and patterns
3. **Extract and Parse** — loop through pages one at a time, extract each page's table, parse immediately, then append to the growing dataset
4. **Structure** — combine all parsed pages into a clean table using pandas
5. **Output** — export to Excel and CSV
6. **Analyse** — aggregations, matching and visualisation

## Technical Skills Demonstrated
- PDF parsing with pdfplumber
- Pattern recognition using regular expressions
- Dutch SEPA payment format parsing
- Data pipeline design
- Error handling and data quality control
- Data transformation with pandas
- Excel output with openpyxl

## Libraries Used
- pdfplumber
- pandas
- openpyxl
- re (built-in Python)

## Project Structure
  explore_pdf.py        #explore and understand the PDF structure
  parse_statement.py    #full parsing pipeline
  README.md
  
## Note on Data Privacy
This project was developed using private financial documents.
No real bank statements or transaction data are included in this repository. A synthetic dummy dataset is provided for demonstration purposes only.
