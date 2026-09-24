# 项目展示

香港中文大学（深圳）人工智能与机器人硕士在读，浙江大学结构工程硕士。主要方向：人类Ego视频和第三视角视频处理管线搭建、仿真-数据增强、强化学习预训练-微调-蒸馏-部署、机械臂与五指灵巧手真机部署，人形机器人强化学习和真机部署。

[项目总览（PDF）](<0. 总览.pdf>)

未经授权请勿随意使用当前项目内容

<a id="mano"></a>
## 1. MANO 数据管线展示

项目背景：枢途科技（深圳），2026.01–2026.05，主要参与者。

参与构建第一视角（Ego）数据处理管线，基于 Dyn-HaMeR 与 FoundationPose 完成人手和物体的 4D 位姿重建。设计 MANO 轨迹后处理流程，对缺帧、跳帧及加速度异常进行筛选、检测与优化。参与项目累计交付 1,200+ 小时 Ego 数据。

| 材料 | 链接 |
| --- | --- |
| 家庭场景手部数据 | [观看视频](<1. MANO数据管线展示/家庭.mp4>) |
| 物流场景手部数据 | [观看视频](<1. MANO数据管线展示/物流.mp4>) |
| 衣厂场景手部数据 | [观看视频](<1. MANO数据管线展示/衣厂.mp4>) |

<a id="locomotion"></a>
## 2. Locomotion 数据管线展示

项目背景：枢途科技（深圳），2026.01–2026.05，负责管线设计与搭建。

基于 GVHMR 从互联网视频提取人体三维姿态，设计穿模、浮空和加速度异常检测流程。在 Isaac Gym 中利用 Motion Tracking 修复低质量动作数据，并组织自动化处理流程。参与项目累计交付 400+ 小时 Locomotion 数据。

- [人体运动轨迹提取：示例 1（MP4）](<2. Locomotion数据管线展示/mocap_example_1.mp4>)
- [人体运动轨迹提取：示例 2（MP4）](<2. Locomotion数据管线展示/mocap_example_2.mp4>)
- [基于 Motion-tracking 的轨迹修复（MP4）](<2. Locomotion数据管线展示/PHC.mp4>)

<a id="simulation"></a>
## 3. 仿真-数据增强管线展示

项目背景：枢途科技（深圳），2026.01–2026.05，主要参与者。

参与构建人类视频到机器人仿真数据的 Real-to-Sim 管线，为 VLA 训练提供轨迹和图像观测。

1. 动作重定向：基于 Dex-retargeting，将 MANO 人手数据重定向到二指夹爪。
2. 轨迹增广：对末端执行器施加随机位姿扰动，通过逆运动学（IK）求解生成新的机器人轨迹。
3. 观测增强：在仿真器中回放轨迹，改变光照、材质等条件，并结合 Domain Randomization、Cosmos Transfer 生成多样化观测。

相关开源数据集 HoRA 在 Hugging Face 的累计下载量为 3,000+ 次，统计截至 2026 年 9 月版简历。

### Cosmos Transfer 观测生成

- [Cosmos Transfer 生成新观测（MP4）](<3. 仿真-数据增强管线展示/cosmos-transfer_dataset/基于cosmos-transfer生成新的观测.mp4>)

### Retargeting / Replay

- [人类动作到机器人动作的重定向演示（MOV）](<3. 仿真-数据增强管线展示/retargeting/Retargeting_example.mov>)
- 不同机器人的仿真任务执行示例：[示例 1](<3. 仿真-数据增强管线展示/retargeting/example_1.mp4>) · [示例 2](<3. 仿真-数据增强管线展示/retargeting/example_2.mp4>) · [示例 3](<3. 仿真-数据增强管线展示/retargeting/example_3.mp4>) · [示例 4](<3. 仿真-数据增强管线展示/retargeting/example_4.mp4>) · [示例 5](<3. 仿真-数据增强管线展示/retargeting/example_5.mp4>)

### Data Reinforcement

- [arm_aug.mp4](<3. 仿真-数据增强管线展示/data_reinforcement/arm_aug.mp4>)
- [bg_aug.mp4](<3. 仿真-数据增强管线展示/data_reinforcement/bg_aug.mp4>)
- [grid.mp4](<3. 仿真-数据增强管线展示/data_reinforcement/grid.mp4>)
- [obj_aug_flipmilk.mp4](<3. 仿真-数据增强管线展示/data_reinforcement/obj_aug_flipmilk.mp4>)

<a id="manipulation"></a>
## 4. 强化学习-机械臂 + 灵巧手项目展示

### HandMimicX：从人类 Ego 视频学习灵巧操作

