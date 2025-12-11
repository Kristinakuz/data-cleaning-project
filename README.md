# Project Overview: <br>
This project is a real-world data cleaning simulation designed to practice data wrangling and documentation. It includes a small retail data set and a large HR dataset to imitate the types of data analysts often work with in industry. The goal of this project is to apply multiple tools (Excel, Python, notebooks) and produce clean, analytic-ready datasets.
<br>
## Project Structure 
data/               → Raw and cleaned datasets (CSV and Excel) <br>
notebooks/          → Jupyter notebooks used for exploratory cleaning and analysis <br>
excel/              → Excel cleaning work, formulas, and Power Query steps <br>
documentation/      → Data quality report, cleaning rules, issue logs, screenshots <br>
scripts/            → Python scripts for automated data cleaning <br>
## Tools and File Formats Used
### Tools Used
- Excel - for manual cleaning, formulas and Power Query <br>
- Python (pandas) - For programmatic cleaning of small and large datasets <br>
- Jupyter Notebooks - To display code, output and explanations together <br>
- Git & Github - For version control and organizing the project <br>
### File Formats
- CSV - Raw and cleaned datasets <br>
- XLSX - Excel-based cleaning and formula work <br>
- IPYNB - Python cleaning workflows <br>
- PY - Automation scripts
- MD - Documentation and reports <br>
- PNG - Screenshots for visual documentation
## Real-World Data Issue Addressed
This project intentionally includes a wide range of common data problems frequently found in retail and business datasets. <br>
These include:

- Duplicate records <br>
- Inconsistent name formatting <br>
- Invalid or malformed email addresses <br>
- Multiple phone number formats and missing values <br>
- Mixed and incorrect date formats <br>
- Inconsistent state abbreviations and casing <br>
- Numerical errors such as text-based values, negative totals, or mismatched calculations <br>
- Payment method inconsistencies across categories <br>
- Missing values across multiple fields <br>

The purpose is to simulate the type of messy real-world data that analysts clean every day and demonstrate the tools and logic required to transform it into a usable dataset.
## Data Cleaning Steps & Methods (Small Retail Dataset)
This section documents the complete cleaning workflow performed ont he small retail dataset. The goal was to transform a messy, inonsisten file into a clean, analysis-ready dataset while demonstrating real-worl data claning techniques. <br>
During profiling, the following issues were found:
#### Customer Name
- Inconsistent capitalization
- Extra spaces
- Incorrectly formatted names
- Missing values
#### Email
- Missing “@”
- Double “@@”
- Missing .com
- Domain typos (gmailcom.com)
- Hyperlinked vs. plain text
- Missing emails
#### Phone Number
- Mixed formats
- Invalid length
- Text entries
- Blanks
- Extra whitespace
#### Order Date
- Multiple formats
- Text values instead of serial dates
- Day-first vs. month-first inconsistencies
- Two-digit vs four-digit
#### State
- Mixed cases
- Full state names vs. abbreviations
#### Product
- Inconsistent naming
- Misspellings
- Hyphens and spacing inconsistent
#### Quantity
- Text instead of numeric
- Improper number formats
#### Unit Price
- $ symbols
- Parentheses representing negtive values
- Missing decimals
#### Total Amount
- Incorrect values
- Needed recalculation
#### Payment Method
- Typos
- Abbreviations
- Multiple naming styles
- Blank entries
## Cleaning Techniques Used
  #### String Functions
  - TRIM
  - LOWER
  - UPPER
  - PROPER
  - SUBSTITUTE
  #### Conditional Logic
  - Nested IF statements to standardize values and handle exceptions.
  #### Date Conversion
  - DATEVALUE
  - SUBSTITUTE
  #### NUMERIC VALIDATION
  - ISNUMBER, digit counting, and type conversion for quantity and price.
  #### Text Normalization
  - State abbreviations, product naming, payment method mapping
  #### Final Replacement
  - After validating helper columns, cleaned values were pasted back as values into original columns.
## Final Cleaned Fields
The final dataset includes: <br>
- Cleaned Customer Name
- Cleaned Email
- Cleaned Phone Number
- Standardized Order Date
- Normalized State
- Cleaned Product Name
- Numeric Quantity
- Numeric Unit Price
- Corrected Total Amount
- Standardized Payment Method
## Skills Demonstrated
- Data profiling
- Text normalization
- Data validation
- Standardization workflows
- Reconciliation & recalculation
- Documentation of a reproducible cleaning process
  
  
