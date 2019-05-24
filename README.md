# Notes_temp

uzh_ptam的第一个bug：
https://answers.ros.org/question/263951/fatal-error-rqt_gui_cpppluginh-no-such-file-or-directory/

# svo ros 
%rosnode list
/play_1558685483645224418
/rosout
/rqt_gui_py_node_21622
/rviz_1558685443760227893
/svo


%rosnode info /rosout 
--------------------------------------------------------------------------------
Node [/rosout]
Publications: 
 * /rosout_agg [rosgraph_msgs/Log]

Subscriptions: 
 * /rosout [rosgraph_msgs/Log]

Services: 
 * /rosout/get_loggers
 * /rosout/set_logger_level


contacting node http://wd-YangTianM4000e-04:35203/ ...
Pid: 20644
Connections:
 * topic: /rosout
    * to: /rviz_1558685443760227893 (http://wd-YangTianM4000e-04:40981/)
    * direction: inbound
    * transport: TCPROS
 * topic: /rosout
    * to: /svo (http://wd-YangTianM4000e-04:43913/)
    * direction: inbound
    * transport: TCPROS
 * topic: /rosout
    * to: /play_1558685483645224418 (http://wd-YangTianM4000e-04:46257/)
    * direction: inbound
    * transport: TCPROS
 * topic: /rosout
    * to: /rqt_gui_py_node_21622 (http://wd-YangTianM4000e-04:42507/)
    * direction: inbound
    * transport: TCPROS

[wd@wd-YangTianM4000e-04]~/monocular/catkin_ws
%rosnode info /svo 
--------------------------------------------------------------------------------
Node [/svo]
Publications: 
 * /rosout [rosgraph_msgs/Log]
 * /svo/dense_input [svo_msgs/DenseInput]
 * /svo/image [sensor_msgs/Image]
 * /svo/image/compressed [sensor_msgs/CompressedImage]
 * /svo/image/compressed/parameter_descriptions [dynamic_reconfigure/ConfigDescription]
 * /svo/image/compressed/parameter_updates [dynamic_reconfigure/Config]
 * /svo/image/compressedDepth [sensor_msgs/CompressedImage]
 * /svo/image/compressedDepth/parameter_descriptions [dynamic_reconfigure/ConfigDescription]
 * /svo/image/compressedDepth/parameter_updates [dynamic_reconfigure/Config]
 * /svo/image/theora [theora_image_transport/Packet]
 * /svo/image/theora/parameter_descriptions [dynamic_reconfigure/ConfigDescription]
 * /svo/image/theora/parameter_updates [dynamic_reconfigure/Config]
 * /svo/info [svo_msgs/Info]
 * /svo/keyframes [visualization_msgs/Marker]
 * /svo/points [visualization_msgs/Marker]
 * /svo/pose [geometry_msgs/PoseWithCovarianceStamped]
 * /tf [tf2_msgs/TFMessage]

Subscriptions: 
 * /camera/image_raw [sensor_msgs/Image]
 * /svo/remote_key [std_msgs/String]

Services: 
 * /svo/get_loggers
 * /svo/image/compressed/set_parameters
 * /svo/image/compressedDepth/set_parameters
 * /svo/image/theora/set_parameters
 * /svo/set_logger_level


contacting node http://wd-YangTianM4000e-04:43913/ ...
Pid: 21445
Connections:
 * topic: /rosout
    * to: /rosout
    * direction: outbound
    * transport: TCPROS
 * topic: /tf
    * to: /rviz_1558685443760227893
    * direction: outbound
    * transport: TCPROS
 * topic: /svo/keyframes
    * to: /rviz_1558685443760227893
    * direction: outbound
    * transport: TCPROS
 * topic: /svo/points
    * to: /rviz_1558685443760227893
    * direction: outbound
    * transport: TCPROS
 * topic: /svo/info
    * to: /rqt_gui_py_node_21622
    * direction: outbound
    * transport: TCPROS
 * topic: /svo/image
    * to: /rviz_1558685443760227893
    * direction: outbound
    * transport: TCPROS
 * topic: /camera/image_raw
    * to: /play_1558685483645224418 (http://wd-YangTianM4000e-04:46257/)
    * direction: inbound
    * transport: TCPROS
 * topic: /svo/remote_key
    * to: /rqt_gui_py_node_21622 (http://wd-YangTianM4000e-04:42507/)
    * direction: inbound
    * transport: TCPROS

[wd@wd-YangTianM4000e-04]~/monocular/catkin_ws
%rosnode info /rviz_1558685443760227893 
--------------------------------------------------------------------------------
Node [/rviz_1558685443760227893]
Publications: 
 * /clicked_point [geometry_msgs/PointStamped]
 * /initialpose [geometry_msgs/PoseWithCovarianceStamped]
 * /move_base_simple/goal [geometry_msgs/PoseStamped]
 * /rosout [rosgraph_msgs/Log]

Subscriptions: 
 * /svo/image [sensor_msgs/Image]
 * /svo/keyframes [visualization_msgs/Marker]
 * /svo/keyframes_array [unknown type]
 * /svo/points [visualization_msgs/Marker]
 * /svo/points_array [unknown type]
 * /tf [tf2_msgs/TFMessage]
 * /tf_static [unknown type]

Services: 
 * /rviz_1558685443760227893/get_loggers
 * /rviz_1558685443760227893/reload_shaders
 * /rviz_1558685443760227893/set_logger_level


contacting node http://wd-YangTianM4000e-04:40981/ ...
Pid: 21147
Connections:
 * topic: /rosout
    * to: /rosout
    * direction: outbound
    * transport: TCPROS
 * topic: /tf
    * to: /svo (http://wd-YangTianM4000e-04:43913/)
    * direction: inbound
    * transport: TCPROS
 * topic: /svo/keyframes
    * to: /svo (http://wd-YangTianM4000e-04:43913/)
    * direction: inbound
    * transport: TCPROS
 * topic: /svo/points
    * to: /svo (http://wd-YangTianM4000e-04:43913/)
    * direction: inbound
    * transport: TCPROS
 * topic: /svo/image
    * to: /svo (http://wd-YangTianM4000e-04:43913/)
    * direction: inbound
    * transport: TCPROS






rostopic list
/Rig
/camera/camera_info
/camera/image_raw
/clicked_point
/clock
/imu/data
/imu/magnetometer
/initialpose
/move_base_simple/goal
/rosout
/rosout_agg
/statistics
/svo/dense_input
/svo/image
/svo/image/compressed
/svo/image/compressed/parameter_descriptions
/svo/image/compressed/parameter_updates
/svo/image/compressedDepth
/svo/image/compressedDepth/parameter_descriptions
/svo/image/compressedDepth/parameter_updates
/svo/image/theora
/svo/image/theora/parameter_descriptions
/svo/image/theora/parameter_updates
/svo/info
/svo/keyframes
/svo/keyframes_array
/svo/points
/svo/points_array
/svo/pose
/svo/remote_key
/tf
/tf_static
[wd@wd-YangTianM4000e-04]~/monocular/catkin_ws
%rostopic hz /svo/pose 
subscribed to [/svo/pose]
average rate: 30.255
	min: 0.026s max: 0.036s std dev: 0.00235s window: 29
average rate: 30.103
	min: 0.018s max: 0.050s std dev: 0.00382s window: 59
average rate: 30.076
	min: 0.018s max: 0.050s std dev: 0.00329s window: 89
average rate: 30.046
	min: 0.018s max: 0.050s std dev: 0.00301s window: 119
average rate: 30.066
	min: 0.017s max: 0.050s std dev: 0.00349s window: 143
no new messages
no new messages
no new messages
no new messages
^Cno new messages
[wd@wd-YangTianM4000e-04]~/monocular/catkin_ws
%rostopic type /svo/pose
geometry_msgs/PoseWithCovarianceStamped
[wd@wd-YangTianM4000e-04]~/monocular/catkin_ws
%rosmsg show geometry_msgs/PoseWithCovariance
geometry_msgs/Pose pose
  geometry_msgs/Point position
    float64 x
    float64 y
    float64 z
  geometry_msgs/Quaternion orientation
    float64 x
    float64 y
    float64 z
    float64 w
float64[36] covariance

[wd@wd-YangTianM4000e-04]~/monocular/catkin_ws
%rosmsg show geometry_msgs/PoseWithCovariance
geometry_msgs/Pose pose
  geometry_msgs/Point position
    float64 x
    float64 y
    float64 z
  geometry_msgs/Quaternion orientation
    float64 x
    float64 y
    float64 z
    float64 w
float64[36] covariance

[wd@wd-YangTianM4000e-04]~/monocular/catkin_ws
%rosservice list
/play_1558685970725192550/get_loggers
/play_1558685970725192550/pause_playback
/play_1558685970725192550/set_logger_level
/rosout/get_loggers
/rosout/set_logger_level
/rqt_gui_py_node_21777/get_loggers
/rqt_gui_py_node_21777/set_logger_level
/rqt_gui_py_node_21927/get_loggers
/rqt_gui_py_node_21927/set_logger_level
/rviz_1558685443760227893/get_loggers
/rviz_1558685443760227893/reload_shaders
/rviz_1558685443760227893/set_logger_level
/svo/get_loggers
/svo/image/compressed/set_parameters
/svo/image/compressedDepth/set_parameters
/svo/image/theora/set_parameters
/svo/set_logger_level



