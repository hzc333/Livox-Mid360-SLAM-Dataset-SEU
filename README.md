# Livox-Mid360-SLAM-Dataset-SEU

[中文版 (Chinese)](#中文说明) | [English Version](#english-version)

---

## 中文说明

本项目包含了在东南大学（SEU）四牌楼校区采集的激光雷达（LiDAR）数据集，主要用于测试和验证 SLAM（即时定位与地图构建）算法。

### 🛠️ 采集设备
- **LiDAR**: Livox Mid-360 (固态激光雷达)

### 📍 采集地点与轨迹说明
所有数据均采集于 **东南大学四牌楼校区**。🌟 **重要特性：本数据集中的所有三条采集轨迹均为严格的闭合路径（起点与终点重合），非常适合用于评估 SLAM 算法的累积漂移误差和回环检测能力。**

根据采集路径的不同，共分为以下三个数据包：

1. **`library.bag`**: 环绕东南大学**图书馆**（闭环）。

2. **`water.bag`**: 环绕**涌泉池（喷泉）**及**中大院**（闭环）。

3. **`zhongxin.bag`**: 环绕**中心楼**及**大礼堂**（闭环）。

### 🗂️ 数据集下载
由于 `.bag` 文件体积较大，未直接包含在此 Git 仓库中。请通过以下 Google Drive 链接下载：

- **Google Drive 下载链接**: https://drive.google.com/drive/folders/16j8hF96GPIxzFb8BDEAUs0ePx-XJ1AFe?usp=drive_link
- **文件说明**: 下载后请将上述三个 `.bag` 文件放置在工程根目录下或新建的 `data/` 文件夹中。

### 🚀 使用方法
确保已安装 ROS 环境，然后在终端运行以下命令播放数据：
```bash
rosbag play library.bag
```

---

## English Version

This repository contains a LiDAR dataset collected at the Sipailou Campus of Southeast University (SEU). It is mainly designed for testing and validating SLAM (Simultaneous Localization and Mapping) algorithms.

### 🛠️ Hardware
- **LiDAR**: Livox Mid-360 (Solid-state LiDAR)

### 📍 Locations & Trajectories
All data were collected at the **Sipailou Campus, Southeast University**. 🌟 **Key Feature: All three trajectories in this dataset are strictly closed-loop (the start and end points perfectly overlap), making them highly suitable for evaluating the cumulative drift error and loop closure capabilities of SLAM algorithms.**

The dataset is divided into three `.bag` files based on their trajectories:

1. **`library.bag`**: Around the **Library** (Closed-loop).

2. **`water.bag`**: Around the **Fountain (Yongquan Pool)** and **Zhongda Hall** (Closed-loop).

3. **`zhongxin.bag`**: Around the **Center Building (Zhongxin Lou)** and the **Grand Auditorium** (Closed-loop).

### 🗂️ Dataset Download
Due to the large size of `.bag` files, they are not directly hosted in this Git repository. Please download them via the Google Drive link below:

- **Google Drive Link**: https://drive.google.com/drive/folders/16j8hF96GPIxzFb8BDEAUs0ePx-XJ1AFe?usp=drive_link
- **Instructions**: After downloading, please place the three `.bag` files in the root directory of this repository or inside a `data/` folder.

### 🚀 Usage
Make sure you have the ROS environment installed, then run the following command in your terminal to play the data:
```bash
rosbag play library.bag
```