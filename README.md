# Hi 👋, I'm Jalanth S

🎓 **B.Tech CSE (AI & ML) @ PES University (2027)**<br>
🤖 **Robotics • Autonomous Systems • Computer Vision**<br>
🔗 [LinkedIn](https://www.linkedin.com/in/jalanth-s/) &nbsp;|&nbsp; ✉️ jalanth9342@gmail.com

---

## 🚀 About Me

I build **autonomous machines** — drones and ground robots that perceive their
surroundings and decide where to go without a human in the loop.

My work sits at the intersection of **ROS 2, flight control, and real-time
perception**: VFH+ obstacle avoidance on live LiDAR, SLAM and Nav2 waypoint
missions, YOLOv8 target tracking streamed between a companion Pi and a host GPU,
and MAVLink/MAVROS bridges down to Pixhawk hardware.

I care about systems that actually fly, not just simulations that compile.

---

## ⚡ Featured Project

### 🚁 [Drone Autonomy in ROS 2](https://github.com/jalanths/Drone-Autonomy-ROS2)

> Autonomous 6-waypoint navigation with dynamic obstacle avoidance and smart retrace.

```
ARM → TAKEOFF → WP1 … WP6  (live avoidance) → SMART RETRACE → LAND
```

- **VFH+ steering in the ENU frame** — 72 × 5° polar histogram fusing raw `/scan`
  (zero-latency) with the Nav2 costmap (persistent, inflated memory)
- **Angular enlargement** — obstacle arcs widen by `γ = asin(r_safe / d)`, replacing
  a table of hand-tuned distance thresholds with one line
- **Corridor selection + hysteresis** — commits to one side of an obstacle instead
  of dithering across its centreline
- **Trap escape** — climbs out when boxed in on all 360°
- **Smart retrace** — drops breadcrumbs only where the path was proven clear, then
  walks them back in reverse with avoidance still armed
- Simulated on **ArduPilot SITL + Gazebo Classic 11** (123 static + 4 moving obstacles),
  visualised in **RViz2**

**Hardware target:** Pixhawk 2.4.8 · Raspberry Pi 5 · Slamtec RPLiDAR C1M1-R2 · Hailo-8 AI HAT

---

## 🧠 Tech Stack

**Robotics & Autonomy**

`ROS 2 Humble` • `Nav2` • `slam_toolbox` • `AMCL` • `MAVROS` • `MAVLink` • `ArduPilot SITL` • `Gazebo` • `RViz2` • `colcon`

**AI / Computer Vision**

`YOLOv8` • `Ultralytics` • `OpenCV` • `scikit-learn` • `NLTK` • `TF-IDF` • `NumPy`

**Languages**

`Python` • `C++` • `TypeScript` • `JavaScript` • `Dart / Flutter` • `HTML/CSS`

**Web & 3D**

`React 19` • `Three.js` • `React Three Fiber` • `Tailwind` • `Vite` • `Flask`

**Systems & Hardware**

`Ubuntu 22.04` • `Linux` • `Git` • `ZeroMQ` • `MQTT` • `Node-RED` • `ESP32` • `Pixhawk` • `Raspberry Pi 5` • `RPLiDAR` • `Picamera2`

---

## 🛠️ Key Projects

### 🚁 [Drone Autonomy in ROS 2](https://github.com/jalanths/Drone-Autonomy-ROS2)
Autonomous waypoint missions with live 3D collision avoidance
- VFH+ avoidance fusing LiDAR + Nav2 costmap
- Smart retrace over proven-clear breadcrumbs
- ArduPilot SITL + Gazebo + MAVROS stack

### 🤖 [Disaster-Response Mobile Robot](https://github.com/jalanths/Disaster-Response-Mobile-Robot)
ROS 2 ground robot for disaster-zone search and survey
- Online async SLAM + AMCL localisation in a custom Gazebo world
- Nav2 waypoint missions (`search_sweep`) with runtime dynamic obstacles
- YOLOv8 detection, anomaly flagging, battery simulation
- Live web telemetry + camera dashboard

### 🎯 [Human-Tracking & Following Drone](https://github.com/jalanths/Human-Tracking-And-Following-Drone)
Distributed lock-on autopilot across Pi and host GPU
- Picamera2 → TCP video stream → YOLOv8 inference on the host
- Click to lock on; IoU tracking holds the target through occlusion
- ZeroMQ pub/sub feeds MAVLink yaw + forward-velocity commands to Pixhawk

### 🏭 [Digital Twin Conveyor](https://github.com/jalanths/Digital-Twin-Conveyor)
Interactive 3D digital twin of a robotic sorting line
- React Three Fiber scene driving a custom GLTF robotic arm
- Live production metrics and per-line box counts
- 0.1×–10× speed control and timeline scrubbing

### 📰 [News Classification](https://github.com/jalanths/news-classification-mini-project)
End-to-end NLP pipeline on the BBC news corpus
- Lemmatisation + TF-IDF (5000 features)
- Naïve Bayes / Logistic Regression / Linear SVM compared — **98.88%** accuracy
- Deployed as a Flask web app

---

## 🏆 Achievements

**🥇 1st Place — EmbedX Hackathon (Xlyem, IoT & Embedded Systems)** · PES University, Bengaluru · Feb 2026
- Won first place against multiple teams for an end-to-end IoT solution
- Built a **Smart Water Management & Leak Detection System** — ESP32, MQTT, Node-RED dashboard,
  autonomous shutoff, and real-time anomaly detection

**🛡️ PARXIS Hackathon (AI/ML Department)** · PES University, Bengaluru · Mar 2026
- AI/ML vulnerability assessment and red-teaming
- Built **ThreatLens** — an AI model vulnerability scanner evaluating LLMs against the **OWASP Top 10**,
  with dual-layer detection and adaptive payload generation

**⚙️ Ignition Hackathon** · PES University, Bengaluru · Nov 2025
- End-to-end IoT build: hardware interfacing, embedded programming, backend connectivity

**📜 Certifications**
- **AI and Big Data in IoT** — Great Learning · Oct 2025
- **App Development using Flutter** — PESU I/O, PES University · Oct–Nov 2024

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=jalanths&show_icons=true&theme=tokyonight&hide_border=true" height="165" alt="Jalanth's GitHub stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=jalanths&layout=compact&theme=tokyonight&hide_border=true" height="165" alt="Top languages" />
</p>

---

## 🔗 Connect with Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jalanth-s/)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jalanth9342@gmail.com)

---

⭐ Currently building: autonomy that survives contact with real hardware.
