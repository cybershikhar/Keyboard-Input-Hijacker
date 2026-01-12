# Keyboard Input Hijacker (VBScript)

## Overview
This project contains a **VBScript** that repeatedly sends simulated keyboard input to the currently active window on a Windows system.  

Despite the name, this script does **not** hijack physical keyboard input or monitor keystrokes. It simply automates typing using the Windows Script Host.

---

## File Included

### `Keyboard_Input_Hijacker.vbs`

**Description:**
- Creates a `WScript.Shell` object
- Uses `SendKeys` to inject keystrokes
- Runs in an infinite loop
- Pauses briefly between each input action

---

## How the Script Works
1. Initializes a Windows Shell object
2. Enters an infinite `Do ... Loop`
3. Sends a predefined text string as keyboard input
4. Sleeps for 500 milliseconds
5. Repeats until manually terminated

---

## Behavior
- Continuously types text wherever the cursor is active
- Can disrupt normal keyboard usage
- Runs indefinitely unless stopped

⚠️ **Warning:** Running this script can make your system difficult to use until the process is terminated.

---

## What This Script Does NOT Do
- ❌ Does not log keystrokes
- ❌ Does not capture passwords
- ❌ Does not hook keyboard drivers
- ❌ Does not access files or the network
- ❌ Does not establish persistence

This is **not a keylogger or real keyboard hijacking malware**.

---

## How to Stop the Script
If the script is running:

1. Press **Ctrl + Alt + Delete**
2. Open **Task Manager**
3. End the process:
   - `wscript.exe` or `cscript.exe`

If needed, reboot the system.

---

## Use Cases
- VBScript automation demonstrations
- Security awareness examples
- Educational analysis of script-based misuse
- Simple prank scripts (not recommended in professional environments)

---

## Security & Ethics Notice
Running scripts that interfere with user input **without consent** can be considered abusive or malicious.

Use this script:
- Only on systems you own
- Only with explicit permission
- For educational or testing purposes

---

## Disclaimer
This project is provided **for educational purposes only**.  
The author assumes no responsibility for misuse or damage caused by executing this script.

---

## Notes
The hardcoded injected message suggests the script was created as a prank or test rather than a serious attack tool.
