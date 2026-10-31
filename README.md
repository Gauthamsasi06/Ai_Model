# 🚦 TRAFFIC PULSE - Real-Time Autonomous Grid Command & Analytics

A futuristic, cyber-themed real-time traffic simulation and analytics frontend built entirely with pure client-side JavaScript, HTML5 Canvas, and Tailwind CSS.

> [!NOTE]
> **Single-File Architecture**: This entire application is packaged into a **100% self-contained `index.html`** file. There are no subfolders or complex asset dependencies required, making it effortless to upload and host directly on GitHub.

---

## 🚀 Instant Deployment to GitHub & GitHub Pages

### Method 1: GitHub Web UI (Drag & Drop)
1. Go to [github.com](https://github.com) and create a new repository (e.g. `traffic-pulse`).
2. Click **"upload an existing file"**.
3. Drag and drop `index.html` and `README.md` into the browser and click **Commit changes**.
4. Go to **Settings** ➔ **Pages**.
5. Under **Branch**, select `main` and root `/` folder, then click **Save**.
6. Your live website URL will be ready at: `https://<your-username>.github.io/<repo-name>/`!

### Method 2: Git CLI
```bash
git init
git add index.html README.md
git commit -m "Initial commit: Real-time Traffic Pulse simulation"
git branch -M main
git remote add origin https://github.com/<your-username>/traffic-pulse.git
git push -u origin main
```

---

## 🌟 Key Simulation Features

### 1. 🏎️ JavaScript Physics Engine (IDM + MOBIL)
- **Intelligent Driver Model (IDM)**: Smooth acceleration, safe headway distance maintenance, and realistic reaction braking.
- **Dynamic Lane Changing**: Vehicles inspect adjacent lane speeds and merge around slow vehicles or road obstructions.
- **7 Vehicle Types**:
  - `Cyber EV`: High acceleration, regenerative braking, ultra-high eco score.
  - `Executive Sedan`: Standard commuter vehicle with smooth cruising physics.
  - `Metro Taxi`: Checkered roof livery, frequent turning patterns.
  - `Delivery Van`: Medium commercial cargo carrier with cautious braking profiles.
  - `18-Wheeler Heavy Semi-Truck`: Extended articulated chassis, heavy inertia, longer stopping distances.
  - `Emergency Unit (Ambulance)`: Flashing siren strobes, priority right-of-way, and automated signal preemption.
  - `Motorbike`: Nimble, high acceleration, quick lane weaving.

### 2. 🚦 Smart Traffic Signals & Emergency Preemption
- **Adaptive AI Mode**: Continuously evaluates queued cars and waiting delays to dynamically switch green phases and clear bottlenecks.
- **Fixed Timer Mode**: Statutory signal cycles with countdown timers.
- **Green Wave Corridor**: Dynamic synchronization for continuous high-speed flow.
- **Emergency Priority Preemption**: Instantly triggers a green wave when an emergency vehicle approaches, while surrounding vehicles yield.
- **Interactive Manual Override**: Click any traffic signal gantry to manually trigger a phase change.

### 3. 🌧️ Dynamic Weather & Atmosphere
- **Cyber Night**: Dark asphalt, neon lane dividers, headlight beam projections, and ambient signal bloom.
- **Torrential Rainstorm**: Animated rain particles, puddle reflections, and a 25% friction reduction requiring longer braking distances.
- **Clear Daylight**: Clean high-contrast metropolitan layout.

### 4. 📊 Real-Time Analytics & Live Charts
- **Live Telemetry KPIs**:
  - Active Grid Fleet count
  - City Congestion Index (0% free flow to 100% gridlock with dynamic color status)
  - Mean Grid Velocity (km/h)
  - Average Signal Delay (seconds stopped per car)
  - Carbon Intensity (g CO2/s based on vehicle idling and acceleration)
  - Intersection Throughput (vehicles cleared per minute)
- **Zero-Dependency Canvas Charts**:
  - **Velocity & Congestion Timeline**: 60-second rolling dual-line graph.
  - **Corridor Density Bars**: Real-time queue depths across North, South, East, and West arteries.
  - **Fleet Breakdown Donut Chart**: Proportional mix of active vehicle types.
  - **Congestion Speedometer Gauge**: Color-coded arc gauge reflecting instant grid pressure.
- **Autonomous AI Advisory Feed**: Evaluates bottleneck risk, recommends signal cycle extensions, and provides environmental emission tips.
- **Vehicle Telemetry Inspector**: Left-click any vehicle on the map to inspect its real-time ID, velocity, driver state, trajectory, wait time, and eco rating.

### 5. 🔊 Self-Contained Web Audio Synthesizer
- Generates UI blips, alert chimes, and ambulance sirens dynamically using the Web Audio API without requiring any external audio files.

---

## 🕹️ Interactive Controls

| Action | Control |
| :--- | :--- |
| **Inspect Vehicle** | Left-click any vehicle on the road |
| **Place Roadblock / Hazard** | Click **"🚧 Place Road Hazard"**, then click on any lane |
| **Remove Hazard** | Click directly on an active orange hazard cone |
| **Manual Signal Switch** | Click any traffic light gantry or click **"⚡ Flip Signal"** |
| **Dispatch Ambulance** | Click **"🚨 Emergency Dispatch"** |
| **Adjust Spawn Rate** | Drag the **"Spawn Flow"** slider (0.4/s to 3.5/s) |
| **Simulation Speed** | Select `0.5x`, `1.0x`, `2.0x`, or `4.0x` |
| **Sound Effects** | Click **"🔇 Sound: OFF / ON"** to toggle synthesizer |
| **Weather Modes** | Click `🌙 Night`, `🌧️ Rain`, or `☀️ Day` |
