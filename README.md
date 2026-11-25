<a id="top"></a>

<p align="center">
  <strong>English</strong> &nbsp; / &nbsp; <a href="README.zh-CN.md">简体中文</a>
</p>

<a href="https://roboparty.com">
  <picture>
    <source media="(max-width: 640px)" srcset="assets/hero-en-mobile.jpg">
    <img src="assets/hero-en.jpg" alt="RoboParty RP1. Fully open-source humanoid platform." width="100%">
  </picture>
</a>

<h1 align="center">RP1: An OpenSource Full-Stack Platform for Agentic Humanoids</h1>

<p align="center">
  From mechanical design and electronics to firmware, control and learning.<br>
  Built to be understood. Open to be built upon.
</p>

<p align="center">
  <a href="https://roboparty.com"><img src="https://img.shields.io/badge/Website-RoboParty-2563EB?style=flat-square&labelColor=6B7280" alt="Website: RoboParty"></a>
  <a href="https://lab.roboparty.com/"><img src="https://img.shields.io/badge/Lab-RoboParty-2563EB?style=flat-square&labelColor=6B7280" alt="Lab: RoboParty"></a>
  <a href="https://github.com/Roboparty/Party_OS"><img src="https://img.shields.io/badge/GitHub-Party_OS-2563EB?style=flat-square&labelColor=6B7280" alt="GitHub: Party_OS"></a>
</p>

---

## Open by Design

**RP1 is RoboParty's fully open-source humanoid platform: a shared foundation for building, understanding and extending a real robot.**

The platform brings mechanical and electrical design, joint modules, firmware, robot models, deployment and learning into one connected development stack. Explore a single subsystem, reproduce a build, or develop your own control and learning workflows.

<table width="999">
<thead>
<tr><th align="left" width="333">Hardware you can inspect</th><th align="left" width="333">Software you can extend</th><th align="left" width="333">Intelligence you can explore</th></tr>
</thead>
<tbody>
<tr><td valign="top" width="333">Mechanical CAD, schematics, PCB layouts, Gerber files, BOM and assembly documentation.</td><td valign="top" width="333">Linux BSP, communication, device interfaces, robot descriptions and deployment modules.</td><td valign="top" width="333">Locomotion training, motion imitation, tracking and behavior-model projects.</td></tr>
</tbody>
</table>

<img src="assets/rp1-box-vault-hq.gif" alt="RP1 vaulting over a box" width="100%">

<p align="center"><sub>RP1, photographed in the real world.</sub></p>

<a id="architecture"></a>

## One Robot. A Connected Stack.

<img src="assets/architecture-en.svg#gh-light-mode-only" alt="RP1 control architecture: input / perception → motion control base (motion retargeting, motion policies) → real-time control (action decoding + serial-link solving at 500 Hz) → whole-body execution (ROMOMO joint modules, RP-hand), with an E-stop and a high-frequency feedback loop." width="100%">
<img src="assets/architecture-en-dark.svg#gh-dark-mode-only" alt="RP1 control architecture: input / perception → motion control base (motion retargeting, motion policies) → real-time control (action decoding + serial-link solving at 500 Hz) → whole-body execution (ROMOMO joint modules, RP-hand), with an E-stop and a high-frequency feedback loop." width="100%">

<p align="center"><strong>No black boxes, nothing withheld — full control handed back to the developer</strong></p>

<a id="repositories"></a>

## Explore the Repositories

> Release contents, supported configurations and setup instructions are maintained in each repository.
>
> Contributions belong in the relevant sub-repository. This overview repository does not accept pull requests; please open issues and pull requests in the project you are working on.

### Hardware & Tools

<table width="1000">
<thead>
<tr><th align="left" width="250">Repository</th><th align="left" width="750">Description</th></tr>
</thead>
<tbody>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/rp1_hardware"><strong>rp1_hardware</strong></a></td><td valign="middle" width="750">Mechanical source files, electronics, testing and assembly SOPs.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/ROMOMO"><strong>ROMOMO</strong></a></td><td valign="middle" width="750">Joint modules, firmware and host tools.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/rp_dexhand"><strong>RP Hand</strong></a></td><td valign="middle" width="750">Dexterous hand product documentation, wiring, companion applications, CAD and robot models. Includes the C++ / Python / ROS 2 SDK entry point.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/rp1_test"><strong>RP1_TEST</strong></a></td><td valign="middle" width="750">RP1 full-machine testing.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/roboparty_joystick"><strong>roboparty_joystick</strong></a></td><td valign="middle" width="750">RoboParty controller and app.</td></tr>
</tbody>
</table>

<details>
<summary><strong>Robot configurations</strong></summary>

