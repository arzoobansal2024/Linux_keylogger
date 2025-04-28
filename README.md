# Linux Keylogger

This project captures raw keyboard input events from the Linux `/dev/input/` system and emits readable `keydown`, `keyup`, and `keypress` events using Node.js.  
It demonstrates direct device reading, buffer parsing, and event-driven architecture.

---

## 🚀 Features
- Real-time key event monitoring
- Low-level binary parsing of Linux input events
- Event-driven handling of keyboard events
- Simple and lightweight Node.js implementation

---

## 🛠 Technologies
- Node.js
- Core Node modules: `fs`, `events`
- Linux input subsystem (`/dev/input/eventX`)

---

## ⚙️ System Requirements
- Linux OS (Kali, Ubuntu, Debian, etc.)
- Node.js v14 or higher
- Root permissions (to read from `/dev/input`)

---

## 📂 Project Structure
| File | Purpose |
|:---|:---|
| `index.js` | Main logic for reading and parsing keyboard events. |
| `keycodes.js` | (Optional) Mapping file for keycodes to readable names. |

---

## 🔥 How to Run

1. Navigate to the project directory:
   cd ~/Downloads/keylogger

2. Install Node.js if not installed:
    sudo apt update
    sudo apt install nodejs npm

3. Identify your keyboard device:
    sudo apt install evtest
    sudo evtest
  Note the correct /dev/input/eventX.

4. Update the device in your code if needed.

5. Run the script:
    sudo node index.js

6. Press keys and observe the console output!
