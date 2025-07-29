# RPA Challenge - UiPath Automation

This UiPath automation fills out the [RPA Challenge form](https://rpachallenge.com/) using data from an Excel file. It intelligently handles changing field positions and updates input records with the processing status.

---

## 📁 Folder Structure

> ⚠️ Before running the bot, make sure this folder structure exists in your **Documents** directory:

C:\Users<YourUsername>\Documents\Production FIles\RPAChallenge_REFramework

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

First Name | Last Name | Company Name | Role in Company | Address | Email | Phone Number | RPA Status

> ✅ **Important:**  
> Before running the bot, **you must manually add a column named `RPA Status` as the last column** in the Excel file.  
> This column will be updated by the bot to show whether each row was processed successfully or failed.

---

## 🚀 How to Use

1. Open the project in UiPath Studio
2. Place your `challenge.xlsx` file inside:
  Documents\RPAChallengeBot\Processing\
3. Run the automation
4. After processing:
- The `RPA Status` column will be updated
- The file will be automatically moved to the **Completed** folder

---

## 🧰 Requirements

- UiPath Studio installed
- Excel installed (or Excel activities package)
- Internet access to reach the challenge website

---

## ✅ Features

- Handles dynamic form field positions
- Uses the manually added `RPA Status` column to write row-wise result
