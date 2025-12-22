🏎️ Autonomous Line Follower using Deep Reinforcement Learning
A custom simulation environment where an AI agent learns to navigate complex, randomly generated "Zig-Zag" tracks using Deep Reinforcement Learning. Unlike traditional PID controllers, this agent learns continuous control for both steering and velocity from scratch.

🚀 Key Features

Self-Learning AI: The robot learns to slow down for sharp corners and accelerate on straights without hard-coded rules.

Custom Gymnasium Environment: Built from scratch to simulate vehicle physics and sensor dynamics.

Dynamic Track Generation: Creates unique, high-frequency zig-zag paths every episode to ensure robust learning.

Realistic Perception: Simulates an array of 5 IR sensors for line detection.

🛠️ Tech Stack
Python (Core Logic)

Gymnasium (Custom Environment)

Stable-Baselines3 (PPO Algorithm)

NumPy (Vector Math & Physics)

Matplotlib (Visualization & Rendering)

🧠 How It Works
Observation: The agent sees 5 sensor readings + its current speed.

Action: It outputs continuous commands for Velocity and Steering Angle.

Reward System:

Positive: For high speed while centered on the line.

Negative: For drifting off-center or moving too slow.

Termination: Episode ends if the robot strays too far from the track
