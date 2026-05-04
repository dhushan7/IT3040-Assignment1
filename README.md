# IT3040 - Assignment 1: Chat Translator Test Automation

This repository contains an automated testing suite designed to validate the Singlish to Sinhala Chat Translator web application. The project utilizes Playwright for browser automation and Openpyxl for managing test data within Excel spreadsheets.

## 🚀 Project Overview
The goal of this project is to automate the validation of transliteration accuracy. It reads Singlish input strings from an Excel file, interacts with the web interface to perform the translation, and compares the actual output against the expected Sinhala results.


## 🛠 Tech Stack
Language: Python 3.10+

Automation: Playwright (Chromium)

Data Management: Openpyxl (Excel Integration)

Environment: Linux (Fedora/CentOS) / Windows


## 📂 Project Structure
test_automation.py: The core automation script that handles browser interaction and Excel I/O.

Assignment 1 - Test cases_2.xlsx: The test suite containing 50+ negative test cases, input types, and rationales.

requirements.txt: List of Python dependencies.


## ⚙️ Installation & Setup
Clone the Repository:

Bash
git clone https://github.com/dhushan7/IT3040-Assignment1.git

cd IT3040-Assignment1

Create a Virtual Environment (Optional but Recommended):

Bash
python -m venv venv

source venv/bin/activate  # Linux/macOS

### or
.\venv\Scripts\activate   # Windows

Install Dependencies:

Bash
pip install playwright openpyxl

Install Playwright Browsers:

Bash
playwright install chromium


## 🏃 How to Run the Tests

To execute the automated test suite using the provided test case file, run the following command:

Bash
python test_automation.py --excel "Assignment 1 - Test cases_2.xlsx" --sheet " Test cases"

Available CLI Arguments:
-- headless: Run the tests without opening a browser window.

-- url: Specify a different frontend URL if needed.

-- wait-ms: Adjust the wait time (default: 5000ms) for the translator to process input.

-- slow-mo-ms: Slow down the interaction to watch the automation in real-time.

## 📝 Test Case Methodology
The test suite in Assignment 1 - Test cases_2.xlsx is categorized into 24 distinct Singlish input types, including:

Question/Command Forms

Spelling Variants

English Digital Terms & Acronyms

Unit of Measurements & Currency

Each test case is designed with a specific Rationale to test the boundaries of the transliteration engine, focusing on phonetic accuracy and character mapping.




## Author: Minindu Madhushan

## Registration No: IT23617414

# Module: IT3040 - Assignment 1
