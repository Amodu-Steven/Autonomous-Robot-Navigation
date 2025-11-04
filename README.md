# Autonomous Mobile Robot Navigation Using Pioneer 3-DX

 ### [YouTube Demonstration](https://www.youtube.com/watch?v=b7HCgPpURcM&t=40s)


<h2>Description</h2>
This project implements autonomous navigation, obstacle avoidance, and target tracking behaviors using the Pioneer 3-DX mobile robot in a living laboratory environment. The robot successfully navigates from a fixed starting point to an endpoint while demonstrating three key robotic behaviors: odometry-based navigation, target tracking, and obstacle avoidance. The system utilizes various sensors including sonar arrays and implements mathematical models for precise movement control.
<br />

<h2>Technologies and Tools Used</h2>

- <b>Pioneer 3-DX Mobile Robot</b>
- <b>Java JDK</b> 
- <b>IntelliJ IDEA</b>
- <b>ARIA Robotics API</b>
- <b>MobileSim</b> (Simulation Environment)
- <b>Mapper3</b> (Map Creation)
- <b>OpenCV</b>

<h2>Hardware Specifications</h2>

- <b>Robot Platform</b>: Pioneer 3-DX
- <b>Dimensions</b>: 485mm × 381mm × 217mm
- <b>Weight</b>: 9 KG
- <b>Max Speed</b>: 1.2 m/s
- <b>Sensors</b>: 8-sonar array (0.1m-5m range)
- <b>Processing</b>: Intel Celeron Dual-Core J1800, 4GB RAM

<h2>Project Implementation</h2>

<p align="center">
Robot Hardware Setup: <br/>
![Pioneer 3-DX](media/robot-setup.jpg) <!-- Replace with your image -->
<br />
<br />

Navigation Map:  <br/>
![Living Lab Map](media/lab-map.png) <!-- Replace with your image -->
<br />
<br />

Odometry Trajectory:  <br/>
![Trajectory Results](media/trajectory-plot.png) <!-- Replace with your image -->
</p>

<h2>Key Features</h2>

- <b>Odometry Navigation</b>: Precise movement between predefined nodes using dead reckoning
- <b>Target Tracking</b>: Visual object tracking using color blob detection
- <b>Obstacle Avoidance</b>: Real-time collision avoidance using sonar sensors
- <b>Mathematical Modeling</b>: Implementation of angular and linear transition models
- <b>Data Analysis</b>: Covariance and correlation analysis of navigation performance

<h2>Navigation Algorithms</h2>

**Odometry Model:**
- Angular transition based on arc-tangent function
- Linear transition using Euclidean distance
- Threshold values: γd = ±200, γθ = ±2.9

**Obstacle Avoidance:**
- Sonar-based collision detection (S0-S7 sensors)
- Collision vector (vc), Avoidance vector (va), Untrap vector (vu)
- Dynamic direction changes based on sensor input

**Target Tracking:**
- Color blob detection and tracking
- Approach vector (va) and Tracking vector (vt) implementation
- Continuous target following capability

<h2>Experimental Results</h2>

**Odometry Performance (Node 1 to 5):**
- Covariance (COVd,t) = -0.3709
- Correlation coefficient (ρ) = -0.12741

**Tracking Performance (Node 5 to 7):**
- Covariance = 0.259478
- Correlation coefficient (ρ) = 0.158713




<h2>Installation & Setup</h2>

1. **Software Requirements:**
   - Install Java JDK 1.7+
   - Install IntelliJ IDEA
   - Download ARIA Robotics API
   - Install MobileSim for simulation

2. **Hardware Setup:**
   - Connect Pioneer 3-DX robot
   - Configure sonar sensors
   - Set up power supply and batteries
   - Establish communication link

3. **Run the Project:**
   ```bash
   # Compile and run in IntelliJ
   javac -cp "Aria.jar" *.java
   java -cp ".;Aria.jar" Run

<h2>Skills Demonstrated</h2>

Autonomous robot navigation system design

Sensor integration and data processing

Mathematical modeling of robot kinematics

Experimental data analysis and interpretation

Robotics software development in Java

Simulation and real-world testing

Statistical analysis of robot performance

<h2>Future Work</h2>
Implement SLAM (Simultaneous Localization and Mapping)

Integrate additional sensors (LiDAR, IMU)

Develop machine learning-based navigation

Enhance obstacle detection algorithms

Multi-robot coordination and swarm intelligence

<br /> <br />
