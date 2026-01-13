# 🚗 AckoDrive Master Scraper & Strategic Analyst: The "Unblockable" Edition

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Scraping](https://img.shields.io/badge/Skill-Web_Scraping-orange?style=for-the-badge)
![Analysis](https://img.shields.io/badge/Skill-Business_Intelligence-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Production_Ready-green?style=for-the-badge)

> **"First we reverse-engineered the API. Then we reverse-engineered the Market."** 🧠

---

## 📖 Overview
Welcome to the internal code audit of the **AckoDrive Car Project**. This repository is a dual-threat:
1.  **The Scraper**: An advanced DOM Simulator that extracts 6,000+ car variants without Selenium.
2.  **The Analyst**: A comprehensive **15-point Strategic Business Intelligence** report that decodes the Indian automotive market.

---

## Part 1: The "Secret Sauce" (Scraper Architecture) \ud83d\udd27

This isn't your average `soup.find()` script. We engineered a custom **DOM Simulator** to handle data complexity.

### 1. ⚡ API Reverse Engineering
Instead of clicking buttons, we discovered the hidden endpoint:
`GET /search/cars?city=Delhi&bodyTypes=Sedan`

### 2. 🏗️ The DOM Simulator
The API returns raw JSON. To make this data compatible with standard parsing logic (and easy to teach), we developed a **Simulation Engine** that:
1.  Takes the **JSON** payload.
2.  Wraps it in a **Simulated HTML Structure** on-the-fly.
3.  Injects **Hidden Data** (clean integers for prices) directly into the DOM.

---

## Part 2: The Strategic Brain (Business Analysis) \ud83d\udcca

We didn't just collect data; we interrogated it. The `Analysis On ACKO Web site.ipynb` notebook provides a **360-degree Market Scan**:

### \ud83c\udf1f 1. Market Overview
*   **Inventory Share**: Analyzing "ACKO Platform Inventory Share" to see which brands dominate the listings (Platform Availability vs Market Share).
*   **Regional Heatmaps**: Availability density across Maharashtra, Delhi, Karnataka, and more.

### \ud83d\udcb8 2. Consumer Insights
*   **The Value Matrix**: A quadrant analysis identifying **"High Value Gems"** (Low Price, High Rating) vs Overpriced assets.
*   **Cost Structure**: "Dumbbell Plots" revealing the massive price gap between Base and Top variants.
*   **Reliability Index**: Identifying brands with the highest customer satisfaction ratings.

### \ud83d\ude80 3. Strategic Deep Dive
*   **ACKO Portfolio Segmentation**: A reality check on "Premium Bias" - differentiating between the online urban user base and the national budget market.
*   **The SUV Battleground**: Who is winning the most competitive segment in India?
*   **Green Adoption**: Which states are leading the charge in EV and Hybrid penetration?

---

## 🛠️ File Structure
*   `AckoDrive_Scraper_Finalized.ipynb` \u2192 **The Engine** (Data Collection)
*   `Analysis On ACKO Web site.ipynb` \u2192 **The Brain** (Data Science & Strategy)

---

## 🚀 How to Run
1.  Clone this repository.
2.  Install dependencies:
    ```bash
    pip install requests beautifulsoup4 pandas matplotlib seaborn
    ```
3.  Open the notebooks:
    ```bash
    jupyter notebook
    ```
4.  Run the **Scraper** to get fresh data, then run the **Analysis** to generate insights! ✨

---

*This project is for educational and internal audit purposes.*
