Allegro Gripper Linux Project
==========================
Note: This project works only for PEAK System CAN interface (chardev) for USB: PCAN-USB

Git Repo
========
https://github.com/wonikrobotics/allegro_gripper_linux


Build and Run: "grasp"
======================

1. Download, build, and install PCAN-USB driver for Linux: libpcan

tar -xzvf peak-linux-driver-x.x.tar.gz
cd peak-linux-driver-x.x
make NET=NO
sudo make install

2. Download, build, and install PCAN-Basic API for Linux: libpcanbasic

tar -xzvf PCAN_Basic_Linux-x.x.x.tar.gz
cd PCAN_Basic_Linux-x.x.x/pcanbasic
make
sudo make install

3. Download, build, and install Grasping Library for Linux, "libBGrip": Grasping_Library_for_Linux

4. Build Allegro Gripper Project using cmake "out of source build" style.

unzip AllegroGriper.zip
cd AllegroGripper
mkdir build
cd build
cmake ..
make
make install

Note: Using cmake "out of source build" style, the entire build tree is created under "build" directory so that you can delete "build" directory without worrying about the sources.

5. Connect PCAN-USB and Allegro Hand (make sure to power off Allegro Gripper)

6. Power on Allegro Gripper.

7. Start the grasping program: "grasp"

bin/grasp

8. Use keyboard command to move Allegro Gripper!!!!

If you have any questions, feel free to ask.

Contact Information
======================

info@wonikrobotics.com