See the description repository's current release for supported robot configurations.

Supported configurations include 24, 28, 30 and 42 DoF variants.

</details>

### Software & Systems

<table width="1000">
<thead>
<tr><th align="left" width="250">Repository</th><th align="left" width="750">Description</th></tr>
</thead>
<tbody>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/roboparty_deploy"><strong>roboparty_deploy</strong></a></td><td valign="middle" width="750">Deployment framework for RPO and RP1, with easy-to-use SDKs for <code>imu</code>, <code>motor</code>, <code>inference</code> and <code>camera</code> modules, callable from C++ and Python.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/RP1_description"><strong>RP1_description</strong></a></td><td valign="middle" width="750">URDF and MJCF models, 3D meshes, and robot and RP Hand configurations.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/roboparty_train"><strong>roboparty_train</strong></a></td><td valign="middle" width="750">Isaac Lab training workspace for RPO locomotion policies, covering AMP, BeyondMimic and Parkour workflows with RSL-RL training and motion retargeting.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/RP1_firmware"><strong>RP1_firmware</strong></a></td><td valign="middle" width="750">Linux BSP, USB-CAN bridge, low-level SDK and packages.</td></tr>
</tbody>
</table>

<a id="learning"></a>

### Demo

<table width="1000">
<thead>
<tr><th align="left" width="250">Project</th><th align="left" width="750">Description</th></tr>
</thead>
<tbody>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/robolab/tree/master/robolab/tasks/manager_based/amp"><strong>AMP</strong></a></td><td valign="middle" width="750">Learns motion priors from reference motions via adversarial training, enabling natural-looking locomotion and control.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/robolab/tree/master/robolab/tasks/manager_based/beyondmimic"><strong>BeyondMimic</strong></a></td><td valign="middle" width="750">Reproduces expressive whole-body movements by tracking reference motions, including dance and motion-imitation sequences.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/robolab/tree/master/robolab/tasks/manager_based/parkour"><strong>Parkour</strong></a></td><td valign="middle" width="750">Learns perceptive locomotion policies to traverse challenging terrain, including stairs, gaps and obstacles.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/MimicLite"><strong>MimicLite</strong></a></td><td valign="middle" width="750">Provides an efficient, general-purpose humanoid motion-tracking system for training deployable PPO and PPO-ROA policies.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/UFO"><strong>UFO</strong></a></td><td valign="middle" width="750">Provides a general unsupervised reinforcement learning framework for humanoid control, supporting FB/TeCH training, motion tracking and reward and goal inference.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/P-BFM"><strong>PBFM</strong></a></td><td valign="middle" width="750">Maps motion references, target body states and rewards into a shared behavioral intent space, combining intent with depth perception for terrain-adaptive control.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/I-BFM-Code"><strong>IBFM</strong></a> <em>(RP1 support coming soon)</em></td><td valign="middle" width="750">Learns reward-conditioned robust humanoid interaction via unsupervised reinforcement learning, demonstrated on carry, push and kick box tasks.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/PredActor"><strong>PredActor</strong></a> <em>(RP1 support coming soon)</em></td><td valign="middle" width="750">Predictive action diffusion model for steerable onboard humanoid control.</td></tr>
<tr height="56"><td valign="middle" width="250"><a href="https://github.com/Roboparty/INTACT-JEPA"><strong>INTACT-JEPA</strong></a> <em>(RP1 support coming soon)</em></td><td valign="middle" width="750">Learns an intent-to-action mapping with JEPA for goal-conditioned robot control without broad action search.</td></tr>
</tbody>
</table>

<details>
<summary><strong>Related papers</strong></summary>

