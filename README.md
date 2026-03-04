# AI-Driven Robotic Sketch Generation using LSTM and MATLAB Kinematics

## Project Description
This project combines **Deep Learning and Robotics** to generate sketches using a trained **LSTM neural network** and reproduce them using a **robotic simulation in MATLAB**.  
The model is trained on the **Google QuickDraw dataset** to learn sketch stroke sequences and predict drawing coordinates. These coordinates are then used in a MATLAB robot simulation where **forward and inverse kinematics** enable the robot to recreate the generated sketches.

---

## Project Overview

The pipeline of the project is:

1. Train an **LSTM-based neural network** on the Google QuickDraw dataset to learn stroke sequences.
2. During inference, the trained model **predicts stroke deltas** `(dx, dy, pen_state)` autoregressively.
3. The predicted deltas are converted into **absolute coordinate trajectories**.
4. These coordinates are passed to a **MATLAB robot simulation**.
5. Using **forward and inverse kinematics**, the simulated robot manipulator reproduces the sketch.

---

## Key Features

- Deep learning based **sketch generation**
- **Sequence modeling using LSTM**
- **Autoregressive sketch prediction**
- Conversion from **stroke deltas to absolute coordinates**
- Integration with **MATLAB robotic simulation**
- Robot motion control using **forward and inverse kinematics**
- Visualization using **animated sketch GIFs**

---

## Dataset

The project uses the **Google QuickDraw Dataset**, which represents drawings as vector strokes rather than images.

Each drawing contains multiple strokes in the form:
