FROM introlab3it/rtabmap_ros:melodic

RUN apt-get update && apt-get install bash-completion wget terminator git vim nautilus -y

# install ros package
RUN apt-get update && apt-get install -y \
      ros-${ROS_DISTRO}-freenect-launch \
      ros-${ROS_DISTRO}-rqt* && \
    rm -rf /var/lib/apt/lists/*

# launch ros package
#CMD ["ros2", "launch", "demo_nodes_cpp", "talker_listener.launch.py"]
CMD ["bash"]
