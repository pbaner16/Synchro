# Synchro — Wireless Motion Intelligence Finger Ring

Synchro is a state-of-the-art marketing landing page and mobile-optimized companion app for a wearable finger ring that wirelessly tracks limb and joint movement for physical rehabilitation, athletic performance, and fitness metrics. Think Oura Ring's compact elegance meets Whoop's high-fidelity athletic credibility.

## 🚀 Live Demo & Preview

This project contains two primary pages that can be run locally without any installation or build systems:

1. **Product Landing Page (`index.html`):** A high-performance, dark-themed marketing landing page featuring a fully interactive **Three.js 3D Smart Ring** with custom metallic materials, dynamic lighting highlights, and cursor-parallax tracking orbits.
2. **Companion Web App (`app.html`):** A mobile-optimized, standalone web app simulating the Synchro companion interface. It includes an interactive **3D Real-time Motion Tracking Visualizer** that can sync with physical mobile device gyro/orientation sensors.

---

## 🛠️ Features & Design Identity

### 🎨 Visual & Motion Identity
- **Background:** `#0A0B0F` (Pitch dark)
- **Surfaces:** `#12141A` (Gravel card surfaces)
- **Accent Color:** `#00D4C8` (Teal neon glow)
- **Typography:**
  - Headings: `Syne` (Geometric, wide letter-spacing)
  - Body: `DM Sans` (Premium sans-serif readability)
  - Data & Metrics: `JetBrains Mono` (Tabular tech figures)
- **Interactivity:** Fluid scroll-driven entries via `IntersectionObserver` and responsive grid layouts.

### 📱 Companion Web App & Instrument Dexterity Trainer (`app.html`)
- **Overview Dashboard:** Features a dynamic animated progress ring showing the daily "Move Index", activity streaks, and battery telemetry.
- **Instrument Dexterity Visualizer:** A high-fidelity 3D kinesthetic tracking environment featuring a procedurally-modeled **5-finger human hand** (with realistic skin tones, joint knuckles, fingernails, and the smart ring on the index finger).
- **Instrument Modes:**
  - **Violin:** The hand forms a realistic bow grip to move the bow across the bridge and steel strings, tracking bow strokes and angle deviations.
  - **Guitar:** The index finger presses down on an angled fretboard with glowing fretted strings, tracking chord changes and fret alignment accuracy.
  - **Piano:** The hand rests over a 3-key piano keyboard, dynamically bending knuckles to press the keys down in response to user motion.
- **Device Telemetry:** Automatically binds to the **DeviceOrientation API** on mobile devices for accelerometer-driven play simulation, falling back to interactive mouse dragging on desktop.
- **Analytics & History:** Interactive weekly range of motion columns and mock clinical PDF exports.

---

## 💻 Running the Project Locally

Since the project uses pure HTML, CSS, and vanilla JS (loading Three.js from a standard CDN), you can preview the pages in two ways:

### Method 1: Python Local HTTP Server (Recommended)
Starting a local server is the best way to test, especially on mobile devices connected to the same local network:

1. Open your terminal in the project directory.
2. Start the local server:
   ```bash
   python3 -m http.server 8000
   ```
3. Open your browser and navigate to:
   - Landing Page: [http://localhost:8000](http://localhost:8000)
   - Companion App: [http://localhost:8000/app.html](http://localhost:8000/app.html)

### Method 2: Open Files Directly
Double-click `index.html` or `app.html` to open them directly in your web browser. Note that some mobile device orientation APIs require secure origins or server contexts (Method 1) to retrieve accelerometer permissions.

---

## 📂 Project Structure

```
Synchro/
├── index.html       # Marketing Landing Page with Three.js Hero
├── app.html         # Mobile Companion Web App with Live tracking
└── README.md        # Project guide and documentation
```
