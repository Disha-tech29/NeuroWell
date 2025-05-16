# NeuroWell 

**NeuroWell** is a lightweight mental wellness assistant designed to help you track your mood, energy, and focus levels, and analyze your emotional rhythms over time.

---

## 🌟 Features
- 🧠 Mood logger with time-based log analysis
- ⏱️ Inactivity detection using idle tracking
- 💬 Friendly self-care messages
- 📊 Weekly mood and rhythm reports
- 🧹 Log cleaner utility
- 📁 Modular C source code (in `src/`) with Makefile for compilation

---

## How to Use

### 1. **Log Your Mood**

Run this in PowerShell:
.\mood_logger.exe

it asks for:
Mood (1–5)
Energy (1–5)
Focus (1–5)

the result is saved in mood_log.txt

### 2. **Analyze Mood Patterns**
Run:
.\rhythm_analyzer.exe

It analyzes the log and creates a report in:
log/report.txt

💡 **To view the report:**
- Open `log/report.txt` using Notepad or any text editor  
- Or, run this command in PowerShell:
  notepad log\report.txt

### 3. **Clean Old Logs**
Run:
.\clean_log.exe
This will clear your existing mood logs and start fresh.

### 4. **Automated Hourly Prompt**
A PowerShell script will auto-run mood_logger.exe hourly.
Script: script/hourly_prompt.ps1
Scheduled via: Windows Task Scheduler
If you want to run manually:

.\script\hourly_prompt.ps1

---
## Example Run:
Here’s what it looks like when you log your mood and analyze the report:
![Screenshot 2025-05-17 004422](https://github.com/user-attachments/assets/89517b69-f372-4978-bd8b-1bad5607f3f0)

---

Project Structure:

NeuroWell/
├── mood_logger.exe         # Log your mood manually
├── rhythm_analyzer.exe     # Analyze mood log
├── clean_log.exe           # Clear mood logs
├── script/
│   └── hourly_prompt.ps1   # Script for hourly mood prompt
├── log/
│   └── report.txt          # Mood report output
├── mood_log.txt            # Mood log file
├── README.md               # Project guide

---

Why Choose NeuroWell?...
Your mental well-being matters. NeuroWell offers a tech-assisted way to check in with yourself privately and reflect on your inner state.

---

Future Plans:

Export data to CSV or Excel.
Add graphs and visualizations.
Text-to-speech prompts.
GUI with buttons and dark mode.

---

Built With:

C (Compiled with GCC via MinGW)
PowerShell
Windows Task Scheduler

---

Created with ❤️ by Disha Paralkar

