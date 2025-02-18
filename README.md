# TJU_IMU_DS

This is a smartphone IMU dataset collected by the Advanced Network Laboratory of Tianjin University. 

## Introduction
It contains IMU data collected by multiple smartphones in the outdoor environment of Tianjin University, including accelerometer, gyroscope and magnetometer data. 
In addition, the dataset also includes the location information collected synchronously by the satellite positioning chip of the mobile phone and the professional satellite positioning terminal device RTKLite.
Among them, the positioning accuracy of the mobile phone satellite positioning chip is 10 meters, and the accuracy of RTKLite is centimeter level.
Therefore, the location information of the mobile phone satellite positioning chip is used as a noisy marker for IMU inertial tracking, and RTKLite provides a true value marker.

## Hardware

- Smartphones: 
- [RTKLite](https://www.qxwz.com/products/litertk2)

## Software

- [AndroidGnssLogger](https://play.google.com/store/apps/details?id=com.google.android.apps.location.gps.gnsslogger): Collect IMU and location data.

## Data Collection
During the experiment, users walked freely in the outdoor environment of the campus to simulate daily walking behavior. Each user held a smartphone and a professional GNSS receiver LiteRTK to synchronously collect IMU data and high-precision position information. This synchronous collection method provides accurate ground truth for evaluating pedestrian trajectory tracking algorithms. The time length of each IMU segment is 1 second and the sampling frequency is 100Hz, so each data segment (sample) contains 100 IMU readings. The GNSS position sequence is recorded at a sampling frequency of 1Hz through Android's location service API.

## Data Format

- IMU data: H5 file, including accelerometer, gyroscope and magnetometer data.
- Info data: yaml file, including extra information.

## Data Description
TODO

## Download

You can download the data from the following link: [TJU_IMU_DS](https://drive.google.com/file/d/1sFQ2tn3P3tF2SfuA1Vkcy_ofJf8QZw3c/view?usp=sharing)

If this link is not available, please contact the author(jiankunwang@tju.edu.cn) for further assistance.

## Usage
TODO

## Citation
Yuefan Tong, Jiankun Wang, Zenghua Zhao, Jiayang Cui, Bin Wu, Noisy Labels Make Sense: Data-Driven Smartphone Inertial Tracking without Tedious Annotations, the 25th IEEE International Symposium on a World of Wireless, Mobile and Multimedia Networks (WoWMoM’2024), Perth, Western Australia, Jun. 04-07 2024.