# SignBridge — ASL Real-Time Translator

> Real-time American Sign Language (ASL) recognition using MediaPipe + Web Speech API.  
> No installation needed. Works directly in the browser — mobile & desktop.

## Live Demo
🔗 **[your-username.github.io/signbridge](https://your-username.github.io/signbridge)**

---

## Features
- Real-time hand landmark detection via **MediaPipe HandLandmarker**
- ASL alphabet recognition (A–Y, 24 supported letters)
- Letter → Word → Sentence builder
- **Text-to-Speech** output (Web Speech API, no API key needed)
- Works on phone camera — tested on Snapdragon 8 Gen 3
- Fully offline after first load (model cached by browser)

## How to Use
1. Open the link in Chrome (mobile or desktop)
2. Allow camera access
3. Show your hand and hold an ASL letter for ~0.6 seconds
4. The letter gets added to the current word automatically
5. Press **Add Space** to finish a word
6. Press **Speak Sentence** to hear the full sentence aloud

## Tech Stack
| Tech | Purpose |
|------|---------|
| [MediaPipe Tasks Vision](https://developers.google.com/mediapipe) | Hand landmark detection |
| TensorFlow Lite (embedded in MediaPipe) | GPU-accelerated inference |
| Web Speech API | Text-to-speech output |
| Vanilla JS (ES Modules) | Zero dependencies |
| GitHub Pages | Free hosting |

## Supported ASL Letters
A B C D E F G H I K L M N O P Q R S T U V W X Y

*(J and Z require motion — coming soon)*

## Deploy in 2 minutes
```bash
git clone https://github.com/YOUR_USERNAME/signbridge
cd signbridge
# Push to GitHub → Settings → Pages → Deploy from main branch
```

## Project Structure
```
signbridge/
└── index.html    ← entire app in one file
└── README.md
```

## Academic Context
Built as a Computer Vision + AI project demonstrating:
- Real-time pose estimation (MediaPipe)
- Geometric gesture classification
- Browser-native ML inference (WebAssembly + WebGL)
- Accessible communication technology

---
Made with 💙 | Powered by Google MediaPipe
