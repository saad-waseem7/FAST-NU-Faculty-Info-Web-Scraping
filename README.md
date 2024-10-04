# FAST-NU Faculty Info Web Scraping:

This mini-project demonstrates how to use *web scraping techniques* to collect and process faculty information from the *FAST National University, Lahore* website. The data is organized into structured CSV files and integrated for easy analysis.

## Project Overview

The goal of this practice is to scrape faculty details from different departments at FAST-NU, Lahore, and save them in a clean, structured format. The process follows a multi-step approach, from extracting the data to integrating and merging it for detailed analysis.

### Key Objectives:

1. *Scrape Faculty Data*: Extract detailed information from multiple departments:
   - ID
   - Name
   - Designation
   - HEC Approved PhD Supervisor Status
   - Email Address
   - Department
   - Profile Image URL

2. *Additional Data Scraping*: Gather more specific information such as:
   - Office Phone Extension
   - Highest Educational Qualification

3. *Data Integration*: Combine the scraped data from different departments into a unified dataset.

### Departments Covered:
- FAST School of Computing (fsc.csv)
- Department of Electrical Engineering (ee.csv)
- Department of Civil Engineering (cv.csv)
- FAST School of Management (fsm.csv)
- Department of Science & Humanities (ss.csv)

## Process Breakdown

### 1. *Data Scraping*  
Using BeautifulSoup and requests, data is extracted from the faculty pages of each department. For each faculty member, key attributes like name, email, designation, and more are collected and saved in CSV format.

### 2. *Profile Data Enhancement*  
A secondary scraping step is performed to gather additional details from the faculty member profile pages, such as phone extensions and highest education attained. These details are saved in separate CSV files for each department.

### 3. *Data Merging*  
The department-specific data is merged to form a comprehensive dataset, providing all relevant information (including phone and education) for each faculty member. The final output is saved as fast_lhr_faculty.csv.

## How to Use

1. *Install Dependencies*:  
   Ensure you have the necessary Python packages installed:
   ```bash
   pip install requests pandas beautifulsoup4

2. *Run the Jupyter Notebook*:
   The project is implemented in a Jupyter Notebook, which contains all the scraping and data manipulation code. Open and execute the notebook to generate the output CSV files.


3. *Access Generated Files*:
After running the notebook, the following files will be generated:
- **fsc.csv, ee.csv, cv.csv, fsm.csv, ss.csv:** Department-wise faculty data
- **fsc_2.csv, ee_2.csv, cv_2.csv, fsm_2.csv, ss_2.csv:** Additional faculty data (extension and education)
- **fast_lhr_faculty.csv:** The final merged dataset with all faculty information