项目背景：未来清研智能科技有限公司（深圳），2026.05–2026.09。共同第一作者，负责强化学习训练与真机部署；论文 ICRA 在投。

参与提出从单条人类 Ego 视频获取灵巧技能的、以物体为中心的强化学习框架，训练 UR5 机械臂与 Wujihand 灵巧手完成抓取及特定任务，并获得空间泛化能力。

- 预训练：利用 YCB-Affordanc 物体与手势数据，在 Isaac Gym 中学习抓取不同物体并到达随机目标位姿。
- 任务微调：基于人类视频中提取的物体 Mesh 和抓取手势，微调预训练策略。
- 策略蒸馏：通过 DAgger 去除特权信息，获得可部署策略。
- 真机执行：利用双目深度相机与 FoundationPose 获取物体实时 6D 位姿，在 UR5 + Wujihand 上部署策略。

| 实验设置 | 简历记录的结果 |
| --- | --- |
| 4,096 个并行仿真环境，30K 步预训练 + 10K 步微调 | 特定任务成功率 85.4% |
| UR5 + Wujihand，8 个真实任务 | 执行成功率 71.3% |

### 项目演示

- [8 个任务的真机演示（MP4）](<4. 强化学习-机械臂+灵巧手项目展示/real-robot-8tasks.mp4>)
- [Umbrella 任务流程演示（MP4）](<4. 强化学习-机械臂+灵巧手项目展示/pipeline_umbrella.mp4>)
- [Eggplant 任务流程演示（MP4）](<4. 强化学习-机械臂+灵巧手项目展示/pipeline_eggplant.mp4>)

<a id="humanoid"></a>
## 5. 人形机器人物流项目展示

项目背景：未来清研智能科技有限公司（深圳），2026.05–2026.09，主要参与者。

基于 PPO 在 Isaac Sim 中训练搭载 BrainCo Hand 五指绳驱手 / Dex3-1 三指手的宇树 G1-D 机器人，抓取传送带上不同尺寸的移动物体并完成分拣。

- 仿真环境与奖励：搭建场景、配置机器人与物体资产、设计动态抓取奖励函数。
- 课程学习与分拣：在移动物体抓取策略基础上，进一步训练抓取后的物体轨迹跟随。

### 项目演示

- [真机演示（MP4）](<5. 人形机器人物流项目展示/真机_去掉前5秒.mp4>)
- [项目演示 1（MP4）](<5. 人形机器人物流项目展示/飞书20260917-120649.mp4>)
- [项目演示 2（MP4）](<5. 人形机器人物流项目展示/飞书20260917-120741.mp4>)

<a id="papers"></a>
## 6. 论文成果

1. HandMimicX（共同第一作者，ICRA 在投）
   研究主题为从人类第一视角视频学习机器人灵巧操作，并通过强化学习训练、策略蒸馏实现真机部署。

2. Behavior of Novel Beam-strengthened Embedded CFST Column Bases under Cyclic Loading: Experimental Study and Strength Prediction （第一作者。Engineering Structures，JCR Q1。）

3. Resistance and embedment depth of embedded rectangular concrete-filled steel tubular column base connection under cyclic loads （第二作者。Structures, 81 (2025), 110257，JCR Q1。）

4. Elastic Local Buckling of I-Sections under Axial Compression Incorporating Web–Flange Interaction （合作作者。Buildings, 2023, 13, 1912。）

<a id="patent"></a>
## 7. 发表的专利

### 一种数据处理方法及相关装置

| 项目 | 证书信息 |
| --- | --- |
| 类型 | 授权发明专利 |
| 发明人 | 刘宇飞 |
| 专利号 | ZL 2026 1 0984799.5 |
| 授权公告号 | CN 122490870 B |
| 专利申请日 | 2026 年 7 月 3 日 |
| 授权公告日 | 2026 年 8 月 28 日 |

[发明专利证书（PDF）](<7. 发表的专利/MP26011291.20260828.发明专利证书.pdf>)

本申请公开了一种数据处理方法及相关装置，包括：获取真实场景环境中目标对象的异常运动数据；确定所述真实场景环境对应的虚拟场景环境和所述目标对象对应的对象仿真模型；基于所述异常运动数据驱动所述对象仿真模型在所述虚拟场景环境中进行仿真运动；在驱动所述对象仿真模型进行所述仿真运动的过程中，基于所述虚拟场景环境关联的动力学仿真参数和所述虚拟场景环境的物理边界的边界参数，对所述对象仿真模型在所述仿真运动的过程中产生的仿真运动数据进行修正，得到所述异常运动数据对应的修正运动数据。本申请基于真实场景环境与虚拟场景环境的对应关系，实现了对异常运动数据的物理约束修正，提高修正运动数据的可用性。

---
