# Python for Drilling Engineers - Environment Setup Guide
![Animo Logo](https://raw.githubusercontent.com/johnryan417/python-for-drilling-engineers/main/assets/animo_signature_hallow.png)

## **1. Introduction**
Welcome to the **Python for Drilling Engineers** course! This guide will walk you through setting up your development environment so you can run Jupyter notebooks and work on Python-based drilling data analysis.

By following this guide, you'll be able to:
- Install VS Code
- Install Python and necessary libraries
- Set up a virtual environment
- Clone the course repository from GitHub
- Run Jupyter notebooks inside VSCode

### **1.1: Download & Install Visual Studio Code**
You can install any popular code editor, however, in this course we will use **VSCode** to write and run Python and Jupyter notebooks. To install VSCode:

- Go to the VSCode download page: https://code.visualstudio.com/download
- Select the version for your OS:
- Windows: Download .exe
- Mac: Download .dmg
- Linux: Download .deb or .rpm
- Run the installer and follow the setup instructions.
- Enable Extensions: During installation, check the box for "Add to PATH" (important for using it from the terminal).

---

## **2. Install Prerequisites**

### **2.1 Install Python**
Ensure you have Python **3.10.9** installed. 

**Check if Python is installed:**
```bash
python --version
```
or
```bash
python3 --version
```
If Python is not installed, download and install it from [python.org](https://www.python.org/downloads/).
- Scroll down to section titled **"Looking for a specific release?"**
- Find "Release version" Python 3.10.9 and click the **Download** link
- Scroll down to section titled Files and select *macOS 64-bit universal2 installer* or *Windows installer (64-bit)* depending on your OS

✅ **Windows Users:** During installation, check the box **"Add Python to PATH"** before clicking Install.

---

### **2.2 Install Git and GitHub Desktop (Optional)**
#### **Option 1: Install GitHub Desktop (For Beginners)**
1. Sign up for a free GitHub account, or sign in if you already have one at [github.com](https://github.com/).
2. Download **GitHub Desktop** from [desktop.github.com](https://desktop.github.com/).
3. Install and sign in to your GitHub account.
4. Use GitHub Desktop to **clone** the repository (see Step 3.2).


#### **Option 2: Install Git (Command Line Users)**
Download and install Git from [git-scm.com](https://git-scm.com/downloads).

---

## **3. Clone the Course Repository**

### **3.1 Open Command Prompt or Terminal**
#### **Windows:**
- Press `Win + S`, type **"Command Prompt"**, and press **Enter**.
- Or open **VSCode > Terminal > New Terminal**.

#### **Mac/Linux:**
- Open **Terminal** (`Cmd + Space`, type `Terminal`, press Enter).

### **3.2 Clone the Repository**
#### **Option 1: Using GitHub Desktop (For Beginners)**
1. Open **GitHub Desktop**.
2. Click **File > Clone Repository**.
3. Select **GitHub.com** and find `python-for-drilling-engineers`.
4. Click **Clone** and select a folder on your computer.
5. Once cloned, open it in **VSCode** by clicking **Repository > Open in Visual Studio Code**.

#### **Option 2: Using Command Line (For Command Line Users)**
```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/python-for-drilling-engineers.git
cd python-for-drilling-engineers
```



---

## **4. Set Up Your Python Environment**

### **4.1 Create a Virtual Environment**
A **virtual environment** ensures that all course dependencies remain isolated from your system Python installation.

Run the following commands:
```bash
cd python-for-drilling-engineers  # Navigate to the project folder
python -m venv venv  # Create a virtual environment
```

### **4.2 Activate the Virtual Environment**
#### **Windows:**
```bash
venv\Scripts\activate
```
#### **Mac/Linux:**
```bash
source venv/bin/activate
```
✅ You should now see `(venv)` at the beginning of your terminal line.

---

## **5. Install Required Libraries**
Install all required dependencies using:
```bash
pip install -r requirements.txt
```

This will install:
- pandas (Data manipulation)
- seaborn (Data visualization)
- matplotlib (Plotting)
- scikit-learn (Machine learning tools)
- numpy (Numerical computing)
- XlsxWriter (Excel file handling)
- jupyter (For running Jupyter notebooks)
- ipykernel (Required for Jupyter in VSCode)

✅ **Verify Installation:**
```bash
python -c "import pandas, seaborn, matplotlib, sklearn, numpy, XlsxWriter; print('All libraries installed successfully!')"
```
If you see **"All libraries installed successfully!"**, you're good to go!

---

## **6. Run Jupyter Notebook in VSCode**

### **6.1 Install VSCode Extensions**
1. Open **VSCode**.
2. Go to **Extensions** (`Ctrl + Shift + X`).
3. Search for **Python** and install it.
4. Search for **Jupyter** and install it.

### **6.2 Open Jupyter Notebook**
With your virtual environment activated, run:
```bash
jupyter notebook
```
This will open Jupyter Notebook in your web browser.

### **6.3 Create a New Notebook**
1. Click **New > Python 3 (ipykernel)**.
2. Start coding!

---

## **7. Updating Dependencies**
If updates are needed, run:
```bash
pip install --upgrade -r requirements.txt
```

---

## **8. Deactivating and Reactivating the Virtual Environment**

- **To deactivate:**
  ```bash
  deactivate
  ```
- **To reactivate later:**
  ```bash
  venv\Scripts\activate  # Windows
  ```
  ```bash
  source venv/bin/activate  # Mac/Linux
  ```

---

## **9. Troubleshooting**

### **Issue: Python Not Found**
- Ensure Python is installed and added to the system PATH.
- Restart your terminal and try again.

### **Issue: Virtual Environment Not Activating**
- Ensure you’re inside the correct project folder (`cd python-for-drilling-engineers`).
- Try using `python3 -m venv venv` if `python -m venv venv` fails.

### **Issue: Jupyter Not Found**
- Run `pip install jupyter` inside your virtual environment.
- Restart VSCode and reopen the terminal.

---

## **10. Next Steps**
Congratulations! 🎉 You now have a fully functional Python environment for the **Python for Drilling Engineers** course.

You’re now ready to:
✅ Work with Jupyter Notebooks.
✅ Analyze drilling data with Python.
✅ Push and pull code from GitHub.

🚀 **Let’s get started!** 🚀