- **[P-BFM: Perceptive Behavioral Foundation Models for Humanoid Control via Unsupervised Reinforcement Learning](https://arxiv.org/abs/2610.15833)** — Xue Wang, Yitang Li, Yiming Zhang, Siqin Wang, Junhan Sun, Zhihao Liu, Yaojie Shen, Jingbo Yuan, Hao Zhao, Qingdu Li. *ICLR 2027*
- **[I-BFM: Reward-Conditioned Robust Humanoid Interaction via Unsupervised Reinforcement Learning](https://arxiv.org/abs/2610.06129)** — Ziqi Han, Yitang Li, Junhan Sun, Fanrong Dong, Yaojie Shen, Lei Ye, Zetong Jing, Yongqi Zhang, Yiming Zhang, Xue Wang, Hao Zhao. *ICRA*
- **[PredActor: Predictive Action Diffusion for Steerable Onboard Humanoid Control](https://arxiv.org/abs/2609.24840)** — Lei Ye, Haibo Gao, Yitang Li, Peng Xu, Zetong Jing, Junhan Sun, Fanrong Dong, Ziqi Han, Xue Wang, Jianhua Sun, Cewu Lu, Hao Zhao, Liang Ding. *ICRA*
- **[From Hitter to Player: Separating Motor Execution and Strategy in Competitive Humanoid Table Tennis](https://arxiv.org/abs/2610.14067)** — Fanrong Dong, Ziyi Sun, Ziqi Han, Junhan Sun, Lei Ye, Zetong Jing, Hao Zhao, Shaoxun Liu, Rongrong Wang. *ICRA*
- **[INTACT: Isomorphic Intent-to-Action Learning for Search-Free World Models](https://arxiv.org/abs/2607.26056)** — Junhan Sun, Hao Zhao, Guofeng Zhang. *ICLR*
- **[VIStream: Bringing Inertial Sensing to Streaming Geometric Foundation Models](https://github.com/CN-MingZheLiu/vistream)** — Mingzhe Liu. *ICRA*

</details>

<a id="citation"></a>

## Citation

If you use RP1 in your research, please cite it as below and refer to the robot as **RoboParty RP1** in your paper. Stating the hardware version and the software release or commit you used helps others reproduce your results.

```bibtex
@misc{roboparty2026rp1,
  title        = {{RP1}: An OpenSource Full-Stack Platform for Agentic Humanoids},
  author       = {{RoboParty}},
  year         = {2026},
  howpublished = {\url{https://github.com/Roboparty/RP1}}
}
```

If your work builds on a specific sub-repository, such as Party OS or PartyMimic, please cite that repository as well.

<a id="community"></a>

## Built in the Open. Built Together.

Meet the community, share your work, and connect with RoboParty.

<p align="center">
  <a href="https://roboparty.com"><img src="https://img.shields.io/badge/Website-RoboParty-2563EB?style=flat-square&labelColor=6B7280" alt="Website: RoboParty" height="24"></a>
  <a href="https://qm.qq.com/q/546376843"><img src="https://img.shields.io/badge/QQ-546376843-12B7F5?style=flat-square&logo=tencentqq&logoColor=white" alt="QQ group 546376843" height="24"></a>
  <a href="assets/wechat.png"><img src="https://img.shields.io/badge/WeChat-RP1-07C160?style=flat-square&logo=wechat&logoColor=white" alt="WeChat: RP1 community QR code" height="24"></a>
  <a href="https://x.com/RoboParty_DEV"><img src="https://img.shields.io/badge/X-%40RoboParty_DEV-181818?style=flat-square&logo=x&logoColor=white" alt="X: @RoboParty_DEV" height="24"></a>
  <a href="https://discord.gg/V35Se8bNd"><img src="https://img.shields.io/badge/Discord-roboparty-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord: roboparty" height="24"></a>
  <a href="https://t.me/RoboParty_channel1"><img src="https://img.shields.io/badge/Telegram-RoboParty-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram: RoboParty_channel1" height="24"></a>
  <a href="https://space.bilibili.com/3546938634930456"><img src="https://img.shields.io/badge/Bilibili-roboparty-FB7299?style=flat-square&logo=bilibili&logoColor=white" alt="Bilibili: roboparty" height="24"></a>
</p>

<h3 align="center">The RoboParty Ecosystem</h3>

<p align="center">
  <a href="https://github.com/Roboparty/ROMOMO"><img src="https://opengraph.githubassets.com/1/Roboparty/ROMOMO" alt="ROMOMO" width="24%"></a>
  <a href="https://github.com/Roboparty/Party_OS"><img src="https://opengraph.githubassets.com/1/Roboparty/Party_OS" alt="Party_OS" width="24%"></a>
  <a href="https://github.com/Roboparty/roboto_origin"><img src="https://opengraph.githubassets.com/f44bef10dbc6297cb05885961f85cf827ff0fce1ddd05ab08623bc02f79d338b/Roboparty/roboto_origin" alt="roboto_origin" width="24%"></a>
  <a href="https://github.com/Roboparty/human-humanoid-tools"><img src="https://opengraph.githubassets.com/1/Roboparty/human-humanoid-tools" alt="human-humanoid-tools" width="24%"></a>
</p>

---

<p align="center">
  <strong>RoboParty</strong><br>
  Open hardware. Open intelligence. Shared possibility.
</p>

<p align="center">
  <a href="LICENSE">GPL-3.0</a> &nbsp; · &nbsp; © <a href="https://roboparty.com">RoboParty</a> &nbsp; · &nbsp; <a href="#top">Back to top</a><br>
  <sub>See each sub-repository for its applicable license.</sub>
</p>
