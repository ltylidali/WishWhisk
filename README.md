# WishWhisk 

**WishWhisk** is a lightweight, Jupyter-based Python tracker designed to monitor designer goods' prices. Built for quick, satisfying wins, V1 specifically targets the SSENSE catalog. 

It automatically scans for your specific keyword combinations, checks the stock status, and triggers a native Mac desktop notification the moment your dream item drops below your target price. No heavy databases, no stressful setup—just run it and let it hunt for deals while you sip your morning coffee. ☕️

## ✨ Features

* **🎯 Precision Targeting (Multi-Keyword Search):** Allows you to define specific combinations (e.g., `["lemaire", "croissant", "small", "black"]`) to ensure you are only tracking the exact style, size, and color you want.
* **💰 Custom Price Thresholds:** Set a hard maximum price limit (e.g., `1000` CAD). The tracker will only bother you if the current price falls at or below this number.
* **💔 In-Stock Verification (Anti-Heartbreak):** Automatically ignores "Sold Out" items, ensuring that every alert you receive is an actionable, purchasable deal.
* **🔔 Native Mac Notifications:** Bypasses the need for third-party messaging apps by leveraging macOS's built-in notification system (`osascript`). When a deal is found, a banner pops up instantly on your screen.

## 🛠 Prerequisites

To run TreatTracker V1, you will need:

* **OS:** macOS (Required for the native desktop notifications).
* **Environment:** VS Code with the Jupyter Notebook extension installed.
* **Python Libraries:** * `requests` (for fetching the webpage)
  * `beautifulsoup4` (for reading the webpage content)

*(You can install the required libraries by running `pip install requests beautifulsoup4` in your terminal or Jupyter cell.)*

## 🚀 How It Works (The V1 Workflow)

1. **Configure Your Radar:** Inside the Jupyter cell, you will add your desired items to a simple Python dictionary, listing your keywords and target price.
2. **Run the Cell:** Click "Run" in Jupyter whenever you want to check prices.
3. **Get Alerted:** The script silently browses SSENSE in the background. If nothing meets your criteria, it quietly prints a status update. If a match is found, your Mac will "ding" and display the deal!

## 🗺 Roadmap (Coming Later)
* Multi-Site Tracking (Farfetch, Mytheresa, etc.)
* Automated Currency Conversion 
* Mobile Push Notifications