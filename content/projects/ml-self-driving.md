---
title: 'Self Driving Racecar'
date: 2024-05-24
draft: false
cover:
    image : "projects/ml-self-driving/cover.png"
---
[GitHub Repository](https://github.com/Gibson431/ai-in-robotics-41118)

This project was done as part of a university project for a subject called "AI in Robotics".

The assignment required us to design and implement any project we could think of (that had to first be approved).

The chosen project was based on the [Formula SAE-A](https://www.saea.com.au/formula-sae-a) Autonomous Division, using the same track and cone styles.

The assignment included grading on documentation via the repository's wiki tab, as well as git project management.

The group received a high distinction for this assignment and I received a high distinction for the subject as a whole.

## Project Details

- [PyBullet](https://pybullet.org/wordpress/) was used for the simulator.
- [Gym](https://www.gymlibrary.dev/) was used for the reinforcment learning API.
- A custom trained [YOLOv5](https://github.com/ultralytics/yolov5) model was used for object detection.
- A modified version of the [Edinburgh University Formula Student (EUFS)](https://gitlab.com/eufs/eufs_sim) track generator was used to randomise the environment for training.
- A deep deterministic policy gradient (DDPG) algorithim was used as the control network.

## Final Video

{{< youtube YQ0deGengaM >}}
