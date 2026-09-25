# Oxylabs E-commerce Product Data Scraping and Analysis

## Overview

This project demonstrates an end-to-end web scraping and data analysis workflow for collecting e-commerce product information from the Oxylabs sandbox website.

The project uses Python to:

- Access the Oxylabs sandbox product listing pages.
- Parse HTML content using BeautifulSoup.
- Identify product cards and extract product information.
- Scrape product data across 94 listing pages.
- Clean and transform product prices into numeric Euro values.
- Remove duplicate and incomplete records.
- Export the processed dataset to CSV.
- Perform exploratory analysis through visualizations.

The complete implementation is available in the accompanying Jupyter Notebook:

`Oxylabs_E_commerce_Product_Data_Scraping_and_Analysis_.ipynb`

---

## Project Pipeline

```mermaid
flowchart LR
    A[Oxylabs Sandbox Website] --> B[HTTP Requests]
    B --> C[HTML Response]
    C --> D[BeautifulSoup Parsing]
    D --> E[Identify Product Cards]
    E --> F[Extract Product Fields]
    F --> G[Collect Data from 94 Pages]
    G --> H[Raw Product DataFrame]
    H --> I[Data Cleaning]
    I --> J[Price Transformation]
    J --> K[Duplicate & Missing Value Removal]
    K --> L[Clean Product Dataset]
    L --> M[CSV Export]
    L --> N[Exploratory Data Analysis]
    N --> O[Price Distribution]
    N --> P[Products per Page]
    N --> Q[Top 10 Most Expensive Products]
