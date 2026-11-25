<a id="top"></a>

<p align="center">
  <a href="README.md">English</a> &nbsp; / &nbsp; <strong>简体中文</strong>
</p>

<a href="https://roboparty.com">
  <picture>
    <source media="(max-width: 640px)" srcset="assets/hero-zh-mobile.jpg">
    <img src="assets/hero-zh.jpg" alt="RoboParty RP1 全开源人形机器人。" width="100%">
  </picture>
</a>

<h1 align="center">RP1: An OpenSource Full-Stack Platform for Agentic Humanoids</h1>

<p align="center">
  从机械、电气到固件、控制与学习，全栈开放。<br>
  让每一层都能被理解，让每一次创新都有起点。
</p>

<p align="center">
  <a href="https://roboparty.com"><img src="https://img.shields.io/badge/官网-RoboParty-2563EB?style=flat-square&labelColor=6B7280" alt="官网：RoboParty"></a>
  <a href="https://lab.roboparty.com/"><img src="https://img.shields.io/badge/Lab-RoboParty-2563EB?style=flat-square&labelColor=6B7280" alt="Lab: RoboParty"></a>
  <a href="https://github.com/Roboparty/Party_OS"><img src="https://img.shields.io/badge/GitHub-Party_OS-2563EB?style=flat-square&labelColor=6B7280" alt="GitHub: Party_OS"></a>
</p>

---

## 以开放为起点

**RP1 是 RoboParty 的全开源人形机器人平台：为理解、构建与拓展真实机器人，提供一个共同的研发起点。**

我们将机械与电气设计、关节模组、固件、机器人模型、部署与学习连接为完整的开发体系。你可以深入研究一个子系统，复刻一台机器人，也可以在此基础上探索自己的控制方式与学习流程。

<table width="999">
<thead>
<tr><th align="left" width="333">可查阅的硬件</th><th align="left" width="333">可拓展的软件</th><th align="left" width="333">可探索的智能</th></tr>
</thead>
<tbody>
<tr><td valign="top" width="333">机械 CAD、原理图、PCB 走线、Gerber、BOM 与装配文档。</td><td valign="top" width="333">Linux BSP、通信、设备接口、机器人描述与部署模块。</td><td valign="top" width="333">行走与跑步训练、动作模仿、运动跟踪与行为模型项目。</td></tr>
</tbody>
</table>

<img src="assets/rp1-box-vault-hq.gif" alt="RP1 翻越箱体实拍" width="100%">

<p align="center"><sub>从机器人本体，到真实世界中的每一步。</sub></p>

<a id="architecture"></a>

## 一台机器人，完整的开放体系

<img src="assets/architecture.svg#gh-light-mode-only" alt="RP1 控制架构：输入 / 感知 → 运控基座（运动重定向、运动策略）→ 实时控制（动作解码 · 串联解算，控制 500 Hz）→ 整机执行（ROMOMO 关节模组 · RP-hand 灵巧手），含急停与高频反馈闭环。" width="100%">
<img src="assets/architecture-dark.svg#gh-dark-mode-only" alt="RP1 控制架构：输入 / 感知 → 运控基座（运动重定向、运动策略）→ 实时控制（动作解码 · 串联解算，控制 500 Hz）→ 整机执行（ROMOMO 关节模组 · RP-hand 灵巧手），含急停与高频反馈闭环。" width="100%">

<p align="center"><strong>我们拒绝黑盒，没有阉割，所见即所得，把对机器人的绝对控制权完整交还开发者</strong></p>

<a id="repositories"></a>

## 仓库导航

> 具体发布内容、支持配置与安装步骤，以各子仓库维护的信息为准。
>
> 欢迎在对应子仓库参与贡献。本首页仓库不受理 PR；请前往相关项目提交 Issue 或 Pull Request。

### 硬件与工具

<table width="1000">
<thead>
<tr><th align="left" width="250">仓库</th><th align="left" width="750">说明</th></tr>
</thead>
<tbody>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/rp1_hardware"><strong>rp1_hardware</strong></a></td><td valign="middle" width="750">机械源文件、电气拓扑、原理图、PCB 走线、Gerber、线束、热管理、测试与 SOP 装配指南。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/ROMOMO"><strong>ROMOMO</strong></a></td><td valign="middle" width="750">关节模组：驱动器原理图、PCB 走线、Gerber、固件与上位机。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/rp_dexhand"><strong>RP Hand</strong></a></td><td valign="middle" width="750">灵巧手产品资料、接线、配套软件、CAD 与机器人模型，提供 C++ / Python / ROS 2 SDK 入口。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/rp1_test"><strong>RP1_TEST</strong></a></td><td valign="middle" width="750">RP1 整机测试相关内容。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/roboparty_joystick"><strong>roboparty_joystick</strong></a></td><td valign="middle" width="750">RoboParty 手柄与 App。</td></tr>
</tbody>
</table>

