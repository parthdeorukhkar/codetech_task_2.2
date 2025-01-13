# codetech_task_2.2

Name:Parth Deorukhkar

Company:CODETECH IT SOLLUTION

ID:CT08EIV

Domain:Python

Duration:Dec17 to Jan 17

Mentor:Neela Santosh Kumar



Data Analysis and PDF Report Generator
This Python script reads a dataset (in CSV format), performs basic statistical analysis, and generates a PDF report with the analysis summary using the FPDF library.

Features
Reads data from a CSV file using pandas.
Computes summary statistics for numerical columns in the dataset.
Automatically generates a structured PDF report containing the analysis.
Requirements
Ensure the following dependencies are installed:

Python 3.x
Libraries:
pandas
fpdf
Install the libraries using pip:

bash
Copy code
pip install pandas fpdf
Setup and Usage
Place your CSV file in the same directory as the script.

Update the input_file variable in the script with the name of your CSV file.

Run the script using the following command:

bash
Copy code
python script_name.py
Replace script_name.py with the name of your script file.

The script will generate a PDF report named report.pdf in the same directory.

Code Breakdown
1. read_and_analyze_data Function
Reads data from the provided CSV file path using pandas.read_csv().
Computes summary statistics for numerical columns using pandas.DataFrame.describe().
2. generate_pdf_report Function
Creates a PDF file using the FPDF library.
Adds a title and summary statistics from the dataset to the PDF.
Saves the PDF to the specified output file path.
3. Main Script
Reads data from a CSV file.
Analyzes the data and generates a PDF report.
Handles errors (e.g., file not found or invalid data).
Example Workflow
Input CSV File (data.csv):
Sample dataset:

Name	Age	Salary
Alice	25	50000
Bob	30	60000
Charlie	35	70000
Generated Summary:

Age:
count: 3.0, mean: 30.0, std: 5.0, min: 25.0, max: 35.0
Salary:
count: 3.0, mean: 60000.0, std: 10000.0, min: 50000.0, max: 70000.0
Output PDF (report.pdf):

Title: Data Analysis Report
Summary Statistics for each numerical column.
Known Issues
Assumes all data is clean and numerical columns are present.
Limited formatting in the PDF (can be enhanced for better visualization).
Future Enhancements
Add support for visualizations (e.g., bar charts, histograms) in the PDF.
Automatically detect and handle missing or invalid data.
Support more file formats (e.g., Excel, JSON).

