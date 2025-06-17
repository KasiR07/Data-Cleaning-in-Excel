# 🧹 Data Cleaning in Excel – Step-by-Step Guide

## 📄 1. Backup Your Data
**Always start by creating a copy of the sheet:**
- Right-click the sheet tab → Hold `Ctrl` → Drag to create a duplicate.

---

## 🧱 2. Auto-Fit Rows and Columns
- Click anywhere inside the data → Press `Ctrl + A` to select all.
- For rows: Press `Alt + H + O + A`  
- For columns: Press `Alt + H + O + I`

---

## 🔁 3. Remove Duplicates
- Click within the data → Press `Ctrl + A`  
- Go to the **Data** tab → Click **Remove Duplicates** → Select all → Confirm to remove them.

---

## ✂️ 4. Remove Text Inside Brackets
- Select the column → Press `Ctrl + H` (Find & Replace)
- In **Find what**: enter `(*)`  
- In **Replace with**: leave it blank  
- Click **Replace All**

---

## 🔠 5. Change Text Case (Lowercase/Uppercase)
1. Insert a new column beside your data (`Ctrl + Shift + +`)
2. Use the formula (example for cell C3):  
   - Lowercase: `=LOWER(C3)`
   - Uppercase: `=UPPER(C3)`
3. Copy the entire column → Right-click → **Paste Values**
4. Delete the original column (`Ctrl + -`)

---

## ✨ 6. Format Text (Proper Case & Trim Spaces)
- Formula: `=TRIM(PROPER(C3))`
- Autofill down → Copy → Paste Values → Delete the original column

---

## ➗ 7. Split Text into Multiple Columns
- Insert a blank column and give it a header
- Select the data (not header) → `Ctrl + Shift + ↓`
- Go to **Data** tab → Click **Text to Columns**
- Choose **Delimited** → Click **Next** → Choose separator (comma, space, etc.) → Set destination → **Finish**

---

## 📉 8. Replace Empty Cells with "NA"
- Select all data (`Ctrl + A`)
- Go to **Find & Select** → **Go to Special** → Choose **Blanks**
- Type `"NA"` in the formula bar → Press `Ctrl + Enter`

---

## ⚠️ 9. Convert Errors to "NA" Using IFERROR
- Formula:  
  ```excel
  =IFERROR(<original formula>, "NA")
