# Spot-Sumo - SpotMicro Quadruped Locomotion

**Status: Ongoing research project**

A sim-to-real locomotion project for [SpotMicro](https://github.com/mike4192/spotMicro), an open-source 12-DOF quadruped robot. Combines a corrected inverse-kinematics solver, Bezier-curve gait generation, and a lightweight learned gait-correction RL policy, validated in PyBullet and MuJoCo, with hardware deployment in progress.

<p align="center">
  <img width="842" height="720" alt="robo-dog mujoco sim" src="https://github.com/user-attachments/assets/7856f2ee-ee63-4efe-acf3-01195483010e" /><br>
  <em>Simulated walking gait — MuJoCo</em>
</p>

## Overview

- Analytical IK solver derived from the robot's own URDF joint axes
- 12-point Bezier curve gait generator, with omnidirectional motion (forward / backward / strafe / yaw)
- Small learned residual policy for gait correction, trained in simulation
- Cross-simulator validation: PyBullet → MuJoCo
- Physical hardware build in progress 

A short write-up of the approach and a couple of the more interesting findings along the way.

## Media

| | | |
|---|---|---|
<img width="1197" height="785" alt="image_1" src="https://github.com/user-attachments/assets/a74f0592-0031-43e7-9e0d-e2711f6d5395" /><img width="721" height="707" alt="image_3" src="https://github.com/user-attachments/assets/222c49ef-a12a-4c14-af82-35bfee80f873" />
<img width="725" height="608" alt="image_2" src="https://github.com/user-attachments/assets/e6b35256-fff8-4abb-85d9-5836614147e4" />


*More clips and build photos added as hardware progress continues.*

## Status / Roadmap

- [x] Open-loop Bezier gait — simulation
- [x] IK correction validated
- [x] Cross-simulator transfer (PyBullet → MuJoCo)
- [ ] Learned policy — hardware validation
- [ ] Physical build — walking demo

## Acknowledgements

Built on the SpotMicro mechanical design/URDF by Mike Reiter, and informed by the D²-GMBC gait modulation framework (Rahme et al., 2020).

---
*Code and detailed writeup to follow as the project matures. Reach out via [email](mailto:a.sohail@ceme.nust.edu.pk) for early access or collaboration.*
