# Goal-Driven Deep RL Policy for Robot Navigation
Deep Reinforcement Learning for mobile robot navigation in ROS2 Gazebo simulator. Using Twin Delayed Deep Deterministic Policy Gradient (TD3) neural network, a robot learns to navigate to a random goal point in a simulated environment while avoiding obstacles. Trained in ROS2 Humble & Gazebo simulator with PyTorch.

# How To Run

Install Python 3.10, ROS2 Humble, Gazebo 11 on Ubuntu 22.04
```
git clone git@github.com:lehoangan2906/Autonomous-Navigation-for-robot-using-TD3.git
cd Autonomous-Navigation-for-robot-using-TD3/DRL_robot_navigation_ros2
sudo rosdep init
rosdep install --from-paths src --ignore-src -y
colcon build
cd ..
```

For Training - 
```
ros2 launch td3 train_simulation.launch.py
```

For Testing - 
```
ros2 launch td3 test_simulation.launch.py
```
