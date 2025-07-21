# McGill Football Analytics Automation Project

---

## Table of Contents
1.  [Description](#description)
2.  [Tech Assets and URLs](#tech-assets-and-urls)
3.  [Installation](#installation)
4.  [Usage](#usage)
5.  [Features](#features)
6.  [Data Sources](#data-sources)
7.  [Troubleshooting](#troubleshooting)
8.  [Costs Involved](#costs-involved)
9.  [Passwords and Credentials](#passwords-and-credentials)
10. [Contact Information](#contact-information)

---

## Description
This project was developed as part of a community collaboration with the McGill Football team to support their coaching staff. The primary purpose is to transform their manual, time-consuming data analysis workflow into an automated, efficient, and sustainable process. The project delivers two distinct solutions:

*   **Stream A (In-Game Analytics):** An automated reporting suite designed to provide the coaching staff with immediate, actionable insights from their DVSport game data. This stream focuses on turning raw play-by-play data into 10 standardized strategic reports.
*   **Stream B (External Data Integration):** A data pipeline to scrape and analyze Twitter (X) data related to competitor programs, providing a new dataset to inform community engagement and recruitment strategies.

---

## Tech Assets and URLs
This project consists of the following key assets, organized into folders for each stream:

*   **`For Maxime - DVSport Report Support/`**
    *   `DVSport 10 Reports Prototype.ipynb`: A Jupyter Notebook containing the Python code and logic used to validate and prototype all 10 strategic reports.
    *   `DVSport Reports 9 & 10.xlsx`: The client-facing Excel workbook for the two most complex reports, which update automatically when new data is pasted.
    *   `DVSport Data Dictionary.xlsx`: A comprehensive guide defining all abbreviated columns from the raw DVSport data.
*   **`For Chris - Twitter Data Scraping/`**
    *   `Twitter_Ivy_League_List.ipynb`: A Jupyter Notebook containing the functional Python pipeline for scraping and processing Twitter data.
*   **`Project Report.pdf`**: The comprehensive final report detailing the project's background, methodology, findings, and recommendations.
*   **`ReadMe - McGill Football`**: This handoff document.
*   **GitHub Repository:** [Link to your private GitHub repository]

---

## Installation
Step-by-step instructions on how to install and set up the project.

### Prerequisites
*   **For DVSport & Excel Reports (Maxime's Stream):**
    *   Microsoft Excel
*   **For Twitter Data Pipeline (Chris's Stream):**
    *   Python 3.7+
    *   Required Python libraries: `pandas`, `snscrape`.

### Step-by-Step Installation
**Maxime's Stream:**
*   No installation is required. The primary solution is automated within the DVSport "Defaults List," and the supplementary reports are in a standard `.xlsx` file.

**Chris's Stream:**
1.  Ensure Python 3.7 or higher is installed.
2.  Open a terminal or command prompt.
3.  Install the necessary libraries by running the following command:
    ```bash
    pip install pandas snscrape
    ```

---

## Usage
Instructions on how to use the project deliverables.

### Maxime’s Reports (Automated Workflow)
*   **In-Platform Reports (Reports 1-8):**
    1.  Create a new game or project in the DVSport system.
    2.  The 8 core reports will be **automatically generated** and populated with the new data from the "Defaults List." No further action is required.
*   **Excel Reports (Reports 9 & 10):**
    1.  Export the complete raw dataset for the desired game from DVSport.
    2.  Open the `DVSport Reports 9 & 10.xlsx` file.
    3.  Navigate to the **"Data-Input"** tab and paste the raw data.
    4.  The pivot tables and visuals in the "Report 9" and "Report 10" tabs will **update automatically**.

### Chris’s Twitter Pipeline
*   **Example Usage:**
    1.  Open the `Twitter_Ivy_League_List.ipynb` Jupyter Notebook.
    2.  Locate the configuration section at the top of the notebook.
    3.  Modify the search parameters (keywords, accounts, start/end dates) as needed.
    4.  Run the cells sequentially from top to bottom.
    5.  A `.csv` file containing the structured tweet data will be saved to the `output/` directory.

---

## Features

### Maxime’s DV Sport Reports
*   A suite of 10 structured analytical reports (8 fully automated in DVSport, 2 in a supporting Excel template).
*   Dual "Global" and "Subgroup" views for both high-level and detailed tendency analysis.
*   Breakdowns by Personnel, Formation, Down & Distance, and Field Zone.
*   Directional tendency analysis (Left/Right and Field/Boundary).
*   A custom yardage attribution model for Offensive Line vs. Running Back performance.
*   Designed for **non-technical reuse** by the coaching staff.

### Chris’s External Integration Stream
*   Configurable, real-time tweet scraping using `snscrape`.
*   Outputs structured CSV files ready for use in Excel, BI tools, or other models.
*   A well-documented prototype for future integration with the official Twitter API v2.

---

## Data Sources
*   **Internal Data:** Game-by-game Excel/CSV exports from the **DVSport platform**.
*   **External Data:** **Twitter (X)** via the `snscrape` library.

---

## Troubleshooting

### Maxime’s Reports
*   **Issue:** Excel reports show old data after pasting new data.
    *   **Solution:** In Excel, navigate to the `Data` tab and click `Refresh All`.
*   **Issue:** Excel reports are broken or show errors.
    *   **Solution:** Ensure the pasted data in the "Data-Input" tab has the exact same column structure as the original raw data export.

### Chris’s Scripts
*   **Issue:** Error `ModuleNotFoundError: No module named 'snscrape'`.
    *   **Solution:** The required libraries are not installed. Run `pip install pandas snscrape` in your terminal.
*   **Issue:** The script runs but no output file is generated.
    *   **Solution:** Check that the date formats in the configuration are correct (YYYY-MM-DD) and that the script has permission to write files in the project folder.

---

## Costs involved
*   All solutions delivered were built using free, open-source tools (Python, `snscrape`) or existing client software (DVSport, Excel). There are **no immediate costs** required to use these deliverables.
*   Future enhancements, such as using the official Twitter API v2 for robust historical data, would require a paid subscription to the API.

---

## Passwords and credentials
*   No passwords or credentials are required for the current implementation of the DVSport reports or the `snscrape` script.
*   The `Twitter_Ivy_League_List.ipynb` notebook's API v2 functions will require a personal **Bearer Token** from a Twitter Developer account to be inserted into the code. This has not been included for security reasons.

---

## Contact Information
For any questions or concerns regarding this project, please contact:

*   **Name:** Shuxi Chen
*   **Email:** `shuxi.chen@mail.mcgill.ca`

*   **Name:** Hamza Javed
*   **Email:** `hamza.javed@mail.mcgill.ca`

*   **Name:** Junpeng Kou
*   **Email:** `junpeng.kou@mail.mcgill.ca`
content_copy
download
Use code with caution.
Markdown
