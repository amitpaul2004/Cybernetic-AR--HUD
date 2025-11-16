# 🚀 Cybernetic AR HUD (with Hand Gesture Control)
A fully interactive **Augmented Reality HUD** running directly in your browser. Includes:
- Live camera feed
- Cybernetic HUD overlay
- Radar tracking system
- Target lock system
- Hand gesture control using **MediaPipe Hands**

This README explains **how to run, use, and customize** the project. A sample UI preview image placeholder is also included.

---

# 📸 UI Preview 
<img width="1919" height="854" alt="image" src="https://github.com/user-attachments/assets/522dd20a-4d2a-4cb8-aa19-30775e377682" />


```

---

# 🛠️ Features
### ✔️ AR camera background
Uses your device webcam to render a real-time AR view.

### ✔️ Cybernetic HUD Components
- Central crosshair
- Animated radar with sweep
- Target boxes with lock-on animation
- System info panel (battery + CPU + time)
- Scanlines + glitch noise

### ✔️ Hand Gesture Controls (MediaPipe)
| Gesture | Action |
|---------|--------|
| 🤚 Open Palm | Spawn target |
| 🤏 Pinch (thumb + index) | Lock target under crosshair |
| ✊ Fist | Toggle camera |
| ↔️ Fast horizontal swipe | Clear all targets |

---

# 🐍 Running the Project (Python Method)
The easiest way to run this AR HUD.

## 1️⃣ Install Python
Make sure Python 3.8+ is installed.
```
python --version
```

## 2️⃣ Place `index.html` inside a folder
Example:
```
AR-HUD/
   index.html
```

## 3️⃣ Run a local server
Open VS Code terminal inside the project folder:
```
python -m http.server 5500
```

## 4️⃣ Open in browser
Visit:
```
http://127.0.0.1:5500/index.html
```
⚠️ **Important:** Camera access works only on localhost or HTTPS.

## 5️⃣ Allow camera permissions
Your browser will ask for webcam access.

✔️ Done — The HUD will start immediately.

---

# ▶️ Alternative Method: VS Code Live Server
1. Install the **Live Server** extension (Ritwick Dey).
2. Right-click `index.html` → **Open With Live Server**.
3. The project opens at:
```
http://127.0.0.1:5500/
```
4. Allow camera access.

---

# 🎮 Usage Guide
### Keyboard Controls
| Key | Action |
|-----|--------|
| **C** | Toggle camera |
| **W** | Spawn target |

### Mouse Controls
- Click a target → Lock
- Drag a target → Move it

### Hand Gestures (MediaPipe Hands)
| Gesture | Action |
|---------|--------|
| 🤚 Open palm | Spawn target |
| 🤏 Pinch | Lock target |
| ✊ Fist | Toggle camera |
| ↔️ Swipe | Clear all targets |

---

# 📦 Project Structure
```
AR-HUD/
 ├── index.html        # Full HUD + gesture script
 ├── assets/
 │    └── ui-preview.jpg (optional screenshot)
 └── README.md         # This file
```

---

# 🔧 Dependencies (CDN Included)
No installation required.
The project uses CDNs for:
- MediaPipe Hands
- Camera Utils

Everything runs in the browser.

---

# 📱 Device Requirements
- Laptop or phone with camera
- Chrome / Edge recommended
- Good lighting for gesture detection

---

# 🧩 Customization
You can modify:
- HUD style → inside `<style>` of `index.html`
- Gesture actions → inside the gesture `<script>` block
- Target behavior → functions like `spawnTarget()` & `lockTarget()`

Need separated CSS + JS files? I can generate them.

---

# 🐛 Troubleshooting
### ❌ Camera not working?
- Ensure URL begins with **http://127.0.0.1** or **http://localhost**
- Do NOT use `file://` — browser blocks camera
- Check browser permissions

### ❌ Gestures not detected?
- Improve lighting
- Hold your hand in front of the camera clearly
- Chrome works best

---

# ⭐ Credits
Developed with:
- HTML + CSS + JavaScript
- MediaPipe Hands for gesture tracking
- Python HTTP server for hosting

---

If you want, I can also generate:
✔️ A full GitHub repository layout
✔️ A `LICENSE` file
✔️ A `setup.sh` auto-run script
✔️ A Flask backend version
✔️ Attach your UI screenshot to the README automatically (upload your image)\n
