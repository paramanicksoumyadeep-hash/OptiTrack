# OptiTrack (pypogs) - Optical Ground Station Simulator

OptiTrack (based on pypogs) is an interactive, web-based Portable Optical Ground Station Simulator. It features a rich graphical user interface for visualizing optical satellite tracking, simulating camera feeds, injecting atmospheric disturbances, and providing an immersive 3D/WebXR view of the optical link.

##  Live Demo

[**Try the Live Demo Here**](https://opti-track-ten.vercel.app/)

*(Note: Ensure GitHub Pages is enabled in your repository settings on the `main` branch or `gh-pages` branch to make this link active.)*

##  Features

- **Simulated Camera Feed:** Real-time rendering of a sensor feed including star fields, drifting satellite targets, and a closed-loop tracking reticle.
- **Interactive Control Panels:** Draggable floating windows for hardware setup, manual control, alignment, and tracking metrics.
- **Disturbance Engine:** Inject real-time atmospheric and platform noise, including Scintillation, Wavefront Distortion, and Platform Jitter.
- **Tracking Metrics:** Live visualization of tracking error RMSE (pixels) and CNN fallback confidence using sparklines and animated charts.
- **3D Immersive View (WebXR):** A Three.js-powered 3D perspective from the ground station. Includes a 15-satellite constellation, targeting reticle, satellite telemetry cards, and simulated optical/laser communication links.
- **Responsive UI:** Custom-styled JetBrains Mono console, hardware controls, and live telemetry updates mimicking a real-world pypogs terminal.

## 🛠️ Technologies Used

- **HTML5/CSS3:** Custom interface with draggable panels and a dark-mode styling tailored for technical applications.
- **JavaScript (ES6):** Real-time simulation loop, PID-like tracking logic, and canvas rendering for the camera feed.
- **Three.js & WebXR:** Rendering the 3D ground station environment, procedural Earth/ground textures, and satellite orbits with immersive VR support.

## 💻 Getting Started

To run the simulator locally:

1. Clone this repository:
   ```bash
   git clone https://github.com/paramanicksoumyadeep-hash/OptiTrack.git
   ```
2. Open the directory and serve it using a local development server. You can use the provided PowerShell script:
   ```powershell
   ./serve.ps1
   ```
   Or use Python:
   ```bash
   python -m http.server 8000
   ```
3. Navigate to `http://localhost:8000` (or the port specified by your server) to interact with the OptiTrack interface.

## 🎮 How to Use

1. **Start Tracking:** Click the `▶ Start Tracking` button in the Control Panel to engage the closed-loop tracking. Watch the reticle acquire the target in the simulated camera feed.
2. **Adjust Disturbances:** Find the "Disturbance Engine" panel and adjust the sliders to see how scintillation, wavefront distortion, and platform jitter affect the tracking RMSE.
3. **Enter 3D View:** Click the `🛰 3D OPTICAL LINK VIEW` button in the bottom bar to switch to the Three.js immersive scene. Target satellites and initiate simulated optical signals.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
