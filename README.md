# RPA Challenge - UiPath Automation

This UiPath automation fills out the [RPA Challenge form](https://rpachallenge.com/) using data from an Excel file. It intelligently handles changing field positions and updates input records with the processing status.

---

## 📁 Folder Structure

> ⚠️ Before running the bot, make sure this folder structure exists in your **Documents** directory:

C:\Users<YourUsername>\Documents\RPAChallengeBot
│
├── Processing
│ └── challenge.xlsx ← Place your input file here
│
└── Completed\ ← Processed file will be moved here

---

## 📥 Input File Format

- File name: `challenge.xlsx`
- Must be placed inside the `Processing` folder
- Required columns (headers must match the field names on the RPA Challenge form):


> During processing, a new column named **`RPA Status`** will be added to track success/failure for each row.

---

## 🚀 How to Use

1. Open the project in UiPath Studio
2. Place your `challenge.xlsx` file inside:
3. Run the automation
4. After processing:
- The Excel file will be updated with an **RPA Status** column
- It will be automatically moved to the **Completed** folder

---

## 🧰 Requirements

- UiPath Studio installed
- Excel installed (or Excel activities package)
- Internet access to reach the challenge website

---

## ✅ Features

- Handles dynamic form field positions
- Adds processing status to each row
- Moves completed files to Completed folder
