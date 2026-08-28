# Hi 👋, I'm Jalanth S

🎓 **B.Tech CSE (AI & ML) @ PES University (2027)**<br>
🤖 **Robotics • Autonomous Systems • Computer Vision**<br>
🔗 [LinkedIn](https://www.linkedin.com/in/jalanth-s/) &nbsp;|&nbsp; ✉️ jalanth9342@gmail.com

---

## 🚀 About Me

I build **autonomous machines** — drones and ground robots that perceive their
surroundings and decide where to go without a human in the loop.

🔭 **Building** — [Drone Autonomy in ROS 2](https://github.com/jalanths/Drone-Autonomy-ROS2): VFH+ avoidance, smart retrace, full autonomous missions on ArduPilot SITL<br>
🌱 **Learning** — semantic segmentation, headed for on-board inference on the Hailo-8 AI HAT<br>
🤝 **Open to** — open-source robotics and hardware/AI integration; anything with a Pixhawk in it<br>
💬 **Ask me about** — training YOLOv8 detectors, ENU vs NED frame conventions, or wiring an ESP32 to a servo<br>
⚡ **Fun fact** — my drone's first avoidance system only worked when flying **east**. "Front" was hard-coded to `+x` of the `odom` frame, so *dodge left* meant *dodge north* no matter which way the nose was pointing.

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

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black) ![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Robotics & Autonomy**

![ROS 2](https://img.shields.io/badge/ROS%202-22314E?style=for-the-badge&logo=ros&logoColor=white) ![Nav2](https://img.shields.io/badge/Nav2-4B8BBE?style=for-the-badge) ![SLAM Toolbox](https://img.shields.io/badge/SLAM%20Toolbox-5A5A5A?style=for-the-badge) ![MAVROS](https://img.shields.io/badge/MAVROS-2C3E50?style=for-the-badge) ![MAVLink](https://img.shields.io/badge/MAVLink-1B5E20?style=for-the-badge) ![ArduPilot](https://img.shields.io/badge/ArduPilot-C62828?style=for-the-badge) ![Gazebo](https://img.shields.io/badge/Gazebo-F58113?style=for-the-badge) ![RViz2](https://img.shields.io/badge/RViz2-37474F?style=for-the-badge) ![Pixhawk](https://img.shields.io/badge/Pixhawk-263238?style=for-the-badge)

**AI / Computer Vision**

![YOLOv8](https://img.shields.io/badge/YOLOv8-111F68?style=for-the-badge) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white) ![scikit--learn](https://img.shields.io/badge/scikit----learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) ![NLTK](https://img.shields.io/badge/NLTK-154F5B?style=for-the-badge)

**Web & 3D**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) ![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white) ![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)

**IoT & Hardware**

![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white) ![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white) ![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white) ![Node--RED](https://img.shields.io/badge/Node----RED-8F0000?style=for-the-badge&logo=nodered&logoColor=white) ![RPLiDAR](https://img.shields.io/badge/RPLiDAR-455A64?style=for-the-badge) ![ZeroMQ](https://img.shields.io/badge/ZeroMQ-DF0000?style=for-the-badge)

**Tools & Platforms**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)

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
