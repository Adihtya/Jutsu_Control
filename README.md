# Jutsu Control: Naruto & Sasuke AR Hand-Tracking Experience

An interactive browser-based Augmented Reality (AR) application powered by MediaPipe Hands. Harness your chakra to summon Naruto's Rasengan / Rasenshuriken, cast Sasuke's Chidori, or launch high-velocity ninja shurikens in real-time using only your webcam and hand gestures.

---

## Features

- **Real-Time Hand Tracking**: Powered by `@mediapipe/hands` to track up to two hands at high frame rates directly in the browser.
- **Naruto Mode (Left Hand)**:
  - Open your left hand to charge up a Rasengan / Rasenshuriken overlay over your palm.
  - Fully charge your chakra and perform a fast flicking motion to launch a spinning Rasenshuriken across the screen.
- **Sasuke Mode (Right Hand)**:
  - Open your right hand to ignite Sasuke's electric Chidori, complete with real-time positional tracking.
- **Audio & Visual FX Integration**:
  - Screen blending modes (`mix-blend-mode: screen`) for seamless lighting integration over the live camera feed.
  - Synchronized jutsu sound effects with automatic gesture triggering and browser-compliant audio unlocking.
- **Glow Skeleton Visualization**: High-contrast neon-cyan hand skeleton and landmark overlay for intuitive feedback.

---

## Gestures & Controls

| Action | Hand | Gesture / Movement |
| :--- | :--- | :--- |
| **Summon Rasengan** | Left Hand | Open hand (at least 3 extended fingers) |
| **Summon Chidori** | Right Hand | Open hand (at least 3 extended fingers) |
| **Throw Rasenshuriken** | Left Hand | Fully charge power (`≥ 85%`), then flick your wrist rapidly |
| **Unlock Sound** | Any | Tap/click anywhere on the screen once |

---

## File Structure & Assets

Make sure the following files are located in the same directory:

```text
jutsu-control/
│
├── index.html          # Main HTML, styling, and MediaPipe logic (naruto_sasuke.html)
├── naruto.mp4          # Rasengan/Rasenshuriken visual overlay video
├── sasuke.mp4          # Chidori visual overlay video
├── shuriken.mp4        # Flying projectile visual overlay
├── chidori.mp3         # Chidori sound effect
├── shuriken.mp3        # Shuriken/Rasenshuriken throw sound effect
└── LICENSE             # Apache 2.0 License
