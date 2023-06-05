# GPT4_ROS2 Mini Pupper Launch Package

This code package is used to launch the related nodes for the GPT4_ROS2 Mini Pupper Robot. This will run within the Robot Operating System 2 (ROS2) framework.

## Function Description

This launch file contains the following functionality:

1. Start the robot's parameter server (GPT4_ROS2 parameter server)
2. Start the robot's GPT4_ROS2 service
3. Start the audio output node
4. Start the audio input node
5. Start the robot control node

Running this launch file will enable the robot to:

- Listen and understand external language commands
- Execute external language commands
- Receive and transmit audio signals

## How to Use

1. Make sure you have ROS2 installed and have set up the environment.
2. Save this code as a file named `mini_pupper.launch.py`.
3. In a terminal, navigate to the folder containing the above file.
4. Run the following command to start the Mini Pupper robot:

```
ros2 launch mini_pupper.launch.py
```

## Parameter Configuration

The parameters in the code can be changed as needed:

- `mini_pupper`: This parameter is used to determine whether the program runs on Mini Pupper hardware. The default value is `True`. Changing this value will affect the configuration of the parameter server and other nodes.

## Node Descriptions

The following describes each of the nodes included in the launch file:

1. `gpt_param_server`: This is the robot parameter server node, responsible for managing the robot's parameters.

2. `gpt_service`: This node provides the GPT4_ROS2 service, allowing users to control the robot through language commands.

3. `audio_output`: This is the audio output node, used to send audio signals for Mini Pupper to play.

4. `audio_input`: This is the audio input node, used to receive audio signals from Mini Pupper.

5. `gpt_robot`: This is the robot control node, used to execute the actual robot movement and control. 