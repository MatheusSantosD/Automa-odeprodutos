# 🛠️ Automating Product Registration with Python

![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## 🚀 Overview

This repository demonstrates **how to automate product registration in web-based systems using Python and the `pyautogui` library**.

If you want to **stop wasting time on manual data entry and learn practical automation with Python**, this project is perfect for you!

---

## 🎯 What does this project do?

✅ Reads product data from a CSV file using pandas.  
✅ Automatically opens your browser and navigates to the system.  
✅ Logs in automatically.  
✅ Fills in product registration forms field by field.  
✅ Repeats the process for the entire product list with no manual effort.

---

## 🧩 Technologies Used

- **Python 3.x**
- `pyautogui` – for automating clicks and keystrokes.
- `pandas` – for reading and manipulating CSV data.
- `time` – for managing pauses during the process.

---

## 🗂️ Project Structure

- `produto.csv` – CSV file containing the list of products to register.
- Python Script:
  - **Step 1:** Automatically opens the system page.
  - **Step 2:** Logs into the system.
  - **Step 3:** Reads the product data.
  - **Step 4:** Fills in the forms with product data.
  - **Step 5:** Repeats until all products are registered.

---

## 🛠️ How to Use

1️⃣ **Clone this repository:**

```bash
git clone https://github.com/yourusername/your-repository-name.git

pip install pandas pyautogui
python automacao_cadastro.py