<details>
<summary><strong>查看机器人配置</strong></summary>

机器人配置以描述仓库当前发布版本为准。

| 配置 | 说明 |
| :--- | :--- |
| 24 DoF | 24 自由度配置 |
| 28 DoF | 固定头部配置 |
| 30 DoF | 搭载 2 自由度运动头部的配置 |
| 42 DoF | 搭载 2 自由度头部与双 RPhand 的配置 |

</details>

### 软件与系统

<table width="1000">
<thead>
<tr><th align="left" width="250">仓库</th><th align="left" width="750">说明</th></tr>
</thead>
<tbody>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/roboparty_deploy"><strong>roboparty_deploy</strong></a></td><td valign="middle" width="750">面向 RPO 与 RP1 的部署框架，提供 <code>imu</code>、<code>motor</code>、<code>inference</code>、<code>camera</code> 等易用 SDK，支持 C++ 与 Python 调用。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/RP1_description"><strong>RP1_description</strong></a></td><td valign="middle" width="750">URDF 与 MJCF 模型、3D 网格资源，以及机器人与 RP Hand 配置。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/roboparty_train"><strong>roboparty_train</strong></a></td><td valign="middle" width="750">基于 Isaac Lab 的 RPO 运动策略训练工作区，涵盖 AMP、BeyondMimic 与 Parkour 工作流，以及 RSL-RL 训练和动作重定向。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/RP1_firmware"><strong>RP1_firmware</strong></a></td><td valign="middle" width="750">Linux 底层 BSP、HPM USB-CAN、底层 SDK 与软件包源。</td></tr>
</tbody>
</table>

<a id="learning"></a>

### Demo

<table width="1000">
<thead>
<tr><th align="left" width="250">项目</th><th align="left" width="750">说明</th></tr>
</thead>
<tbody>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/robolab/tree/master/robolab/tasks/manager_based/amp"><strong>AMP</strong></a></td><td valign="middle" width="750">通过对抗训练从参考动作中学习运动先验，实现自然流畅的行走与运动控制。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/robolab/tree/master/robolab/tasks/manager_based/beyondmimic"><strong>BeyondMimic</strong></a></td><td valign="middle" width="750">跟踪参考动作以复现富有表现力的全身运动，包括舞蹈与动作模仿序列。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/robolab/tree/master/robolab/tasks/manager_based/parkour"><strong>Parkour</strong></a></td><td valign="middle" width="750">学习感知驱动的运动控制策略，可跨越台阶、沟壑与障碍等复杂地形。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/MimicLite"><strong>MimicLite</strong></a></td><td valign="middle" width="750">提供高效、通用的人形运动跟踪系统，用于训练可部署的 PPO 与 PPO-ROA 策略。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/UFO"><strong>UFO</strong></a></td><td valign="middle" width="750">提供面向人形控制的通用无监督强化学习框架，支持 FB/TeCH 训练、运动跟踪以及奖励与目标推断。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/P-BFM"><strong>PBFM</strong></a></td><td valign="middle" width="750">将参考动作、目标身体状态与奖励函数映射到共享的行为意图空间，并结合深度感知实现地形自适应控制。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/I-BFM-Code"><strong>IBFM</strong></a> <em>（即将支持 RP1）</em></td><td valign="middle" width="750">通过无监督强化学习实现奖励条件驱动的鲁棒人形交互，展示搬运、推箱与踢箱等任务。</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/INTACT-JEPA"><strong>INTACT-JEPA</strong></a> <em>（即将支持 RP1）</em></td><td valign="middle" width="750">基于 JEPA 学习意图到动作的映射，实现无需大范围动作搜索的目标条件机器人控制。</td></tr>
</tbody>
</table>

<details>
<summary><strong>相关论文</strong></summary>

