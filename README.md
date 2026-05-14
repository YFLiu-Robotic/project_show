# Project_Show

本仓库用于展示个人简历中的代表性项目材料，内容覆盖机器人数据处理、仿真数据增强、强化学习、VLA 模型后训练与真机部署，以及有限元仿真、力学分析和建筑结构方向研究成果。

仓库材料主要包括：

- 项目展示视频：用于快速查看数据处理、仿真、策略回放、推理和真机部署效果。
- 项目报告与展示 PDF：用于说明项目背景、技术路线、实验结果和阶段性成果。
- 已发表论文：用于展示力学与建筑结构方向的研究成果。

> 本仓库材料仅用于个人项目展示，请勿未经许可转载、商用或二次分发。

## 内容概览

| 序号 | 方向 | 主要内容 | 材料类型 |
| --- | --- | --- | --- |
| 1 | MANO / Mocap 数据处理 | 手部模型可视化、Mocap 数据处理、轨迹重定向 | 视频 |
| 2 | 仿真数据增强 | 仿真场景中的观测和数据增强效果 | 视频 |
| 3 | 强化学习轨迹重定向 | Mano 轨迹重定向到机械臂夹爪 | 视频 |
| 4 | VLA 后训练与真机部署 | SO101 / UR5 机械臂后训练、观测生成、推理和部署 | 视频、报告 |
| 5 | 机械建筑领域研究 | 有限元仿真、力学理论分析、3D 打印试验 | 展示 PDF |
| 6 | 发表论文 | 力学与建筑结构方向论文 | 论文 PDF |
| 7 | Isaac Gym 强化学习复现 | Franka 机械臂抓取与堆叠任务复现 | 视频、报告 |

## 项目材料

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

该部分展示基于强化学习策略将 Mano 轨迹重定向到机械臂夹爪的结果。

- [policy_replay.webm](<3. 基于强化学习的 Mano 轨迹重定向/policy_replay.webm>)

### 4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署

该部分展示 VLA 模型后训练、观测生成、推理和真机部署效果，并包含 SO101 机械臂抓取任务相关报告。

- [基于 cosmos-transfer 生成新的观测.mp4](<4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署/cosmos-transfer_dataset/基于cosmos-transfer生成新的观测.mp4>)
- [pick_the_white_box.mp4](<4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署/Inference/pick_the_white_box.mp4>)
- [Fine-Tuning and Testing of Grasping Tasks Based on pi0.5 Foundation Model for SO101 6-DOF Robot Arm.pdf](<4. 基于 pi0.5VLA 模型的 SO101 机械臂和 UR5 机械臂后训练和真机部署/report/Fine-Tuning and Testing of Grasping Tasks Based on π0.5 Foundation Model for SO101 6-DOF Robot Arm.pdf>)

### 5. 机械建筑领域研究

该部分展示机械建筑方向的有限元仿真、力学理论分析和 3D 打印试验成果。

- [项目展示-新型机械超材料阻尼器设计和试验.pdf](<5. 机械建筑领域研究(有限元仿真_力学理论_3D打印)/新型机械超材料阻尼器设计和试验/项目展示-新型机械超材料阻尼器设计和试验.pdf>)

### 6. 发表论文

该部分收录力学与建筑结构方向的已发表论文。

- [1. Resistance and embedment depth of embedded rectangular concrete-filled.pdf](<6. 发表的论文/1. Resistance and embedment depth of embedded rectangular concrete-filled.pdf>)
- [2. Behavior of Novel Beam-strengthened Embedded CFST Column Bases under Cyclic Loading-Experimental Study and Resistance Prediction.pdf](<6. 发表的论文/2. Behavior of Novel Beam-strengthened Embedded CFST Column Bases under Cyclic Loading-Experimental Study and Resistance Prediction.pdf>)
- [3. Elastic Local Buckling of I-Sections under Axial Compression.pdf](<6. 发表的论文/3. Elastic Local Buckling of I-Sections under Axial Compression.pdf>)

### 7. 基于 Isaac Gym 的机械臂抓取强化学习项目复现

该部分展示 Franka Emika Panda 机械臂在 Isaac Gym 中完成立方体抓取与堆叠任务的训练效果，并包含项目展示和报告材料。

- [训练结果演示视频.mp4](<7. 其他/基于Isaac_gym的机械臂抓取强化学习项目复现/训练结果演示视频.mp4>)
- [项目展示.pdf](<7. 其他/基于Isaac_gym的机械臂抓取强化学习项目复现/项目展示.pdf>)
- [项目报告.pdf](<7. 其他/基于Isaac_gym的机械臂抓取强化学习项目复现/项目报告.pdf>)

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
│   ├── Inference/
│   │   └── pick_the_white_box.mp4
│   └── report/
│       └── Fine-Tuning and Testing of Grasping Tasks Based on π0.5 Foundation Model for SO101 6-DOF Robot Arm.pdf
├── 5. 机械建筑领域研究(有限元仿真_力学理论_3D打印)/
│   └── 新型机械超材料阻尼器设计和试验/
│       └── 项目展示-新型机械超材料阻尼器设计和试验.pdf
├── 6. 发表的论文/
│   ├── 1. Resistance and embedment depth of embedded rectangular concrete-filled.pdf
│   ├── 2. Behavior of Novel Beam-strengthened Embedded CFST Column Bases under Cyclic Loading-Experimental Study and Resistance Prediction.pdf
│   └── 3. Elastic Local Buckling of I-Sections under Axial Compression.pdf
└── 7. 其他/
    └── 基于Isaac_gym的机械臂抓取强化学习项目复现/
        ├── 训练结果演示视频.mp4
        ├── 项目展示.pdf
        └── 项目报告.pdf
```

## 查看说明

- 视频文件可在 GitHub 页面中预览；不同浏览器对 `.mp4`、`.mov`、`.webm` 的支持可能不同。
- PDF 文件可直接在 GitHub 页面中打开查看。
