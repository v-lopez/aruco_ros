^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package aruco_ros
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1.0.0 (2018-02-08)
------------------
* Update readme for new coordinates
* Fix orientation changes in aruco 3.0.0
* Migration to aruco 3.0.4
* Merge branch 'indigo-devel' into kinetic-devel
* Merge pull request `#41 <https://github.com/pal-robotics/aruco_ros/issues/41>`_ from Voidminded/kinetic-devel
  Fixed OpenCV Calib3D link error on ROS Kinetic
* Fixed OpenCV Calib3D link error on ROS Kinetic
* Merge pull request `#36 <https://github.com/pal-robotics/aruco_ros/issues/36>`_ from pal-robotics/add-aruco-ros-utils
  Add aruco_ros_utils lib and fix some missing dependencies
* Add aruco_ros_utils lib and fix some missing dependencies
* Merge pull request `#35 <https://github.com/pal-robotics/aruco_ros/issues/35>`_ from ugnelis/kinetic-devel
  Removed duplicated line.
* Removed duplicated line.
* Merge pull request `#27 <https://github.com/pal-robotics/aruco_ros/issues/27>`_ from cehberlin/assert_fix
  Replace assert by error message to keep library functional
* Improved camera_frame\_ assert and removed unecessary opencv includes
* Replace assert by error message to keep library functional
* Contributors: Bence Magyar, Christopher Hrabia, Jordi Pages, Ugnius Malūkas, Victor Lopez, Voidminded

0.2.2 (2017-07-25)
------------------
* only look for aruco if someone is looking for them
* Contributors: Victor Lopez

0.2.1 (2017-07-21)
------------------
* Change default threshold to match defaults of aruco marker detector
* Add dynamic reconfigure to simple_single
* Contributors: Victor Lopez

0.2.0 (2016-10-19)
------------------
* only proccesses images if there are subscribers
* add rviz marker and add corner param
* use double precision to improve accuracy
* Contributors: Jordi Pages, Procópio Stein

0.1.0 (2015-08-10)
------------------
* Update changelogs and maintainer email
* Frame parameters only checked when using camera info
* Add marker list publisher
* Remove unused broadcaster
* Only do 3d when there is camera info
* Use waitForMessage for camerainfo
* Remove nonsense assert
* Reorganize and allow no camera_info
* Fix crash when distortion vector is 0 long (usb_cam)
* Contributors: Bence Magyar

0.0.1 (2015-05-20)
------------------
* More accurate ROS timestamps (callback triggering time)
  This commit ensures that:
  - all published msgs in a callback have the same timestamp
  - the time is as close as possible to the frame grabbing time (as fast as the marker detection may be, the delay might affect TF interpolation in an unacceptable way for applications like visual servoing)
* Install marker_publisher executable
  This target was missing in the installation rule
* Finished some renaming
* changes to finish branch merge
* aruco_ros: Fixing superfluous (and broken) linker arg to -laruco
* Reorganize aruco_ros into 3 packages
* Contributors: Bence Magyar, Jordi Pages, Josh Langsfeld, ObiWan, Steve Vozar
