# 🚗 AckoDrive Master Scraper: The "Unblockable" Edition

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Scraping](https://img.shields.io/badge/Skill-Web_Scraping-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Production_Ready-green?style=for-the-badge)
![Education](https://img.shields.io/badge/Mode-Educational_Deep_Dive-purple?style=for-the-badge)

> **"Why scrape the frontend when you can talk to the backend?"** 🧠

---

## 📖 Overview
Welcome to the internal code audit of the **AckoDrive Car Scraper**. This project demonstrates an advanced, robust approach to extracting data from modern Single Page Applications (SPAs) **without** using slow, brittle browser automation tools like Selenium.

We successfully reverse-engineered the private API used by AckoDrive to extract over **6,000+ car variants** across 30+ cities with precision speed.

---

## 💡 The "Secret Sauce" (Architecture)

This isn't your average `soup.find()` script. We engineered a custom **DOM Simulator** to handle data complexity.

### 1. ⚡ API Reverse Engineering
Instead of clicking buttons, we discovered the hidden endpoint:
`GET /search/cars?city=Delhi&bodyTypes=Sedan`

### 2. 🏗️ The DOM Simulator
The API returns raw JSON. To make this data compatible with standard parsing logic (and easy to teach), we developed a **Simulation Engine** that:
1.  Takes the **JSON** payload.
2.  Wraps it in a **Simulated HTML Structure** on-the-fly.
3.  Injects **Hidden Data** (clean integers for prices) directly into the DOM.
4.  Feeds it to `BeautifulSoup` as if it were a real website.

### 3. 🛡️ The "Catch-All" Strategy
AckoDrive limits results to 50 cars per list. We bypass this by:
*   **Iterating Body Types**: `Sedan`, `SUV`, `Hatchback`...
*   **The Checkmate Move**: A final `Other` query that runs without filters to catch any car (like a rare Coupe) that slipped through the main categories.

---

## 🎓 Educational Features
This repository is designed for **Learning**. The Source Code (`AckoDrive_Scraper_Finalized.ipynb`) is heavily commented with:
*   **# THEORY**: Why we chose a specific library.
*   **# STRATEGY**: High-level architectural decisions.
*   **# LOGIC**: Detailed breakdowns of complex if/else chains.
*   **# VISUAL CODING**: HTML construction separated from Python logic for readability.

---

## 🛠️ Tech Stack
*   **Python 3**: The engine.
*   **Requests**: For mimicking browser network calls.
*   **BeautifulSoup4**: For parsing our simulated DOM.
*   **Pandas**: For structuring data into clean CSV reports.
*   **Tqdm**: For real-time progress tracking.

---

## 🚀 How to Run
1.  Clone this repository.
2.  Install dependencies:
    ```bash
    pip install requests beautifulsoup4 pandas tqdm
    ```
3.  Open the notebook:
    ```bash
    jupyter notebook AckoDrive_Scraper_Finalized.ipynb
    ```
4.  Run all cells and watch the magic happen! ✨

---

*This project is for educational and internal audit purposes.*
