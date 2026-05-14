# Project_Show

如果要使用或借鉴本仓库内容，烦请 Star 或 Fork。

本仓库目前仅用于展示项目视频，内容覆盖 MANO/Mocap 数据处理、仿真数据增强、强化学习轨迹重定向、VLA 模型后训练与真机部署，以及 Isaac Gym 机械臂抓取强化学习复现。仓库不在 README 中展开论文、报告、代码、模型权重或原始数据。

> 视频材料仅用于个人项目展示，请勿未经许可转载、商用或二次分发。

## 视频索引

| 序号 | 方向 | 视频数量 | 视频目录 |
| --- | --- | ---: | --- |
| 1 | MANO / Mocap 数据处理管线 | 4 | [1. MANO和Mocap数据处理管线展示](<1. MANO和Mocap数据处理管线展示>) |
| 2 | 仿真数据增强 | 5 | [2. 仿真-数据增强展示](<2. 仿真-数据增强展示>) |
| 3 | 基于强化学习的 Mano 轨迹重定向 | 1 | [3. 基于强化学习的 Mano 轨迹重定向](<3. 基于强化学习的 Mano 轨迹重定向>) |
| 4 | pi0.5VLA 后训练与真机部署 | 2 | [4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署](<4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署>) |
| 5 | Isaac Gym 机械臂抓取强化学习复现 | 1 | [7. 其他/基于Isaac_gym的机械臂抓取强化学习项目复现](<7. 其他/基于Isaac_gym的机械臂抓取强化学习项目复现>) |

## 目录结构

```text
Project_Show/
├── 1. MANO和Mocap数据处理管线展示/
│   ├── mano_egodex_visualization.mp4
│   ├── mocap_example_1.mp4
│   ├── mocap_example_2.mp4
│   └── Retargeting_example.mov
├── 2. 仿真-数据增强展示/
│   ├── example_1.mp4
│   ├── example_2.mp4
│   ├── example_3.mp4
│   ├── example_4.mp4
│   └── example_5.mp4
├── 3. 基于强化学习的 Mano 轨迹重定向/
│   └── policy_replay.webm
├── 4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署/
│   ├── cosmos-transfer_dataset/
│   │   └── 基于cosmos-transfer生成新的观测.mp4
│   └── Inference/
│       └── pick_the_white_box.mp4
└── 7. 其他/
    └── 基于Isaac_gym的机械臂抓取强化学习项目复现/
        └── 训练结果演示视频.mp4
```

## 视频列表

### 1. MANO 和 Mocap 数据处理管线展示

该部分展示 MANO 手部模型、Mocap 数据处理、可视化和重定向效果。

- [mano_egodex_visualization.mp4](<1. MANO和Mocap数据处理管线展示/mano_egodex_visualization.mp4>)
- [mocap_example_1.mp4](<1. MANO和Mocap数据处理管线展示/mocap_example_1.mp4>)
- [mocap_example_2.mp4](<1. MANO和Mocap数据处理管线展示/mocap_example_2.mp4>)
- [Retargeting_example.mov](<1. MANO和Mocap数据处理管线展示/Retargeting_example.mov>)

### 2. 仿真-数据增强展示

该部分展示仿真场景中的数据增强效果。

- [example_1.mp4](<2. 仿真-数据增强展示/example_1.mp4>)
- [example_2.mp4](<2. 仿真-数据增强展示/example_2.mp4>)
- [example_3.mp4](<2. 仿真-数据增强展示/example_3.mp4>)
- [example_4.mp4](<2. 仿真-数据增强展示/example_4.mp4>)
- [example_5.mp4](<2. 仿真-数据增强展示/example_5.mp4>)

### 3. 基于强化学习的 Mano 轨迹重定向

该部分展示基于强化学习策略的 Mano 轨迹重定向结果。

- [policy_replay.webm](<3. 基于强化学习的 Mano 轨迹重定向/policy_replay.webm>)

### 4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署

该部分展示 VLA 模型后训练、观测生成、推理和真机部署效果。

- [基于 cosmos-transfer 生成新的观测.mp4](<4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署/cosmos-transfer_dataset/基于cosmos-transfer生成新的观测.mp4>)
- [pick_the_white_box.mp4](<4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署/Inference/pick_the_white_box.mp4>)

### 5. 基于 Isaac Gym 的机械臂抓取强化学习项目复现

该部分展示 Franka Emika Panda 机械臂在 Isaac Gym 中完成立方体抓取与堆叠任务的训练效果。

- [训练结果演示视频.mp4](<7. 其他/基于Isaac_gym的机械臂抓取强化学习项目复现/训练结果演示视频.mp4>)

## 查看说明

- 点击上方视频链接可在 GitHub 页面中查看对应展示材料。
- `.mp4`、`.mov`、`.webm` 的在线预览效果取决于 GitHub 和浏览器对对应格式的支持。
