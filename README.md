# isaacsim_grc26

## set isaacsim path
```
export isaac_sim_package_path=<path>/isaacsim-5.1.0
```

## run

- source `ros jazzy`
- build package and source workspace
- launch sim via:
  ```
  ros2 launch isaacsim_grc26 sim.launch.py
  ```

# test

```
ros2 topic pub -r 30 /kinova1/joint_command sensor_msgs/msg/JointState \
"{name: ['kinova1_joint_1'], position: [0.5]}"
```
