# Email Integrated Keylogger

> **WARNING — Legal & Ethical:** This tool logs keystrokes and emails them. **Use only on devices you own or where you have explicit, written permission to monitor.** Unauthorized use is illegal and unethical. The author is not responsible for misuse.

---

## Overview

An educational/administrative tool that records keystrokes with timestamps and, on command (pressing `ESC`), emails the log and deletes the local file. **Designed for lawful use only** (device owner testing, lab research, or explicit monitoring consent).

## Features

* Logs every keystroke with a timestamp.
* Human-readable special key names: `[SPACE]`, `[ENTER]`, `[TAB]`, `[BACKSPACE]`, `[ESC]`, etc.
* Press `ESC` to: send the current log as an email, securely delete the local log file, and stop the program.
* No hardcoded passwords — supports secure credentials via environment variables or a `.gitignored` config file.

## Requirements

* Python 3.8+.
* Internet connection (to send email).
* SMTP-capable email account (Gmail with App Password recommended).

## Installation

```bash
# clone the repo
git clone https://github.com/yourusername/keylogger-project.git
cd keylogger-project

# create and activate a virtual environment (recommended)
python3 -m venv venv
source venv/bin/activate   # macOS / Linux
# venv\Scripts\activate   # Windows (PowerShell)

# install dependencies
pip install -r requirements.txt
```

## Usage

```bash
python3 keylogger.py
```

Compatibility

This project was tested with Python 3.11. pynput (used for key capture) is known to be incompatible with Python 3.12+ as of mid 2024–2025 and will crash with a _ThreadHandle TypeError.
If you see that error: run the project with Python 3.11 (create a venv), or use the keyboard fallback/branch.


