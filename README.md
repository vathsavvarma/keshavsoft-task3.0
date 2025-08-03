## Overview

This project is a responsive dashboard built using **Bootstrap 5**, modern ES6 JavaScript, and ApexCharts for data visualization. It has been enhanced to dynamically display live statistics and charts by **binding frontend components to data from an external API**.

## 🔄 What Was Changed

- **Stat card values** (Profile Views, Followers, Following, Saved Post) are now **populated from `data.json`** at runtime, not hardcoded.
- **Chart data** (bar and donut charts via ApexCharts) are also **fetched from `API`**, allowing for easy updates and scalability.
- New or updated **code (`data-binding.js`)** handles fetching/parsing the data file and injecting values into the DOM and chart configs.
- The **HTML structure** (in `index.html`) was modified to assign unique `id` attributes to stat elements so JavaScript can target and update them.


## 📖 How It Works

1. On page load, `data-binding.js` uses `fetch()` to load `data.json`.
2. Stat cards and charts are updated automatically to reflect values from the latest data file.
3. Simply update `data.json` to refresh dashboard figures—no changes to HTML/JS required for new data.

## 🛠️ Key Skills/Demonstrated Concepts

- **Understanding and Modifying Existing Code:**
Retrofitted static dashboard to support dynamic, decoupled data binding.
- **Frontend-Backend Integration:**
Seamless update of UI (cards, charts) from a decoupled backend data source.
- **Bootstrap 5 Proficiency:**
Maintained a responsive and visually appealing layout using Bootstrap classes and grid.
- **JavaScript ES6:**
Utilized `fetch()`, template strings, and object destructuring for clean asynchronous code.
- **ApexCharts Integration:**
Updated charts dynamically using `updateOptions()` with data from the JSON file.
- **Responsiveness \& Clean UI:**
Maintained mobile-first design, supporting all modern browsers and device sizes.


## 🚀 Usage Instructions

1. **Clone the repository**
1. **Run with a local web server!** (Do not open with `file://`).
Example (in terminal):

```
cd filename
npm run dev
```

2. Access the dashboard at [http://localhost:5173//](http://localhost:5173//).
3. Edit `api` to update dashboard content live.

## 📁 Key Modified Files

- `index.html` — Added `id` attributes to stats for JS binding
- `data-binding.js` — Fetches/parses JSON, updates DOM and charts
- `data.json` — Holds all dashboard stats and chart data

**Summary:**
This project now demonstrates a clear separation between UI and data, modern code practices, and deep understanding of Bootstrap, JavaScript, and integration patterns.


<div style="text-align: center">⁂</div>

[^1]: index.html

[^2]: data.json

[^3]: data-binding.js

