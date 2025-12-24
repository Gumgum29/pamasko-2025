# 🎄 Pamasko Game 2025

A festive web-based "Lucky Gift" game built with HTML5, CSS3, and JavaScript. This project features a serverless backend integration using Google Apps Script to log winners directly into a Google Sheet database.

## 🚀 Deployment Instructions

### 1. Database Setup (Google Sheets)
1. Create a new Google Sheet.
2. In the first row, set the following headers: 
   `Name`, `Number`, `Prize`, `Device`, `Time`.
3. Go to **Extensions > Apps Script**.
4. Paste the `doPost` script provided in the project documentation.
5. Click **Deploy > New Deployment**.
   - **Type:** Web App
   - **Execute as:** Me
   - **Who has access:** Anyone
6. Copy the generated **Web App URL**.

### 2. Frontend Configuration
1. Open `gift.html` (or `index.html`).
2. Locate the `scriptURL` constant in the `<script>` section.
3. Replace the placeholder string with your copied **Web App URL**.
   ```javascript
   const scriptURL = 'YOUR_GOOGLE_SCRIPT_URL_HERE';