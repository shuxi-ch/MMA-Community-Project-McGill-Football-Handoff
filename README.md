# MMA-Community-Project-McGill-Football-Handoff

## 1. Description

This project was developed in collaboration with the McGill Football team to support the coaching staff—specifically Maxime Chaput Dupuy and Christopher Clement—by building practical, automated solutions for their analytics workflows. The project was executed in two distinct streams:

#### Stream A: In-Game Analytics Automation (for Maxime)
This stream focused on improving the efficiency and strategic value of in-game analysis using the team's existing **DV Sport platform**. We designed and delivered a suite of **10 automated reports** based on game-tracked datasets. These reports help coaches extract key insights related to play tendencies, directional efficiency, and player performance, all formatted for easy reuse each week. Eight of these reports are automated directly within DVSport, while two more complex reports are delivered via a supporting Excel template.

#### Stream B: External Data Integration (for Chris)
This stream aimed to build a long-term infrastructure for integrating external data to support goals like scouting, recruiting, and performance benchmarking. A working data pipeline was created using `snscrape` to collect Twitter data, and a prototype pipeline was built for future integration with the official Twitter API v2.

---

## 2. Tech Assets & Key Deliverables

*   **DV Sport Report Templates (8):** In-platform report designs saved to the "Defaults List" for full automation.
*   **Excel Analytics Workbook (2 Reports):** A single Excel file containing pivot tables for Reports 9 & 10, which require advanced calculations.
*   **Data Dictionary (`Data_Dictionary.xlsx`):** A comprehensive guide defining all abbreviated column names from the raw DVSport data.
*   **Python Scripts (Stream B):**
    *   `snscrape_pipeline.py`: A fully functional script for scraping Twitter data.
    *   `twitter_api_v2_prototype.py`: A well-documented prototype for future integration with the official Twitter API.
*   **Configuration File (`config.py`):** An editable file for setting keywords, date ranges, and export paths for the Twitter scripts.
*   **Sample Dataset:** `Sample_DVSport_Export.xlsx` to demonstrate the expected raw data format.

---

## 3. Installation

### For Maxime’s DV Sport & Excel Reports:
No installation is needed.
- The 8 core reports are already implemented and automated within the DVSport "Defaults List".
- The supporting Excel Workbook requires only Microsoft Excel to open.

### For Chris’s Twitter Pipeline:
1.  **Clone the Repository:**
    ```bash
    git clone [URL_to_your_GitHub_repo]
    ```
2.  **Install Python:** Ensure you have Python 3.7+ installed on your system.
3.  **Install Required Libraries:** Navigate to the project folder in your terminal and run:
    ```bash
    pip install pandas snscrape
    ```
4.  **Configure:** Open the `snscrape_pipeline.py` script and update the configuration variables as needed.

---

## 4. Usage

### Maxime’s Reports (Automated Workflow)
**In-Platform Reports (Reports 1-8):**
1.  Create a new game/project in DVSport.
2.  The 8 reports will be **automatically generated** from the "Defaults List". No further action is required.

**Excel Reports (Reports 9 & 10):**
1.  Export the complete raw dataset for the desired game from DVSport.
2.  Open the `McGill_Football_Advanced_Reports.xlsx` file.
3.  Go to the "Data-Input" tab and paste the raw data.
4.  Navigate to the "Report 9" and "Report 10" tabs. The pivot tables and visuals will **update automatically**.

### Chris’s Twitter Pipeline:
1.  Adjust the configuration in `snscrape_pipeline.py` (e.g., keywords, accounts, date ranges).
2.  Run the script from your terminal:
    ```bash
    python snscrape_pipeline.py
    ```
3.  Review the exported `.csv` file in the `output/` folder. This structured data can be loaded into Excel, Tableau, or other analytics tools.

---

## 5. Features

### Maxime’s DV Sport Reports:
*   10 structured analytical reports (8 in-platform, 2 in Excel).
*   Dual "Global" and "Subgroup" views for comprehensive analysis.
*   Breakdowns by Personnel, Formation, Down & Distance, and Field Zone.
*   Directional tendency analysis (L/R, Field/Boundary).
*   Yardage attribution model for OL vs. RB (in Excel).
*   Designed for **non-technical reuse** by coaches.

### Chris’s External Integration Stream:
*   Configurable tweet scraping using `snscrape`.
*   Outputs structured CSVs ready for analysis.
*   Well-documented prototype for future Twitter API v2 integration.
*   Modular design ready for expansion to CFL and Genius Sports APIs.

---

## 6. Data Sources

*   **Internal Data:** Game-by-game Excel/CSV exports from the **DVSport platform**.
*   **External Data:** **Twitter (X)** via the `snscrape` library.

---

## 7. Troubleshooting

### Maxime’s Reports:
*   **Excel reports show old data:** In Excel, go to the `Data` tab and click `Refresh All`.
*   **Excel reports are broken:** Ensure the pasted data in the "Data-Input" tab matches the column structure of the sample file.

### Chris’s Scripts:
*   **Error: `ModuleNotFoundError`:** Ensure you have installed the required libraries by running `pip install pandas snscrape`.
*   **No output generated:** Check that the date formats in the configuration are correct and that the script has permission to write to the `output/` folder.

---

## 8. Costs Involved

*   All solutions delivered were built using free and open-source tools (Python, `snscrape`) or existing client software (DVSport, Excel). There are **no immediate costs** to use these deliverables.
*   **Future Costs:** Full, robust access to historical Twitter data via the official API v2 requires a paid subscription (e.g., Academic or Enterprise tiers). Future integrations with platforms like Genius Sports may also require credentials or licensing fees.

---

## 9. Passwords and Credentials

*   No credentials are required for the current implementation of the DVSport reports or the `snscrape` script.
*   The `twitter_api_v2_prototype.py` will require a personal Bearer Token from a Twitter Developer account to function. This has not been included for security reasons.

---

## 10. Contact Information

| Name | Role | Email |
| :--- | :--- | :--- |
| **Shuxi Chen** | McGill MMA '25 | `shuxi.chen@mail.mcgill.ca` |
| **Hamza Javed** | McGill MMA '25 | `hamza.javed@mail.mcgill.ca` |
| **Junpeng Kou** | McGill MMA '25 | `junpeng.kou@mail.mcgill.ca` |
content_copy
download
Use code with caution.
Markdown
