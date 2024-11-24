# Isaac Sim Unitree Simulation

## Overview
The **Isaac Sim Unitree Simulation** project involves simulating and training **Unitree robots** using **Isaac Sim** developed by NVIDIA. The simulation utilizes the **Proximal Policy Optimization (PPO)** algorithm for tasks such as standing up, walking, and climbing stairs. This project focuses on testing and training robots in dynamic environments, enhancing their robustness for real-world applications.

## Key Features
- **PPO Algorithm**: Implements the PPO reinforcement learning algorithm to train Unitree robots.
- **Simulation in Isaac Sim**: Provides a realistic simulation environment for testing robotic tasks.
- **Dynamic Terrain Adaptation**: Trains robots to adapt to various types of terrain, including flat and rough environments (stairs).
- **Real-Time Feedback**: Enables real-time monitoring and adjustments during simulation.

## Example Tasks
- **Standing From Crouch**: The robot learns to transition from a crouching position to standing.
- **Walking in Flat Environment**: The robot is trained to walk in a flat terrain environment.
- **Walking in Rough/Stair Environment**: The robot is trained to handle rough terrain and navigate stairs.

## Project Setup
This guide will help you set up your environment to use **NVIDIA Isaac Sim** and clone the **NVIDIA Isaac Lab** repository.

### Prerequisites
- Ensure you have **Python 3.6** or later installed.
- Ensure you have **Git** installed.

### Installation

#### Step 1: Install NVIDIA Isaac Sim
1. Download the **NVIDIA Isaac Sim** package from the [NVIDIA Developer website](https://developer.nvidia.com/isaac-sim).
2. Follow the installation instructions provided on the website.

#### Step 2: Clone the NVIDIA Isaac Lab Repository
1. Open a terminal or command prompt.
2. Navigate to the directory where you want to clone the repository.
3. Run the following command to clone the repository:
   ```bash
   git clone https://github.com/isaac-sim/IsaacLab.git
   ```
4. Navigate into the cloned repository:
   ```bash
   cd IsaacLab
   ```

### Workspace Customization for Unitree A1
1. Navigate to the **Wrapper Folder**:
   ```plaintext
   \source\extensions\omni.isaac.lab_tasks\omni\isaac\lab_tasks\manager_based\locomotion\velocity\config\a1
   ```
2. After adding a new wrapper in the configuration folder, you need to initialize the wrapper in:
   ```plaintext
   \manager_based\locomotion\velocity\__init__.py
   ```
3. You can also add new rewards in the **velocity_env_cfg.py** file:
   ```plaintext
   \manager_based\locomotion\velocity\velocity_env_cfg.py
   ```

### Additional Resources
- **[NVIDIA Isaac Sim Documentation](https://developer.nvidia.com/isaac-sim)**: Official documentation for using NVIDIA Isaac Sim.
- **[NVIDIA Isaac Lab Documentation](https://developer.nvidia.com/isaac-sim)**: Guides and references for using NVIDIA Isaac Lab.

## Video Demonstration
[![Isaac Sim Unitree Simulation](https://img.youtube.com/vi/o566fd4ZG74/0.jpg)](https://youtu.be/o566fd4ZG74)

## Team Members
- **Kunlanith Busabong**  
- **Saranya Vichakyotin**  
- **Watcharaphong Chiangthong**
