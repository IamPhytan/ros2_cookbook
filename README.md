# ROS2 Cookbook

 * Client Libraries
   * rclcpp [API](http://docs.ros2.org/latest/api/rclcpp/)
     * [Logging](rclcpp/logging.md)
     * [Nodes and Components](rclcpp/nodes.md)
     * [Parameters](rclcpp/parameters.md)
     * [Point Clouds](rclcpp/pcl.md)
     * [Time](rclcpp/time.md)
     * [TF2](rclcpp/tf2.md)
     * [Workarounds](rclcpp/workarounds.md)
   * rclpy [API](http://docs.ros2.org/latest/api/rclpy/)
     * [Nodes](rclpy/nodes.md)
     * [Parameters](rclpy/parameters.md)
     * [Time](rclpy/time.md)
     * [TF2](rclpy/tf2.md)
 * [ros2launch](pages/launch.md)
 * [Networking (DDS & CycloneDDS)](pages/networking.md)
 * Command Line Tools
   * ```ros2 run <pkg> <node>```
   * ```ros2 node list```
   * ```ros2 topic list```
   * ```ros2 topic info <topic_name> --verbose``` gives details about QoS.
   * ```ros2 param list```
   * [colcon](pages/colcon.md) is the build tool.
   * ```ros2 doctor --report``` gives tons of information.
* [CMake](pages/cmake.md)
* Bag Files:
   * ```ros2 bag record /topic1 /topic2```
   * Playback:
      * ```ros2 run rviz2 rviz2 --ros-args -p use_sim_time:=true```
      * ```ros2 bag play <bagfile>```
* Packaging
   * [Setting bloom/git to always use ssh](https://answers.ros.org/question/234494/diagnosing-issues-with-bloom-github-two-factor-authentication/)
     * ```git config --global url.ssh://git@github.com/.insteadOf https://github.com/```
   * ```rosdep install --from-paths src --ignore-src --rosdistro=humble -y```
* [Package Documentation](pages/packages.md)
* Status Pages
  * [Rolling Debian Build Status](http://repo.ros2.org/status_page/ros_rolling_default.html)
  * [Iron Debian Build Status](http://repo.ros2.org/status_page/ros_iron_default.html)
  * [Humble Debian Build Status](http://repo.ros2.org/status_page/ros_humble_default.html) 

## License

<a rel="license" href="http://creativecommons.org/publicdomain/zero/1.0/">
  <img src="http://i.creativecommons.org/p/zero/1.0/88x31.png" style="border-style: none;" alt="CC0" />
</a>

The contents of this cookbook are placed in the Public Domain through the CC0 license.
You can use code snippets in your code without attribution and without impact to your
license choice. This cookbook is provided as-is and without any warranties of any kind.
See the full text of the
[CC0 license](https://creativecommons.org/publicdomain/zero/1.0/legalcode).

While not required by license, if you want to copy the entire cookbook somewhere, please
give some attribution.
