# Keylogger Script 


This Python script is a **basic keylogger** that captures keyboard input and logs it into a file named `simple_key_log.txt`. Below is an explanation of how it works:

---

### **How It Works**
1. **Imports Necessary Modules**:  
   - `pynput.keyboard`: To listen to keyboard events.

2. **Log File**:  
   - Creates or appends to a file named `simple_key_log.txt` to store logged keys.

3. **Key Logging Function**:  
   - `log_key(key)`: Captures pressed keys and writes them to the file.
     - If the key is a regular character, it writes it directly.
     - For special keys like `space` or `enter`, it adds the corresponding actions (space or newline).
     - Other keys (e.g., `Ctrl`, `Shift`) are logged as `[KeyName]`.

4. **Stop Logging**:  
   - `stop_logging(key)`: Stops the listener when the `Escape` key is pressed.

5. **Start the Listener**:  
   - Creates a listener that runs until `Esc` is pressed.

---

### **Usage**
- Run the script using Python:
  ```bash
  python keylogger.py
  ```
- All keys pressed will be logged in `simple_key_log.txt`.

---

### **Important Notes**
1. **Ethical Considerations**:  
   This script is for **educational purposes only**. Unauthorized keylogging is illegal and unethical. Always obtain explicit permission before using it.

2. **Applications**:
   - Testing keyboard input in software.
   - Studying Python programming with external libraries.

3. **Dependencies**:  
   Install `pynput` if not already installed:
   ```bash
   pip install pynput
   ```

