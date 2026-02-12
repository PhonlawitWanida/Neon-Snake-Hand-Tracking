# Neon-Snake-Hand-Tracking
An interactive web-based Snake game controlled by real-time hand gestures using MediaPipe Hands and face-api.js, featuring a neon UI and a unique Face Yoga challenge.
# 🐍 Neon Snake: Hand-Tracking & Face Yoga Edition

An interactive, web-based adaptation of the classic Snake game, powered by real-time Computer Vision. This project replaces traditional keyboard inputs with **Hand Gesture Controls** and introduces a unique **Face Yoga Challenge** to unlock new levels, demonstrating seamless integration of AI models into web applications.

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Tech Stack](https://img.shields.io/badge/Tech-HTML%20|%20CSS%20|%20JS-blue)
![AI Models](https://img.shields.io/badge/AI-MediaPipe%20|%20face--api.js-orange)

---

## 📸 Demo & Screenshots
!(picture/1.gif)
!(picture/2.gif)

---

## 🚀 Key Features

* **🖐️ Real-Time Hand Tracking:** Utilizes MediaPipe Hands to detect index finger coordinates, translating them into directional velocity for the snake.
* **😎 Face Yoga (Facial Landmarks):** Integrates `face-api.js` to detect facial landmarks. Players must successfully capture specific face poses to unlock higher difficulty levels.
* **🕹️ Dynamic Gameplay Logic:** The game speed, obstacles, and grid complexity dynamically adapt as the player progresses.
* **✨ Cyberpunk/Neon UI:** Designed a responsive, visually engaging interface using HTML5 Canvas and CSS3.

---

## 🛠️ Technology Stack

* **Frontend:** HTML5 (Canvas API), CSS3 (Neon UI styling), Vanilla JavaScript.
* **Computer Vision & AI:** * [MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker) (Gesture recognition)
  * [face-api.js](https://github.com/justadudewhohacks/face-api.js) built on TensorFlow.js (Facial landmark detection)
* **Architecture:** Client-side processing (AI models run directly in the browser for zero-latency interactions).

---

## 🧠 How It Works (The CV Pipeline)

1. **Video Capture:** The browser accesses the user's webcam via the `navigator.mediaDevices` API.
2. **Inference & Processing:** * Video frames are continuously fed into the MediaPipe and face-api.js models.
   * The models return a structured JSON containing the X and Y coordinates of specific landmarks (e.g., tip of the index finger, 68 face landmarks).
3. **Logic Mapping:** JavaScript logic normalizes these coordinates to the game's Canvas dimensions, determining the snake's next move based on the user's physical position.

---

## 💻 Installation & Setup

Since this project relies on client-side web technologies and webcam access, it needs to be run on a local server.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/PhonlawitWanida/neon-snake-hand-tracking.git](https://github.com/PhonlawitWanida/neon-snake-hand-tracking.git)
