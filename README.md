# mujoco-g1-walk
Unitree G1 Humanoid Robot Reinforcement Learning Locomotion Project

## Project Introduction
Built on the MuJoCo simulation environment, this project adopts the PPO algorithm to realize gait walking training for Unitree G1 biped robot, enabling stable walking with multi-directional velocity tracking.
**Fully supports CPU training, no NVIDIA graphics card required**
No strict hardware limitations. Training can be completed smoothly on ordinary laptops and office computers with extremely low entry barriers.

## Important Notes
Only core source codes are uploaded in this repository, **excluding robot model files**.
Please download the official Unitree G1 MuJoCo model by yourself, and place `scene.xml` under this path: `model/unitree_g1/`

## Start Training
```bash
python ppo_train.py
```

## Test
```bash
python test.py
```

## Main Functions
- Achieve stable bipedal walking for humanoid robot
- Support velocity command tracking including forward, lateral movement and turning
- Built-in joint safety limits and anti-fall posture control
- Automatically save optimal trained models and normalization parameters
- Adopt curriculum training strategy for fast gait convergence

## License
MIT License
Free for learning, modification and personal use.
Any suggestions and feedback are welcome.
