# McGill Football Analytics Project - Final Handoff

**Project Developed for: BUSA 649 - Analytics-Based Community Project**  
**Client: McGill University Football Team**  
**Authors: Shuxi Chen, Hamza Javed, Junpeng Kou**  
**Date: July 20, 2025**

---

## 1. Description

This repository contains the final deliverables for our community project with the McGill Football team. The project was executed in two distinct streams to support the analytical needs of Coaches Maxime Chaput Dupuy and Christopher Clement.

#### Stream A: In-Game Analytics Automation (for Maxime)
This stream focused on improving the efficiency and strategic value of in-game analysis. We designed and delivered a suite of **10 automated reports** based on game data from the team's DVSport platform. Eight of these reports are designed to be automated directly within DVSport, while two more complex reports are delivered via a supporting Excel template.

#### Stream B: Social Media Analysis (for Chris)
This stream focused on analyzing the team's external social media landscape. A working data pipeline was created to collect Twitter data related to Ivy League football programs, providing a new dataset for community engagement and recruitment analysis.

---

## 2. Handoff File Structure & Key Deliverables

This project is organized into two main folders, one for each project stream.

### For Maxime - DVSport Report Support

This folder contains all assets related to the DVSport reporting workflow.

*   **DVSport 10 Reports Prototype.ipynb**
    *   This Jupyter Notebook contains the complete Python code and logic used to reverse-engineer, validate, and prototype all 10 strategic reports. It serves as the technical documentation for how every calculation was derived.

*   **DVSport Reports 9 & 10.xlsx**
    *   This is the client-facing Excel Workbook. It is a ready-to-use template for the two most complex reports (QB Performance and OL/RB Yardage Attribution) that could not be fully implemented in DVSport.

*   **DVSport Data Dictionary.xlsx**
    *   A comprehensive guide defining all abbreviated column names from the raw DVSport data. This is a sustainable asset for any future analytics projects.

### For Chris - Twitter Data Scraping

This folder contains the assets for the social media analysis stream.

*   **Twitter_Ivy_League_List.ipynb**
    *   This Jupyter Notebook contains the fully functional Python data pipeline. It includes the code to query the Twitter (X) API, scrape relevant data, and structure it into a clean, usable format.

### Project-Wide Documentation

*   **Project Report.pdf**
    *   The comprehensive final report detailing the project's background, methodology, findings, and recommendations for both streams.

*   **ReadMe - McGill Football** (This Document)
    *   The central guide for navigating the project deliverables, explaining installation, and usage.

---

## 3. Installation & Setup

### For Maxime’s Deliverables:
*   **DVSport Reports 9 & 10.xlsx**: No installation is needed. Requires Microsoft Excel to open.
*   **DVSport 10 Reports Prototype.ipynb**: To run the code, you will need Python 3.7+ with standard data science libraries (pandas, numpy, etc.).

### For Chris’s Deliverable:
1.  **Open `Twitter_Ivy_League_List.ipynb`**: This notebook contains all the code and instructions.
2.  **Install Required Libraries**: The notebook will have a cell at the top to install the necessary libraries, such as `pandas` and `snscrape`.
3.  **Credentials**: To use the official Twitter API v2 functions, you will need to insert your own personal Bearer Token into the designated variable within the notebook.

---

## 4. Usage

### For Maxime’s Reports:
1.  **In-Platform Automation:** The 8 core reports are designed to be saved to the DVSport "Defaults List" for full, zero-maintenance automation on all new games.
2.  **Excel Reports (9 & 10):**
    *   Export the raw game dataset from DVSport.
    *   Open `DVSport Reports 9 & 10.xlsx` and paste the raw data into the **"Data-Input"** tab.
    *   The "Report 9" and "Report 10" tabs will update automatically.

### For Chris’s Twitter Analysis:
1.  Open the `Twitter_Ivy_League_List.ipynb` notebook.
2.  Adjust the configuration variables (e.g., keywords, accounts, date ranges) at the top of the notebook as needed.
3.  Run the cells sequentially to execute the data scraping and analysis.

---

## 5. Costs Involved

*   All solutions delivered were built using free and open-source tools or existing client software. There are **no immediate costs** to use these deliverables.
*   **Future Costs:** Robust, historical access to Twitter data via the official API v2 requires a paid subscription.

---

## 6. Contact Information

| Name | Role | Email |
| :--- | :--- | :--- |
| **Shuxi Chen** | McGill MMA '25 | `shuxi.chen@mail.mcgill.ca` |
| **Hamza Javed** | McGill MMA '25 | `hamza.javed@mail.mcgill.ca` |
| **Junpeng Kou** | McGill MMA '25 | `junpeng.kou@mail.mcgill.ca` |
