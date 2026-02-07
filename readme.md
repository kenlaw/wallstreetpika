# Wall Street Pika Dashboard ⚡📈

A lightweight, single-file stock portfolio tracker and dashboard designed for quick asset monitoring, leverage calculation, and market overview.

> **Current Version:** v7.0.0

## 📋 Overview

Wall Street Pika is a browser-based dashboard built with pure HTML, CSS, and JavaScript. It connects to the Finnhub API to provide real-time stock quotes and calculates your total net equity, loan ratios, and portfolio distribution instantly.

It features a "Pika" themed UI with responsive design for both desktop and mobile use.

## ✨ Key Features

* **Real-Time Tracking:** Live stock prices via Finnhub API.
* **Portfolio Management:**
    * Input share counts and loan amounts.
    * Automatic calculation of **Net Equity** and **Leverage Ratio**.
    * **Smart Sorting (v7.0):** Default sorting by Asset Value (High to Low) to prioritize your biggest positions.
* **Privacy Mode:** One-click button (👁️) to mask all financial figures for safe viewing in public.
* **Snapshot System:** Save history records of your portfolio performance locally.
* **Backup & Restore:** Export your data to JSON/Base64 string to transfer between devices.
* **Responsive UI:**
    * **Card View:** Visual cards with price flashing effects.
    * **List View:** Compact rows for desktop power users.
* **Market Overview:** Quick glance at BTC, ETH, Oil, Gold, and major ETFs.

## 🚀 How to Run

Because this is a **single-file application**, no installation or build process (Node.js, NPM, etc.) is required.

1.  Clone this repository:
    ```bash
    git clone https://github.com/yourusername/wallstreetpika.git
    ```
2.  Open the `index.html` (or `v7.0.0.html`) file directly in any modern web browser.

### Hosting on GitHub Pages
1.  Go to your repository **Settings**.
2.  Navigate to **Pages**.
3.  Select the `main` branch as the source.
4.  Your dashboard will be live at `https://yourusername.github.io/wallstreetpika/`.

## ⚙️ Configuration & API Key

This dashboard uses [Finnhub.io](https://finnhub.io/) for stock data.

**Important Note on Security:**
The current code contains a hardcoded API token. If you plan to make this repository public, it is recommended to:
1.  Get your own free API key from Finnhub.
2.  Replace the `const API_KEY` variable in the script section.
3.  *(Optional)* For advanced security, consider asking the user to input their own key via the UI rather than hardcoding it in the file.

```javascript
// Inside the script tag
const API_KEY = 'YOUR_API_KEY_HERE';
```

## 🛠️ Tech Stack

* **Core:** HTML5, CSS3, Vanilla JavaScript (ES6+)
* **Data:** Finnhub API
* **Storage:** `localStorage` (for persistence)
* **Fonts:** Plus Jakarta Sans & Roboto Mono
* **Icons:** SVG & CSS-based graphics

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
```