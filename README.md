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

## Part 2: The Strategic Brain (Business Analysis) 📊

We didn't just collect data; we interrogated it. The `Analysis On ACKO Web site.ipynb` notebook provides a **360-degree Market Scan**:

### 🌟 1. Market Overview
We analyze the **"ACKO Platform Inventory Share"** to see which brands dominate the listings. This acts as a proxy for platform availability versus national market share. We also map availability density across key states like **Maharashtra** and **Delhi**.

### 💸 2. Consumer Insights
Our **Value Matrix** quadrant analysis identifies **"High Value Gems"** (Low Price, High Rating) versus overpriced assets. We also use **"Dumbbell Plots"** to reveal the massive price gap between Base and Top variants, along with a **Reliability Index** to spotlight customer satisfaction leaders.

### 🚀 3. Strategic Deep Dive
A reality check on **"Premium Bias"**—differentiating between the online urban user base and the national budget market. We also identify the winner of the **SUV Battleground** and track **Green Adoption** (EV/Hybrid penetration) across states.

---

## 🛠️ File Structure
*   `AckoDrive_Scraper_Finalized.ipynb` → **The Engine** (Data Collection)
*   `Analysis On ACKO Web site.ipynb` → **The Brain** (Data Science & Strategy)

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
