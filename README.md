# Computer_Spyware

This Python project is a **computer monitoring tool** that demonstrates how to capture different types of user and system information. It combines multiple modules to record keystrokes, retrieve clipboard contents, extract Chrome browsing history, gather system details, and take screenshots.  

⚠️ **Disclaimer**: This project is for **educational purposes only**. Using it on someone else’s device without their consent is illegal and unethical.  

---

## Features  

### 1. Keystroke Logging (Keylogger)  
- Records all keys pressed by the user.  
- Saves keystrokes to a file named **`logs.txt`**.  
- Stops recording when the **Escape (Esc)** key is pressed.  

📂 Output: `logs.txt`  

---

### 2. System Information Retrieval  
- Collects details about the computer including:  
  - Date  
  - IP Address  
  - Processor information  
  - Operating System and Release version  
  - Hostname  
- Stores the collected data in an **Excel file**.  

📂 Output: `keystrokes.xlsx`  

---

### 3. Clipboard Data Retrieval  
- Captures the current text data in the **clipboard**.  
- Stores the clipboard content with a timestamp in **`clipboard.txt`**.  
- If no clipboard data is available, it logs an error message.  

📂 Output: `clipboard.txt`  

---

### 4. Google Chrome Browsing History Extraction  
- Retrieves URLs, titles, and timestamps of visited websites from Chrome’s **History database**.  
- Copies Chrome’s locked database into a temporary file (`History_copy`) so it works even if Chrome is open.  
- Extracts history into a **DataFrame** and saves it in Excel format.  

📂 Output: `search_history.xlsx`  

---

### 5. Screenshot Capture  
- Takes a screenshot of the current computer screen.  
- Saves the screenshot as a **PNG image**.  

📂 Output: `screenshot.png`  

---

## Requirements  

Install dependencies using **pip**:  

```bash
pip install pynput pandas pillow requests pywin32 openpyxl
