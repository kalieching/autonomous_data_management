Source: https://aws.amazon.com/blogs/robotics/record-store-robot-data-rosbag/

All code files have been modified by the resources provided by the AWS 
Robotics Blog.

In order to set up the nodes, the following commands must be run, 
each in different tabs:
-roslaunch s3_file_uploader s3_file_uploader.launch s3_bucket:=datastoretest
-roslaunch rosbag_cloud_recorders duration_recorder.launch
-python recorder_client.py duration_recorder

Based on this resource: http://library.isr.ist.utl.pt/docs/roswiki/rosbag(2f)Tutorials(2f)Recording(20)and(20)playing(20)back(20)data.html
-Run "rostopic list -v" to examine the currently publishing topics
-Run "rosbag play <your file>" (/home/vboxuser/rosbag_sensor_example.bag)
