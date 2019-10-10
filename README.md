# create_point_clouds_with_t265_d400_camera

This repo is based on [tracking-and-depth](https://github.com/IntelRealSense/librealsense/tree/master/examples/tracking-and-depth) from librealsense example.

However, this project will accumulated depth frames into a full point cloud.

# Requirements
- [Point Cloud Library](http://pointclouds.org): used to create point cloud, save to pcd, visualize in realtime and perform down sampling to reduce cloud size.
- OpenCV: used to visualize the RGB frame
- librealsense: works with T265 and D400 camera.

# Steps
- Step 1: Print the provided0 [STL](https://github.com/IntelRealSense/librealsense/blob/master/examples/tracking-and-depth/bracket_t265nd435_external.stl) from the tracking-and-depth repo.
- Step 2: Compile and run
- Step 3: Select the opencv color window. Here are some key command:
    - **d**: Capture the current frame into the point cloud
    - **s**: Save the point cloud. Edit the name variable if you want to change the saved folder. `pcl::io::savePCDFile(name, *point_cloud_ptr)`
    - **q**: Quit.