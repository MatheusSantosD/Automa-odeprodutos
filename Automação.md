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

```bash
1️⃣ Clone this repository:

git clone https://github.com/yourusername/your-repository-name.git

2️⃣ Install dependencies:

bash
Copiar
Editar
pip install pandas pyautogui

3️⃣ Edit produto.csv with your product data.

4️⃣ Adjust the click coordinates (pyautogui.click(x, y)) according to your screen and browser if needed.

5️⃣ Run the script:

bash
Copiar
Editar
python automacao_cadastro.py
The script will open your browser, log in, and start registering products automatically for you.

⚠️ Important Notes
Use this in a test environment first before running in production.

Avoid using your mouse and keyboard during execution, as pyautogui will be controlling your system.

Adjust pyautogui.PAUSE and time.sleep() according to your internet speed and machine performance.

🤝 Contributions
Contributions are super welcome to improve the code, optimize flows, or add new features.
Feel free to open an Issue or Pull Request if you would like to contribute!

📜 License
This project is licensed under the MIT License.

✉️ Contact
Questions or suggestions? Open an issue or reach out on LinkedIn so we can connect!

🚀 Happy learning and productive automations!
👊 #LetsGo

