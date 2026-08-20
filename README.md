# Spot-Sumo — SpotMicro Quadruped Locomotion

**Status: 🚧 Ongoing research project**

A sim-to-real locomotion project for [SpotMicro](https://github.com/mike4192/spotMicro), an open-source 12-DOF quadruped robot. Combines a corrected inverse-kinematics solver, Bezier-curve gait generation, and a lightweight learned gait-correction policy, validated in PyBullet and MuJoCo, with hardware deployment in progress.

<p align="center">
  <img src="media/walk_demo.gif" width="480" alt="SpotMicro walking demo — GIF placeholder"><br>
  <em>Simulated walking gait — MuJoCo</em>
</p>

## Overview

- Analytical IK solver derived from the robot's own URDF joint axes
- 12-point Bezier curve gait generator, with omnidirectional motion (forward / backward / strafe / yaw)
- Small learned residual policy for gait correction, trained in simulation
- Cross-simulator validation: PyBullet → MuJoCo
- Physical hardware build in progress (Raspberry Pi 4)

A short write-up of the approach and a couple of the more interesting findings along the way is here: [`docs/notes.md`](docs/notes.md) *(placeholder — link to trimmed preprint)*.

## Media

| | | |
|---|---|---|
| ![placeholder](media/thumb1.png) | ![placeholder](media/thumb2.png) | ![placeholder](media/thumb3.png) |

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
