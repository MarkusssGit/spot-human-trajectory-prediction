# Human Trajectory Prediction for Boston Dynamics Spot
Aalto University team project with the Boston Dynamics Spot robot on socially compliant robot navigation.

Original team repository: https://github.com/harshaguda/spot-human-trajectory-prediction

## My contribution

I implemented the ROS2 human trajectory-prediction component in Python. An Extended Kalman Filter (EKF) was used to estimate human position and velocity from noisy measurements and predict future motion. The predicted state was then used to generate a "danger zone" representing likely future positions of the tracked person.

My contribution can be found in this directory from the project: https://github.com/harshaguda/spot-human-trajectory-prediction/tree/main/ros2_ws/src/human_trajectory_prediction/human_trajectory_prediction

- `prediction_node.py` - EKF state estimation and trajectory prediction
- `danger_zone_publisher.py` - predicted danger-zone generation
- `listener_node.py` - ROS2 communication for the prediction component
