# Fuzzy Vibration Control System 

## Project Overview
This project is a **Fuzzy Control System for Monitoring Vibration in Industrial Equipment**, such as motors, pumps, or compressors. The system uses **Fuzzy Logic** to evaluate the risk level of equipment based on three main factors:
- **Vibration (0 - 100 mm/s)**
- **Temperature (0 - 120 °C)**
- **Operation Time (0 - 500 hours)**

The system calculates a **Risk Level (0 - 10)**, providing an automatic assessment of equipment status.

---

## Features
- Real-time calculation of equipment risk using Fuzzy Logic.
- Multiple input variables (Vibration, Temperature, Operation Time).
- Intuitive interactive interface using Google Colab.
- Clear and clean automated testing section.
- Easy-to-understand risk evaluation system with visual graphs.

---

## Technologies Used
- **Python (3.x)**
- **scikit-fuzzy** - Fuzzy Logic Control System Library
- **Matplotlib** - For Visual Graphs
- **ipywidgets** - Interactive User Interface (in Google Colab)
- **Pandas** - For Clear Test Result Tables

---



##  Project Structure (Detailed by Sections)

### **Section 1: Install and Import Required Libraries**
- **Install Libraries:**
  - `scikit-fuzzy` (Fuzzy Logic Control System)
  - `matplotlib` (Graph Visualization)
  - `ipywidgets` (Interactive User Interface)
  - `pandas` (Test Result Display)
- **Import Libraries:**
  - `numpy` (Numerical Calculations)
  - `skfuzzy` (Fuzzy Logic Control)
  - `matplotlib.pyplot` (Graph Display)
  - `ipywidgets` (Interactive UI Components)
  - `IPython.display` (Output Control)

---

### **Section 2: Defining Fuzzy Variables**
- **Vibration Variable (0 - 100 mm/s):**
  - Membership: Low, Medium, High
- **Temperature Variable (0 - 120 °C):**
  - Membership: Low, Medium, High
- **Operation Time Variable (0 - 500 hours):**
  - Membership: Short, Moderate, Long
- **Risk Level Variable (0 - 10):**
  - Membership: Low, Moderate, High

---

### **Section 3: Defining Fuzzy Rules and Controller**
- **High Risk Rules:**
  - Conditions where high values of Vibration, Temperature, or Time result in High Risk.
- **Moderate Risk Rules:**
  - Conditions that represent balanced or medium risk situations.
- **Low Risk Rules:**
  - Conditions where values are within safe operating ranges.

---

### **Section 4: Risk Calculation and Visualization**
- **Risk Calculation Function:**
  - Accepts inputs: Vibration, Temperature, and Operation Time.
  - Computes the Risk Level using Fuzzy Logic.
  - Displays the calculated risk and active rules.
- **Risk Graph Display:**
  - Visualizes the Risk Level using `matplotlib`.

---

### **Section 5: Graph Display (Visual Representation)**
- Displays a clear graphical representation of the Risk Levels.
- Risk levels are color-coded:
  - Green for Low Risk
  - Orange for Moderate Risk
  - Red for High Risk

---

### **Section 6: Interactive User Interface**
- **Sliders:**
  - User-adjustable sliders for:
    - Vibration (0 - 100 mm/s)
    - Temperature (0 - 120 °C)
    - Operation Time (0 - 500 hours)
- **Run Button:**
  - Calculates the risk based on slider values.
  - Displays the result directly below the sliders.

---

### **Section 7: Automated Tests for Fuzzy System**
- **Test Case Definitions:**
  - Multiple predefined test cases (Low, Moderate, High Risk scenarios).
  - Each test has expected values for comparison.
- **Test Result Display:**
  - Shows the results of each test case (Pass/Fail).
  - Displays a summary of all test cases (Total, Passed, Failed).

---

### **README.md (Project Documentation)**
- Clear documentation for project setup and usage.
- Project structure and explanation of each section.
- Instructions for running the project and automated tests.


---

## ⚡ Setup and Installation
1. Make sure you have **Python 3.x** installed.
2. Install the required libraries:
   ```bash
   pip install -U scikit-fuzzy matplotlib ipywidgets pandas
