# 交通灯控制与车道线检测（Simulink + Arduino）

## 文件说明

| 文件 | 功能 |
|------|------|
| `traffic_light_controller.slx` | 基于 Arduino 的交通信号灯状态机，控制人行道与机动车道的红黄绿灯切换 |
| `lane_detection_hough.slx` | 使用 Hough 变换检测视频中的车道线 |

## 运行环境

- MATLAB R2015b 或更高
- Simulink
- Computer Vision System Toolbox
- Image Processing Toolbox
- `traffic_light_controller.slx` 需 Simulink Support Package for Arduino Hardware 及 Arduino 开发板

## 运行说明

1. **车道线检测**：打开 `lane_detection_hough.slx`，在 `From Multimedia File` 模块中重新指向本机视频文件（如 Computer Vision Toolbox 自带的 `viplanedeparture.avi`），点击运行。
2. **交通灯控制**：连接 Arduino 开发板，打开 `traffic_light_controller.slx`，配置 Arduino 支持包后部署/运行，观察红绿灯状态机切换。
