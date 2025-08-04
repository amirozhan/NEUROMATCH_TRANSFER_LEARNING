# Transfer Learning from Pong to Tennis (Atari) – Neuromatch RL 2023

This repository contains code for a reinforcement learning (RL) project focused on transferring knowledge between two Atari environments: Pong and Tennis. The project was developed as part of Neuromatch Academy's 2023 Reinforcement Learning track.

---

## 🎯 Objective

The goal is to:
1. Train a convolutional neural network (CNN)-based agent to play Pong using the Advantage Actor-Critic (A2C) algorithm.
2. Transfer the learned weights to a new environment (Tennis).
3. Fine-tune or retrain the model in the new environment and assess the effectiveness of transfer learning.

---

## 🕹 Environments

The notebook utilizes the following **Atari Gym environments**:
- `ALE/Pong-v5`
- `ALE/Tennis-v5`

Both are accessed using the `gymnasium` API.

---

## 🧱 Architecture

- **Backbone**: Convolutional neural network (CNN) with optional batch normalization and grayscale preprocessing.
- **Algorithm**: Advantage Actor-Critic (A2C)
- **Training**:
  - Custom training loop with flexible hyperparameters
  - Video recording of gameplay
  - Logs of loss, reward, and performance

---

## 🔁 Workflow

1. Install dependencies (`gymnasium`, `stable-baselines3`, `pyvirtualdisplay`, `pygame`, etc.)
2. Train on `Pong` using selected hyperparameters
3. Save weights and environment interactions
4. Load weights into new model and retrain on `Tennis`
5. Log and visualize results to compare zero-shot performance vs. fine-tuning

---

## 📦 Dependencies

Install via:

```bash
pip install gymnasium[box2d] stable-baselines3[extra] ale-py pyvirtualdisplay pygame rarfile
