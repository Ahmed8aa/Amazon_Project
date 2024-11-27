## Contributors
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ahmed8aa"><img src="https://avatars.githubusercontent.com/u/111169742?v=4" width="100px;" alt="Ahmed Abdelrhman"/><br /><sub><b>Ahmed Abdelrhman</b></sub></a><br /><a href="#data-Ahmed8aa" title="Code">💻🔣🎨</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/OmarElmenofy"><img src="https://avatars.githubusercontent.com/u/144100276?v=4?s=100" width="100px;" alt="OmarElmenofy"/><br /><sub><b>OmarElmenofy</b></sub></a><br /><a href="#data-OmarElmenofy" title="Design">🔣🎨</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Boda1515"><img src="https://avatars.githubusercontent.com/u/132951877?v=4?s=100" width="100px;" alt="Abdelrahman"/><br /><sub><b>Abdelrahman Hany</b></sub></a><br /><a href="#design-Boda1515" title="Data">💻🔣📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Mbaligh"><img src="https://avatars.githubusercontent.com/u/186023899?v=4?s=100" width="100px;" alt="Mbaligh"/><br /><sub><b>Mohammed Baligh</b></sub></a><br /><a href="#doc-Mbaligh" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ragdan-ramadan-852752223"><img src="https://avatars.githubusercontent.com/u/111773709?v=4?s=100" width="100px;" alt="Raghdan Ramadan"/><br /><sub><b>Raghdan Ramadan</b></sub></a><br /><a href="#data-RAGHDANN" title="Data">🔣💻📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/youssef-khalf"><img src="https://avatars.githubusercontent.com/u/115180292?v=4?s=100" width="100px;" alt="youssef-khalaf"/><br /><sub><b>youssef-khalaf</b></sub></a><br /><a href="#design-youssef-khalf" title="Design">🔣🎨📖</a></td>
    </tr>
  </tbody>
</table>


<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
![dataengineeringproject6 drawio_5f9f4d55](https://github.com/user-attachments/assets/4d73eec5-a2ab-4cea-ab9a-f46c58fc449d)
# Azure Ascent: Pioneering Cross-Border E-Commerce Analytics (End-To-End Cloud Based Data Engineering Project)

## Overview
This project demonstrates a comprehensive data scraping, processing, and visualization pipeline leveraging Azure, GitHub, Power BI, and Tableau. The solution was designed to extract e-commerce data from Amazon's regional websites, transform it using scalable Azure services, and visualize insights using interactive dashboards.

### Key Features:
- **Scraping Code Development**: Built using Python, Docker, and VS Code.
- **Data Pipelines**: Enabled via Azure Synapse Analytics for transformation and Azure SQL for warehousing.
- **Visualization**: Interactive dashboards created in Power BI and Tableau.
- **Integration with GitHub**: Continuous integration and deployment managed with GitHub Actions.

---

## Technologies Used

- **Scraping Libraries**: BeautifulSoup, Selenium, aiohttp, Asycio.
- **Azure Services**:
  - Azure Durable Functions for orchestrating scraping tasks.
  - Azure Synapse Analytics for data transformation.
  - Azure Blob Storage for raw and processed data.
  - Azure SQL Data Warehouse for structured data storage.
- **GitHub**: Managing source code, CI/CD workflows, and secrets.
- **Visualization Tools**: Power BI and Tableau for dashboards.

---

## Architecture
### Workflow Summary
1. **Scraping Code Development**:
   - Python scripts perform scraping across Amazon’s regional websites (e.g., Egypt, India, Saudi Arabia, Japan).
   - Challenges such as CAPTCHAs and dynamic content are addressed using Selenium and EasyOCR.

2. **Data Pipeline Development**:
   - Data is uploaded using Azure Functions.
   - Azure Synapse Analytics processes raw data into structured datasets.
   - Transformed data is stored in an Azure SQL Data Warehouse for querying.

3. **Visualization Development**:
   - Dashboards in Power BI and Tableau provide insights into:
     - Regional price variations.
     - Best-selling products.
     - Seasonal trends in e-commerce.

---

## Detailed Components

### 1. Data Scraping
- **Regions Covered**: Amazon Egypt, India, Saudi Arabia, Japan.
- **Data Extracted**:
  - Product name, price, availability, ratings, product category.
- **Tools**:
  - BeautifulSoup for parsing HTML.
  - Scrapy for crawling and scraping.
  - Selenium for JavaScript-rendered pages.

### 2. Data Ingestion
- **Azure Durable Functions**:
  - Functions receive scraped data as JSON, preprocess and validate it, then upload it to Azure Blob Storage.
- **Pipeline 1**: Raw Data Ingestion
  - Azure Data Factory ingests raw data into the “Raw Folder” in Azure Blob Storage.

### 3. Data Transformation
- **Pipeline 2**:
  - Data is cleaned, normalized, and structured using Azure Synapse Analytics.
  - Normalization includes handling missing values, currency conversion, and unifying product categories.

### 4. Data Warehousing
- **Azure SQL**:
  - Star schema design with fact tables (e.g., Price data) and dimension tables (e.g., product details, regions).

### 5. Dashboards
- **Key Visualizations**:
  - Price trends across regions.
  - Most popular products by region.
  - Interactive maps showing regional comparisons.
- **Tools**:
  - Power BI for data modeling and dashboard creation.
  - Tableau for additional visuals.

---

## Key Insights
- Significant price variations for the same product across regions.
- Top-selling products differ significantly by market.
- Seasonal sales trends reveal price fluctuations during holidays.

---

## Future Enhancements
1. **Expand Coverage**:
   - Include Amazon websites from the US, UK, and other regions.
2. **Real-Time Updates**:
   - Automate scraping and data pipeline execution for live dashboards.
3. **Predictive Analytics**:
   - Integrate machine learning models to predict price trends and demand spikes.

---

## Challenges & Solutions
1. **CAPTCHAs**:
   - Managed using proxies and EasyOCR.
2. **Dynamic Content**:
   - Addressed using Selenium.
3. **Scalability**:
   - Leveraged Azure’s serverless architecture for automatic scaling.

---

## Team Credits
- Ahmed Abdelrahman
- Abdelrahman Hany
- Omar Elmnofy
- Mohammed Baligh
- Raghdan Ramadan
- Youssef Khalaf

### Supervisor: Eng. Khalid Seif





