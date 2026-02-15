# Ryomen-Sukuna
# ⛩️ DOMAIN EXPANSION: MALEVOLENT SHRINE

> **"Know your place, fool."**

A high-performance, interactive web visualizer that uses computer vision to render Ryomen Sukuna's cursed techniques in real-time. Built with **Three.js** for 3D particle systems and **MediaPipe** for hand tracking.

## 🔮 Overview

This project simulates a **Domain Expansion** inside your browser. It uses your webcam to track hand gestures and instantly transmutes 15,000+ WebGL particles into the various attacks of Ryomen Sukuna from *Jujutsu Kaisen*.

The simulation features:

* **Volumetric Particle Physics:** Smooth damping and interpolation for fluid movement.
* **Post-Processing:** Unreal-style bloom and glow effects.
* **Optimized Performance:** Throttled AI detection and half-res rendering for maximum FPS.

## 🖐️ Controls & Techniques

Use your hand to command the Cursed Energy. The system detects specific gestures to trigger different states:
```
| Technique | Hand Gesture | Visual Effect |
| --- | --- | --- |
| **Malevolent Shrine** | ✊ **Fist / Prayer** (All fingers closed) | Constructs the 4-pillar Shinto shrine with a spectral maw. |
| **Dismantle** | ✋ **Open Hand** (All fingers extended) | High-speed, horizontal slashing planes. |
| **Cleave** | ✌️ **Two Fingers** (Index + Middle up) | A chaotic, spiderweb-like cutting grid. |
| **Kamino (Fuga)** | 👌 **Pinch** (Index + Thumb touching) | Generates a dense fireball and rising flame tornado. |
| **Neutral** | **Relaxed / None** | Particles drift as ambient cursed dust. |
```

## 🚀 How to Run

### Option 1: Quick Start (VS Code)

1. Save the code as `index.html`.
2. Install the **Live Server** extension in VS Code.
3. Right-click the file and select **"Open with Live Server"**.
4. Allow camera permissions when prompted.

### Option 2: Python Simple Server

If you have Python installed, you can run a local server in the folder where you saved the file:

```bash
# Python 3
python -m http.server 8000

```

Then open `http://localhost:8000` in your browser.

> **Note:** This project requires an active internet connection to load the Three.js and MediaPipe libraries via CDN.

## 🛠️ Technologies Used

* **[Three.js](https://threejs.org/)**: The 3D engine used for rendering the particle system.
* **[MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker)**: Google's machine learning model for real-time hand tracking.
* **EffectComposer**: For the "Cursed Energy" bloom and post-processing effects.

## ⚙️ Customization

You can tweak the constants in the `<script>` tag to adjust the experience:

* `COUNT`: Number of particles (Default: 15,000). Increase for density, decrease for performance.
* `bloomPass.strength`: Intensity of the glow.
* `lerpFactor`: Speed of the particle transition.

## ⚠️ Disclaimer

This is a fan-made project inspired by *Jujutsu Kaisen*. Please do not use this domain expansion on innocent civilians in Shibuya.
