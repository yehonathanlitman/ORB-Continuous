This is some experimental code based on LearnVIORB which encompasses continuous preintegration instead of the traditional preintegration model, as well as some other modifications. Inspiration was taken from the original VIO paper with ORB-SLAM and RK4 preintegration (see ORB-VINS_RK4), but it's still very experimental and not bug free. In my experience it works on Ubuntu 16.04, but ONLY for new installations. If you have been using 16.04 for a while chances are it won't work, but if you try it in Virtual Box you should have luck (somehow). More changes to come.

******
**LearnVIORB README**
Not bug-free. Not real-time. Just try the basic ideas of Visual Inertial SLAM in above paper. Welcome to improve it together!

Please run "echo "export ROS_PACKAGE_PATH=${ROS_PACKAGE_PATH}:{your_path_here}/ORB-Continuous/Examples/ROS/PINK_ORB" >> ~/.bashrc; source ~/.bashrc".
build with `build.sh`. Modify the data path in `config/euroc.yaml`. 
Then you can run "roslaunch Examples/ROS/ORB_VIO/launch/euroc.launch" to experience this code.


Tested on [EuRoc](http://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets) ROS bag data with ROS launch file `Examples/ROS/ORB_VIO/launch/testeuroc.launch`. Files in `pyplotscripts` can be used to visualize some results.

Tested on sensors: [UI-1221-LE](https://en.ids-imaging.com/store/ui-1221le.html) and [3DM-GX3-25](http://www.microstrain.com/inertial/3dm-gx3-25), see video on [Youtube (real-time)](https://youtu.be/AUWBpSj-XtA) or [YouKu](http://v.youku.com/v_show/id_XMTkxMjgzMzMwOA).
