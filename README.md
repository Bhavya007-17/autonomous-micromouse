# autonomous-micromouse

An autonomous maze-solving micromouse robot — a small wheeled robot that maps a maze and drives itself to the center.

![Status](https://img.shields.io/badge/status-early%20development-orange)
![Domain](https://img.shields.io/badge/domain-robotics%20%2F%20embedded-blue)

## Overview

`autonomous-micromouse` is an early-stage robotics project to build a [Micromouse](https://en.wikipedia.org/wiki/Micromouse) — a compact autonomous robot that explores an unknown grid maze, builds an internal map, and then plans and drives the fastest route to the goal. This repository is the home for the firmware, hardware notes, and design files as the project develops.

> This repo is currently a placeholder being scaffolded. The sections below describe the intended design; concrete details are marked `TODO:` and will be filled in as hardware and firmware come together.

## Planned features

- Wall detection and maze mapping from onboard distance sensors
- Maze-solving / shortest-path planning (e.g. flood-fill)
- Closed-loop motor control with encoder odometry
- Exploration run followed by an optimized speed run

## Tech stack (planned)

- TODO: confirm microcontroller (e.g. STM32 / ESP32 / RP2040)
- TODO: sensors (IR / ToF distance sensors, IMU)
- TODO: motors + encoders and motor driver
- TODO: firmware language (C/C++)

## How it works (intended)

1. **Explore** — drive the maze, reading wall sensors at each cell and recording the layout.
2. **Map** — maintain an internal grid representation of discovered walls.
3. **Plan** — compute the shortest path from start to center (flood-fill / BFS).
4. **Speed run** — execute the planned path with tuned motion control.

## Getting started

TODO: add build/flash instructions once firmware and hardware are defined.

## Status

Early development — design and scaffolding phase.

## Roadmap

- TODO: finalize hardware selection and bill of materials
- TODO: bring up motor control + encoder odometry
- TODO: implement wall sensing and maze mapping
- TODO: implement flood-fill solver and speed run
- TODO: add photos and a demo video

## License

MIT — see the [LICENSE](LICENSE) file.

## Contact

Bhavya Dosi — [LinkedIn](https://www.linkedin.com/in/bhavya-dosi)
