# 🖐️ GestureDraw — Finger Painting Studio

> Paint in mid-air using just your hand. No stylus, no touch, no installs — just your webcam and your fingers.

![GestureDraw Banner](https://ibb.co/6Jv47hWF)

## ✨ What is this?

GestureDraw is a browser-based creative painting tool powered by **AI hand tracking**. It uses your webcam and Google's MediaPipe library to detect your hand in real time — then turns your finger movements into brush strokes on a neon canvas.

Just open the HTML file in your browser, allow camera access, and start painting.

---

## 🎮 How to Use

| Gesture | Action |
|--------|--------|
| ☝️ Point one finger | Draw / paint |
| 🤚 Open palm | Erase |
| ✌️ Peace sign | Pause drawing |

**Mouse & touch also work** — you can draw normally with your mouse or finger on a touchscreen too.

---

## 🛠️ Features

- **AI Hand Tracking** — real-time finger detection using MediaPipe Hands
- **5 Drawing Tools** — Pencil, Brush, Highlighter, Eraser, Fill
- **12 Neon Colors** — full color palette on the right panel
- **Adjustable brush size & opacity**
- **Undo / Redo** — full history stack
- **Screenshot** — save your artwork as a PNG
- **Screen Recording** — record your drawing session as a `.webm` video
- **Animated particle background**
- **Keyboard shortcuts** — `P` Pencil · `B` Brush · `H` Highlighter · `F` Fill · `E` Eraser · `Ctrl+Z` Undo · `Ctrl+Shift+Z` Redo · `Delete` Clear

---

## 🚀 Getting Started

No build tools, no npm, no setup needed.

1. **Clone or download** this repo
   ```bash
   git clone https://github.com/mohit8gh/gesture-draw.git
   ```

2. **Open** `gesture-draw.html` in your browser (Chrome or Edge recommended)

3. **Allow camera access** when prompted

4. **Raise your hand** and start painting!

> ⚠️ Must be opened over `http://` or `https://` for camera access to work. Opening directly as a local file (`file://`) may block the webcam in some browsers. Use a simple local server like VS Code Live Server, or just host it online.

---

## 🌐 Live Demo

👉 **[Try it live here](https://livecamdraw.infinityfreeapp.com/)**

---

## 🧰 Tech Stack

| Tech | Purpose |
|------|---------|
| Vanilla HTML / CSS / JS | No frameworks, zero dependencies |
| [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands) | Real-time hand landmark detection |
| Canvas API | Drawing engine |
| MediaRecorder API | Screen recording |
| Google Fonts (Orbitron, Inter) | UI typography |

---

## 📁 File Structure

```
gesture-draw/
└── gesture-draw.html    # Everything — single self-contained file
└── README.md
```

---

## 🖼️ Screenshots

<!-- Add your screenshots here -->
| Start Screen | Drawing Mode |
|---|---|
| ![drawing](https://ibb.co/6Jv47hWF) |

---

## 🔧 Customization

Everything is in one file — just open `gesture-draw.html` in any editor.

- **Add colors:** find the `COLORS` array around line 674 and add hex codes
- **Change default tool:** update `tool: 'pencil'` in the `state` object
- **Adjust hand tracking sensitivity:** find `minDetectionConfidence` and `minTrackingConfidence` and change the values (0–1)
- **Change background:** find `#000010` in the `animateBg` function

---

## 📋 Browser Support

| Browser | Status |
|---------|--------|
| Chrome 90+ | ✅ Full support |
| Edge 90+ | ✅ Full support |
| Firefox | ⚠️ Partial (recording may vary) |
| Safari | ⚠️ Limited (MediaPipe may have issues) |
| Mobile Chrome | ✅ Works (touch drawing supported) |

---

## 📄 License

MIT — free to use, modify, and share.

---

## 🙌 Credits

- Hand tracking powered by [MediaPipe](https://google.github.io/mediapipe/) by Google
- Built with ❤️ using plain HTML, CSS, and JavaScript

---

*Made by [Mohit Milan](https://github.com/mohit8gh)*