- **[P-BFM: Perceptive Behavioral Foundation Models for Humanoid Control via Unsupervised Reinforcement Learning](https://arxiv.org/abs/2610.15833)** — Xue Wang, Yitang Li, Yiming Zhang, Siqin Wang, Junhan Sun, Zhihao Liu, Yaojie Shen, Jingbo Yuan, Hao Zhao, Qingdu Li. *ICLR 2027*
- **[I-BFM: Reward-Conditioned Robust Humanoid Interaction via Unsupervised Reinforcement Learning](https://arxiv.org/abs/2610.06129)** — Ziqi Han, Yitang Li, Junhan Sun, Fanrong Dong, Yaojie Shen, Lei Ye, Zetong Jing, Yongqi Zhang, Yiming Zhang, Xue Wang, Hao Zhao. *ICRA*
- **[PredActor: Predictive Action Diffusion for Steerable Onboard Humanoid Control](https://arxiv.org/abs/2609.24840)** — Lei Ye, Haibo Gao, Yitang Li, Peng Xu, Zetong Jing, Junhan Sun, Fanrong Dong, Ziqi Han, Xue Wang, Jianhua Sun, Cewu Lu, Hao Zhao, Liang Ding. *ICRA*
- **[From Hitter to Player: Separating Motor Execution and Strategy in Competitive Humanoid Table Tennis](https://arxiv.org/abs/2610.14067)** — Fanrong Dong, Ziyi Sun, Ziqi Han, Junhan Sun, Lei Ye, Zetong Jing, Hao Zhao, Shaoxun Liu, Rongrong Wang. *ICRA*
- **[INTACT: Isomorphic Intent-to-Action Learning for Search-Free World Models](https://arxiv.org/abs/2607.26056)** — Junhan Sun, Hao Zhao, Guofeng Zhang. *ICLR*
- **[VIStream: Bringing Inertial Sensing to Streaming Geometric Foundation Models](https://github.com/CN-MingZheLiu/vistream)** — Mingzhe Liu. *ICRA*

</details>

<a id="citation"></a>

## 引用

如果你在研究中使用了 RP1，请引用以下条目，并在论文中将机器人称为 **RoboParty RP1**。注明所用的硬件版本和软件 release 或 commit，便于他人复现你的结果。

```bibtex
@misc{roboparty2026rp1,
  title        = {{RP1}: An OpenSource Full-Stack Platform for Agentic Humanoids},
  author       = {{RoboParty}},
  year         = {2026},
  howpublished = {\url{https://github.com/Roboparty/RP1}}
}
```

如果你的工作基于某个子仓库（例如 Party OS 或 PartyMimic），也请一并引用该仓库。

<a id="community"></a>

## 开放共建，连接同行者

交流开发经验，分享你的项目，与 RoboParty 社区一起探索。

<p align="center">
  <a href="https://roboparty.com"><img src="https://img.shields.io/badge/Website-RoboParty-2563EB?style=flat-square&labelColor=6B7280" alt="Website: RoboParty" height="24"></a>
  <a href="https://qm.qq.com/q/546376843"><img src="https://img.shields.io/badge/QQ-546376843-12B7F5?style=flat-square&logo=tencentqq&logoColor=white" alt="QQ 群：546376843" height="24"></a>
  <a href="assets/wechat.png"><img src="https://img.shields.io/badge/WeChat-RP1-07C160?style=flat-square&logo=wechat&logoColor=white" alt="微信：RP1 交流群" height="24"></a>
  <a href="https://x.com/RoboParty_DEV"><img src="https://img.shields.io/badge/X-%40RoboParty_DEV-181818?style=flat-square&logo=x&logoColor=white" alt="X：@RoboParty_DEV" height="24"></a>
  <a href="https://discord.gg/V35Se8bNd"><img src="https://img.shields.io/badge/Discord-roboparty-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord：roboparty" height="24"></a>
  <a href="https://t.me/RoboParty_channel1"><img src="https://img.shields.io/badge/Telegram-RoboParty-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram：RoboParty_channel1" height="24"></a>
  <a href="https://space.bilibili.com/3546938634930456"><img src="https://img.shields.io/badge/Bilibili-roboparty-FB7299?style=flat-square&logo=bilibili&logoColor=white" alt="哔哩哔哩：roboparty" height="24"></a>
</p>

<h3 align="center">RoboParty 生态</h3>

<p align="center">
  <a href="https://github.com/Roboparty/ROMOMO"><img src="https://opengraph.githubassets.com/1/Roboparty/ROMOMO" alt="ROMOMO" width="24%"></a>
  <a href="https://github.com/Roboparty/Party_OS"><img src="https://opengraph.githubassets.com/1/Roboparty/Party_OS" alt="Party_OS" width="24%"></a>
  <a href="https://github.com/Roboparty/roboto_origin"><img src="https://opengraph.githubassets.com/f44bef10dbc6297cb05885961f85cf827ff0fce1ddd05ab08623bc02f79d338b/Roboparty/roboto_origin" alt="roboto_origin" width="24%"></a>
  <a href="https://github.com/Roboparty/human-humanoid-tools"><img src="https://opengraph.githubassets.com/1/Roboparty/human-humanoid-tools" alt="human-humanoid-tools" width="24%"></a>
</p>

---

<p align="center">
  <strong>RoboParty</strong><br>
  硬件开放，智能开放，可能性属于每一个人。
</p>

<p align="center">
  <a href="LICENSE">GPL-3.0</a> &nbsp; · &nbsp; © <a href="https://roboparty.com">RoboParty</a> &nbsp; · &nbsp; <a href="#top">返回顶部</a><br>
  <sub>各子仓库的适用许可证以其自身声明为准。</sub>
</p>
