# Keylogger
Keylogger using Python

Overview
This project is a keylogger written in Python using the pynput library. It records keystrokes and saves them in a text file (`keylogger.txt`).

This project is for educational and ethical purposes only. Unauthorized use of keyloggers is illegal and unethical. Always obtain consent before running it on any system.


Features
- Logs all keystrokes typed by the user.
- Saves the recorded keys to a text file (`keylogger.txt`).
- Automatically writes keystrokes to the file after every 5 key presses.
- Stops logging when the `Esc` key is pressed.
- Captures timestamps for logging sessions.

Installation & Setup
Prerequisites
Ensure you have Python installed (3.x recommended). If not, download and install it from [Python's official website](https://www.python.org/downloads/).

Install Required Python Modules
Open the terminal (or command prompt) and install the `pynput` package:

```bash
pip install pynput
```

Clone or Download the Repository
Clone the repository using Git:

```bash
git clone https://github.com/surajjshinde/keylogger-python.git
cd keylogger-python
```

Or manually download and extract the files.

Run the Keylogger
Execute the Python script:

```bash
python key_logger.pyw  # Runs in the background (no console window)
# OR
python key_logger.py   # Runs with a console window (for debugging)
```

How It Works
1. Records Keystrokes: Captures all key presses.
2. Writes Logs in Batches: After every 5 key presses, it saves them to `keylogger.txt`.
3. Timestamps: Adds a timestamp at the beginning of the log session.
4. Stops on Esc Key: The keylogger stops recording when the `Esc` key is pressed.

---

Code Explanation

on_press(key)
- Appends the pressed key to a list.
- If 5 keys are collected, it writes them to the file and resets the list.

on_release(key)
Stops the keylogger when the `Esc` key is pressed.

write_file(keys)
Writes collected keys to `keylogger.txt`, replacing unwanted characters.









