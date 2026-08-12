# Awesome-Embodied-Robotics

具身智能(Embodied AI / VLA)领域优秀论文、Tech Report 与代码链接汇总。
重点整理 **[Physical Intelligence](https://www.pi.website/)**、**[NVIDIA](https://developer.nvidia.com/isaac/gr00t)**、**[Google DeepMind](https://deepmind.google/models/gemini-robotics/)**、**[Figure](https://www.figure.ai/)**、**[Tesla](https://www.tesla.com/AI)**、**[Generalist](https://generalistai.com/)**、**[Qwen (Alibaba)](https://github.com/QwenLM)**、**[字节跳动 ByteDance](https://arxiv.org/abs/2410.06158)**、**[智元机器人 AgiBot](https://agibot-world.com)**、**[灵初智能 PsiBot](https://github.com/Psi-Robot)**、**[自变量机器人 X Square](https://x2robot.com)**、**[宇树 Unitree](https://github.com/unitreerobotics)** 等团队,并附社区经典开源工作。

> 链接图例:[📄 Paper] 论文 ｜ [📝 Blog] 技术博客 ｜ [🌍 Website] 项目主页 ｜ [💻 Code] 代码 ｜ [🤗 Model] 模型 ｜ [📊 Dataset] 数据集
> 更新于 2026-07。

---

# Physical Intelligence (π 系列)

面向通用机器人策略(generalist policy)的 VLA 基础模型团队。研究列表:[https://www.pi.website/blog](https://www.pi.website/blog)

- **π0**, *A Vision-Language-Action Flow Model for General Robot Control*, 2024.10. [[📄 Paper](https://arxiv.org/abs/2410.24164)] [[📝 Blog](https://www.pi.website/blog/pi0)] [[💻 Code](https://github.com/Physical-Intelligence/openpi)] [[🤗 Model](https://huggingface.co/lerobot/pi0)]
- **FAST**, *FAST: Efficient Action Tokenization for Vision-Language-Action Models*, 2025.01. [[📄 Paper](https://arxiv.org/abs/2501.09747)] [[📝 Blog](https://www.pi.website/research/fast)] [[🤗 Model](https://huggingface.co/lerobot/pi0fast_base)]
- **openpi**, *Open Sourcing π0*, 2025.02. [[📝 Blog](https://www.pi.website/blog/openpi)] [[💻 Code](https://github.com/Physical-Intelligence/openpi)]
- **Hi Robot**, *Hi Robot: Open-Ended Instruction Following with Hierarchical Vision-Language-Action Models*, 2025.02. [[📄 Paper](https://arxiv.org/abs/2502.19417)] [[📝 Blog](https://www.pi.website/research/hirobot)]
- **π0.5**, *π0.5: a Vision-Language-Action Model with Open-World Generalization*, 2025.04. [[📄 Paper](https://arxiv.org/abs/2504.16054)] [[📝 Blog](https://www.pi.website/blog/pi05)]
- **π0 + KI**, *Knowledge Insulating Vision-Language-Action Models: Train Fast, Run Fast, Generalize Better*, 2025.05. [[📄 Paper](https://arxiv.org/abs/2505.23705)] [[📝 Blog](https://www.pi.website/research/knowledge_insulation)]
- **RTC**, *Real-Time Execution of Action Chunking Flow Policies*, 2025.06. [[📄 Paper](https://arxiv.org/abs/2506.07339)] [[📝 Blog](https://www.pi.website/research/real_time_chunking)]
- **π\*0.6**, *π\*0.6: a VLA that Learns from Experience*, 2025.11. [[📝 Blog](https://www.pi.website/blog/pistar06)]
- **Human-to-Robot**, *Emergence of Human to Robot Transfer in VLAs*, 2025.12. [[📝 Blog](https://www.pi.website/research/human_to_robot)]
- **Memory VLA**, *VLAs with Long and Short-Term Memory*, 2026.03. [[📝 Blog](https://www.pi.website/research/memory)]
- **RLT**, *Precise Manipulation with Efficient Online RL*, 2026.03. [[📝 Blog](https://www.pi.website/research/rlt)]
- **π0.7**, *π0.7: a Steerable Model with Emergent Capabilities*, 2026.04. [[📝 Blog](https://www.pi.website/blog/pi07)]

> **openpi** 仓库(Apache-2.0)包含 π0(flow-based VLA)、π0-FAST(自回归 VLA)、π0.5,基座 checkpoint 基于 10k+ 小时机器人数据预训练,提供 ALOHA / DROID / LIBERO 微调 checkpoint,支持 JAX 与 PyTorch。

---

# NVIDIA (GR00T / Cosmos)

面向通用人形机器人(generalist humanoid)的开放 VLA 基础模型。

- **GR00T N1**, *GR00T N1: An Open Foundation Model for Generalist Humanoid Robots*, 2025.03. [[📄 Paper](https://arxiv.org/abs/2503.14734)] [[🌍 Website](https://research.nvidia.com/labs/lpr/publication/gr00tn1_2025/)] [[💻 Code](https://github.com/NVIDIA/Isaac-GR00T)] [[🤗 Model](https://huggingface.co/nvidia/GR00T-N1.7-3B)]
  - 历史分支:[N1.5](https://github.com/NVIDIA/Isaac-GR00T/tree/n1d5) ｜ [N1.6](https://github.com/NVIDIA/Isaac-GR00T/tree/n1d6) ｜ 模型合集 [🤗](https://huggingface.co/collections/nvidia/gr00t-n17) ｜ 数据 [Physical AI](https://huggingface.co/collections/nvidia/physical-ai)
  - 架构:视觉-语言基础模型 + Diffusion Transformer 动作头;代码 Apache-2.0,权重 NVIDIA Open Model License。
- **Cosmos-Reason1**, *Cosmos-Reason1: From Physical Common Sense To Embodied Reasoning*, 2025.03. [[📄 Paper](https://arxiv.org/abs/2503.15558)] [[🌍 Website](https://research.nvidia.com/labs/dir/cosmos-reason1/)] [[💻 Code](https://github.com/nvidia-cosmos/cosmos-reason1)]

---

# Google DeepMind (RT / Gemini Robotics)

从 Robotics Transformer 到 Gemini Robotics 的通用机器人基础模型序列。研究主页:[https://deepmind.google/models/gemini-robotics/](https://deepmind.google/models/gemini-robotics/)

- **RT-1**, *RT-1: Robotics Transformer for Real-World Control at Scale*, 2022.12. [[📄 Paper](https://arxiv.org/abs/2212.06817)] [[🌍 Website](https://robotics-transformer1.github.io/)] [[💻 Code](https://github.com/google-research/robotics_transformer)]
- **PaLM-E**, *PaLM-E: An Embodied Multimodal Language Model*, 2023.03, ICML 2023. [[📄 Paper](https://arxiv.org/abs/2303.03378)] [[🌍 Website](https://palm-e.github.io/)]
- **RoboCat**, *RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation*, 2023.06, TMLR. [[📄 Paper](https://arxiv.org/abs/2306.11706)] [[📝 Blog](https://deepmind.google/discover/blog/robocat-a-self-improving-robotic-agent/)]
- **RT-2**, *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*, 2023.07, CoRL 2023. [[📄 Paper](https://arxiv.org/abs/2307.15818)] [[🌍 Website](https://robotics-transformer2.github.io/)] [[📝 Blog](https://deepmind.google/discover/blog/rt-2-new-model-translates-vision-and-language-into-action/)]
- **Q-Transformer**, *Q-Transformer: Scalable Offline RL via Autoregressive Q-Functions*, 2023.09, CoRL 2023. [[📄 Paper](https://arxiv.org/abs/2309.10150)]
- **Open X-Embodiment / RT-X**, *Open X-Embodiment: Robotic Learning Datasets and RT-X Models*, 2023.10, ICRA 2024. [[📄 Paper](https://arxiv.org/abs/2310.08864)] [[🌍 Website](https://robotics-transformer-x.github.io/)] [[💻 Code](https://github.com/google-deepmind/open_x_embodiment)]
- **RoboVQA**, *RoboVQA: Multimodal Long-Horizon Reasoning for Robotics*, 2023.11. [[📄 Paper](https://arxiv.org/abs/2311.00899)] [[🌍 Website](https://robovqa.github.io/)]
- **RT-Trajectory**, *RT-Trajectory: Robotic Task Generalization via Hindsight Trajectory Sketches*, 2023.11. [[📄 Paper](https://arxiv.org/abs/2311.01977)] [[🌍 Website](https://rt-trajectory.github.io/)]
- **SARA-RT**, *SARA-RT: Scaling up Robotics Transformers with Self-Adaptive Robust Attention*, 2023.12. [[📄 Paper](https://arxiv.org/abs/2312.01990)]
- **AutoRT**, *AutoRT: Embodied Foundation Models for Large Scale Orchestration of Robotic Agents*, 2024.01. [[📄 Paper](https://arxiv.org/abs/2401.12963)] [[🌍 Website](https://auto-rt.github.io/)]
- **ALOHA Unleashed**, *ALOHA Unleashed: A Simple Recipe for Robot Dexterity*, 2024.10, CoRL 2024. [[📄 Paper](https://arxiv.org/abs/2410.13126)] [[🌍 Website](https://aloha-unleashed.github.io/)]
- **Gemini Robotics**, *Gemini Robotics: Bringing AI into the Physical World*, 2025.03. [[📄 Paper](https://arxiv.org/abs/2503.20020)] [[🌍 Website](https://deepmind.google/models/gemini-robotics/)] [[📝 Blog](https://deepmind.google/discover/blog/shaping-the-future-of-advanced-robotics/)]
- **Gemini Robotics On-Device**, *首个可微调的端侧 VLA*, 2025.06. [[📝 Blog](https://deepmind.google/discover/blog/gemini-robotics-on-device-brings-ai-to-local-robotic-devices/)]
- **Gemini Robotics 1.5**, *Gemini Robotics 1.5: Pushing the Frontier of Generalist Robots with Advanced Embodied Reasoning, Thinking, and Motion Transfer*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.03342)] [[📝 Blog](https://deepmind.google/discover/blog/gemini-robotics-15-brings-ai-agents-into-the-physical-world/)]

> **世界模型 Genie 系列**(用于具身训练环境生成):Genie *Generative Interactive Environments*, 2024.02, ICML 2024 Best Paper [[📄 Paper](https://arxiv.org/abs/2402.15391)] ｜ [Genie 2](https://deepmind.google/discover/blog/genie-2-a-large-scale-foundation-world-model/), 2024.12 ｜ [Genie 3](https://deepmind.google/discover/blog/genie-3-a-new-frontier-for-world-models/), 2025.08。

---

# Figure

面向通用人形机器人的 System 1 / System 2 VLA 模型 Helix。技术更新以博客为主:[https://www.figure.ai/news](https://www.figure.ai/news)

- **Helix**, *Helix: A Vision-Language-Action Model for Generalist Humanoid Control*, 2025.02. [[📝 Blog](https://www.figure.ai/news/helix)]
- **Helix Logistics**, *Accelerating Real-World Logistics*, 2025.02. [[📝 Blog](https://www.figure.ai/news/helix-logistics)]
- **RL Walking**, *Natural Humanoid Walk Using Reinforcement Learning*, 2025.03. [[📝 Blog](https://www.figure.ai/news/reinforcement-learning-walking)]
- **Scaling Helix**, *A New State of the Art in Humanoid Logistics*, 2025.06. [[📝 Blog](https://www.figure.ai/news/scaling-helix-logistics)]
- **Project Go-Big**, *Internet-Scale Humanoid Pretraining and Direct Human-to-Robot Transfer*, 2025.09. [[📝 Blog](https://www.figure.ai/news/project-go-big)]
- **Helix 02**, *Introducing Helix 02: Full-Body Autonomy*, 2026.01. [[📝 Blog](https://www.figure.ai/news/helix-02)]

> Helix 采用双系统架构:7B VLM 骨干(System 2,7-9 Hz)+ 80M 交叉注意力 Transformer(System 1,200 Hz),端到端训练,覆盖 35-DoF 上半身动作空间。

---

# Tesla (Optimus)

Tesla 人形机器人 Optimus 沿用与 FSD 一致的纯视觉端到端神经网络技术栈,信息主要来自 AI Day 演示与产品页,暂无正式论文。

- **Optimus**, *Tesla 通用人形机器人*, AI Day 2021.08 首次发布,2022.09 展示原型。[[🌍 Website](https://www.tesla.com/AI)]

---

# Generalist

面向通用机器人的具身基础模型团队,随物理交互数据规模扩展。博客:[https://generalistai.com/blog](https://generalistai.com/blog)

- **GEN-0**, *Embodied Foundation Models That Scale with Physical Interaction*, 2025.11. [[📝 Blog](https://generalistai.com/blog/gen-0)]
- **GEN-1**, *Scaling Embodied Foundation Models to Mastery*, 2026.04. [[📝 Blog](https://generalistai.com/blog/gen-1)]
- **Beyond World Models**, *Going Beyond World Models & VLAs*, 2026.04. [[📝 Blog](https://generalistai.com/blog/beyond-world-models)]

---

# Qwen / Alibaba

Qwen 团队的多模态与具身相关工作。组织主页:[https://github.com/QwenLM](https://github.com/QwenLM)

- **Qwen-RobotManip**, *机器人操作(Manipulation)官方仓库*. [[💻 Code](https://github.com/QwenLM/Qwen-RobotManip)]
- **Qwen-RobotNav**, *机器人导航(Navigation)官方仓库*. [[💻 Code](https://github.com/QwenLM/Qwen-RobotNav)]
- **Qwen-AgentWorld**, *Language World Models for General Agents*(语言世界模型,Apache-2.0). [[💻 Code](https://github.com/QwenLM/Qwen-AgentWorld)]
- **Qwen3-VL**, *系列最强视觉-语言模型:3D grounding / 空间推理 / 具身 AI,可作为 VLA 视觉-语言底座*. [[💻 Code](https://github.com/QwenLM/Qwen3-VL)] [[🤗 Model](https://huggingface.co/Qwen)]
- **Qwen2.5-VL**, *Qwen2.5-VL Technical Report*, 2025.02. [[📄 Paper](https://arxiv.org/abs/2502.13923)] [[📝 Blog](https://qwenlm.github.io/blog/qwen2.5-vl/)] [[💻 Code](https://github.com/QwenLM/Qwen2.5-VL)] [[🤗 Model](https://huggingface.co/collections/Qwen/qwen25-vl-6795ffac22b334a837c0f9a5)]

---

# 字节跳动 ByteDance (GR 系列)

ByteDance Research / Seed 的视频生成预训练 + 机器人操作工作。

- **RoboFlamingo**, *Vision-Language Foundation Models as Effective Robot Imitators*, 2023.11, ICLR 2024 Spotlight. [[📄 Paper](https://arxiv.org/abs/2311.01378)] [[💻 Code](https://github.com/RoboFlamingo/RoboFlamingo)]
- **GR-1**, *Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation*, 2023.12, ICLR 2024. [[📄 Paper](https://arxiv.org/abs/2312.13139)]
- **GR-2**, *GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation*, 2024.10. [[📄 Paper](https://arxiv.org/abs/2410.06158)]

---

# 智元机器人 AgiBot (GO-1 / Genie)

与 OpenDriveLab 合作的大规模操作平台与世界模型。组织主页:[https://github.com/AgibotTech](https://github.com/AgibotTech)

- **GO-1 / AgiBot World**, *AgiBot World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems*, 2025.03, IROS 2025. [[📄 Paper](https://arxiv.org/abs/2503.06669)] [[🌍 Website](https://agibot-world.com)] [[💻 Code](https://github.com/OpenDriveLab/AgiBot-World)] [[📊 Dataset](https://huggingface.co/agibot-world)]
- **Genie Envisioner**, *Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation*, 2025.08. [[📄 Paper](https://arxiv.org/abs/2508.05635)] [[💻 Code](https://github.com/AgibotTech/Genie-Envisioner-V1)]
- **WholebodyVLA**, *Towards Unified Latent VLA for Whole-body Loco-manipulation Control*, ICLR 2026. [[💻 Code](https://github.com/OpenDriveLab/WholebodyVLA)]

---

# 灵初智能 PsiBot

灵初智能(PsiBot)的灵巧操作 VLA 工作。组织主页:[https://github.com/Psi-Robot](https://github.com/Psi-Robot)

- **DexGraspVLA**, *DexGraspVLA: A Vision-Language-Action Framework Towards General Dexterous Grasping*, 2025.02, AAAI 2026 Oral. [[📄 Paper](https://arxiv.org/abs/2502.20900)] [[💻 Code](https://github.com/Psi-Robot/DexGraspVLA)]
- **Awesome-VLA-Papers**, *VLA 论文合集(含 Action Tokenization 综述)*. [[💻 Code](https://github.com/Psi-Robot/Awesome-VLA-Papers)]

> Psi R0 / R0.5 / R1 为公司产品级模型(快慢双脑 + Chain-of-Action-Thought),以官网发布为准:[https://www.psibot.ai](https://www.psibot.ai)。

---

# 自变量机器人 X Square

端到端具身基础模型 WALL 系列。官网:[https://x2robot.com](https://x2robot.com)

- **WALL-OSS**, *Igniting VLMs toward the Embodied Space*, 2025.09. [[📄 Paper](https://arxiv.org/abs/2509.11766)] [[💻 Code](https://github.com/X-Square-Robot/wall-x)]

---

# 宇树 Unitree

宇树开源的机器人学习 / 强化学习与 VLA 代码库(Go2 / H1 / G1)。组织主页:[https://github.com/unitreerobotics](https://github.com/unitreerobotics)

- **unitree_rl_gym**, *Isaac Gym 强化学习示例(Go2/H1/G1 运动控制)*. [[💻 Code](https://github.com/unitreerobotics/unitree_rl_gym)]
- **unitree_rl_lab**, *基于 IsaacLab 的强化学习实现*. [[💻 Code](https://github.com/unitreerobotics/unitree_rl_lab)]
- **unitree_mujoco**, *MuJoCo 仿真与 sim-to-real(C++/Python)*. [[💻 Code](https://github.com/unitreerobotics/unitree_mujoco)]
- **xr_teleoperate**, *XR 设备遥操作与数据采集*. [[💻 Code](https://github.com/unitreerobotics/xr_teleoperate)]
- **unitree_lerobot**, *端到端具身智能:LeRobot 策略训练/推理与部署*. [[💻 Code](https://github.com/unitreerobotics/unitree_lerobot)]
- **unifolm-vla**, *面向人形操作的视觉-语言-动作大模型*. [[💻 Code](https://github.com/unitreerobotics/unifolm-vla)]
- **unifolm-world-model-action**, *开源世界模型-动作架构*. [[💻 Code](https://github.com/unitreerobotics/unifolm-world-model-action)]

---

# 社区经典开源工作

- **RT-2**, *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*, 2023.07, CoRL 2023. [[📄 Paper](https://arxiv.org/abs/2307.15818)] [[🌍 Website](https://robotics-transformer2.github.io/)]
- **Open X-Embodiment**, *Open X-Embodiment: Robotic Learning Datasets and RT-X Models*, 2023.10, ICRA 2024. [[📄 Paper](https://arxiv.org/abs/2310.08864)] [[🌍 Website](https://robotics-transformer-x.github.io)] [[💻 Code](https://github.com/google-deepmind/open_x_embodiment)]
- **Octo**, *Octo: An Open-Source Generalist Robot Policy*, 2024.05, RSS 2024. [[📄 Paper](https://arxiv.org/abs/2405.12213)] [[🌍 Website](https://octo-models.github.io)] [[💻 Code](https://github.com/octo-models/octo)] [[🤗 Model](https://huggingface.co/rail-berkeley)]
- **OpenVLA**, *OpenVLA: An Open-Source Vision-Language-Action Model*, 2024.06, CoRL 2024. [[📄 Paper](https://arxiv.org/abs/2406.09246)] [[🌍 Website](https://openvla.github.io/)] [[💻 Code](https://github.com/openvla/openvla)] [[🤗 Model](https://huggingface.co/openvla)]
- **RDT-1B**, *RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation*, 2024.10, ICLR 2025. [[📄 Paper](https://arxiv.org/abs/2410.07864)] [[🌍 Website](https://rdt-robotics.github.io/rdt-robotics/)] [[💻 Code](https://github.com/thu-ml/RoboticsDiffusionTransformer)] [[🤗 Model](https://huggingface.co/robotics-diffusion-transformer/rdt-1b)]
- **RoboBrain**, *RoboBrain: A Unified Brain Model for Robotic Manipulation from Abstract to Concrete*, 2025.02, CVPR 2025. [[📄 Paper](https://arxiv.org/abs/2502.21257)] [[🌍 Website](https://superrobobrain.github.io/)] [[💻 Code](https://github.com/FlagOpen/RoboBrain)] [[📊 Dataset](https://huggingface.co/datasets/BAAI/ShareRobot)]
- **GO-1 / AgiBot World**, *AgiBot World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems*, 2025.03. [[📄 Paper](https://arxiv.org/abs/2503.06669)] [[🌍 Website](https://agibot-world.com)] [[💻 Code](https://github.com/OpenDriveLab/AgiBot-World)] [[📊 Dataset](https://huggingface.co/agibot-world)]
- **LeRobot**, *端到端机器人学习库(集成 SmolVLA / ACT / Diffusion Policy / π0 移植)*. [[💻 Code](https://github.com/huggingface/lerobot)] [[🤗 Model](https://huggingface.co/lerobot)]
- **SmolVLA**, *SmolVLA: A Vision-Language-Action Model for Affordable and Efficient Robotics*, 2025.06. [[📄 Paper](https://arxiv.org/abs/2506.01844)] [[💻 Code](https://github.com/huggingface/lerobot)]
- **ACT / ALOHA**, *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware*, 2023.04, RSS 2023. [[📄 Paper](https://arxiv.org/abs/2304.13705)] [[🌍 Website](https://tonyzhaozh.github.io/aloha/)] [[💻 Code](https://github.com/tonyzhaozh/act)]
- **Mobile ALOHA**, *Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation*, 2024.01. [[📄 Paper](https://arxiv.org/abs/2401.02117)] [[🌍 Website](https://mobile-aloha.github.io/)] [[💻 Code](https://github.com/MarkFzp/mobile-aloha)]
- **Diffusion Policy**, *Diffusion Policy: Visuomotor Policy Learning via Action Diffusion*, 2023.03, RSS 2023. [[📄 Paper](https://arxiv.org/abs/2303.04137)] [[🌍 Website](https://diffusion-policy.cs.columbia.edu/)] [[💻 Code](https://github.com/real-stanford/diffusion_policy)]
- **3D Diffusion Policy (DP3)**, *3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations*, 2024.03, RSS 2024. [[📄 Paper](https://arxiv.org/abs/2403.03954)] [[💻 Code](https://github.com/YanjieZe/3D-Diffusion-Policy)]
- **Open-TeleVision**, *Open-TeleVision: Teleoperation with Immersive Active Visual Feedback*, 2024.07, CoRL 2024. [[📄 Paper](https://arxiv.org/abs/2407.01512)] [[🌍 Website](https://robot-tv.github.io/)] [[💻 Code](https://github.com/OpenTeleVision/TeleVision)]
- **Prismatic VLMs**, *Prismatic VLMs: Investigating the Design Space of Visually-Conditioned Language Models*, 2024.02, ICML 2024. [[📄 Paper](https://arxiv.org/abs/2402.07865)] [[💻 Code](https://github.com/TRI-ML/prismatic-vlms)]

## 人形 / 运动控制(Humanoid / Locomotion)

- **legged_gym**, *Learning to Walk in Minutes Using Massively Parallel Deep RL*, 2021.09, CoRL 2021. [[📄 Paper](https://arxiv.org/abs/2109.11978)] [[💻 Code](https://github.com/leggedrobotics/legged_gym)]
- **HumanPlus**, *HumanPlus: Humanoid Shadowing and Imitation from Humans*, 2024.06, CoRL 2024. [[📄 Paper](https://arxiv.org/abs/2406.10454)] [[🌍 Website](https://humanoid-ai.github.io/)] [[💻 Code](https://github.com/MarkFzp/humanplus)]
- **H2O / OmniH2O**, *H2O: Learning Human-to-Humanoid Real-Time Whole-Body Teleoperation*, 2024.03, IROS 2024. [[📄 Paper](https://arxiv.org/abs/2403.04436)] [[🌍 Website](https://human2humanoid.com/)] [[💻 Code](https://github.com/LeCAR-Lab/human2humanoid)]

## 仿真与基准(Simulators & Benchmarks)

- **Genesis**, *通用物理 / 生成式机器人仿真平台*, 2024.12. [[💻 Code](https://github.com/Genesis-Embodied-AI/Genesis)] [[📝 Blog](https://genesis-world.readthedocs.io/)]
- **Isaac Lab**, *NVIDIA 基于 Isaac Sim 的机器人学习框架*. [[💻 Code](https://github.com/isaac-sim/IsaacLab)] [[📝 Blog](https://isaac-sim.github.io/IsaacLab/)]
- **ManiSkill3**, *ManiSkill3: GPU Parallelized Robotics Simulation and Rendering for Generalizable Embodied AI*, 2024.10. [[📄 Paper](https://arxiv.org/abs/2410.00425)] [[💻 Code](https://github.com/haosulab/ManiSkill)]
- **robosuite**, *robosuite: A Modular Simulation Framework and Benchmark for Robot Learning*. [[📄 Paper](https://arxiv.org/abs/2009.12293)] [[🌍 Website](https://robosuite.ai/)] [[💻 Code](https://github.com/ARISE-Initiative/robosuite)]
- **LIBERO**, *LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning*, 2023.06, NeurIPS 2023. [[📄 Paper](https://arxiv.org/abs/2306.03310)] [[🌍 Website](https://libero-project.github.io/)] [[💻 Code](https://github.com/Lifelong-Robot-Learning/LIBERO)]
- **RLBench**, *RLBench: The Robot Learning Benchmark & Learning Environment*, 2019.09, RA-L 2020. [[📄 Paper](https://arxiv.org/abs/1909.12271)] [[💻 Code](https://github.com/stepjam/RLBench)]
- **RoboCasa**, *RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots*, 2024.06, RSS 2024. [[📄 Paper](https://arxiv.org/abs/2406.02523)] [[🌍 Website](https://robocasa.ai/)] [[💻 Code](https://github.com/robocasa/robocasa)]
- **CALVIN**, *CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks*, 2021.12, RA-L 2022. [[📄 Paper](https://arxiv.org/abs/2112.03227)] [[💻 Code](https://github.com/mees/calvin)]

---

## 说明
- 各团队博客随版本迭代持续更新,建议以官方 Blog / GitHub 最新 release 为准。
- 社区仓库以 GitHub star 数(约 >800)为收录参考,星标为近似值,请以仓库主页实时数据为准。
- 格式参考同目录 `template.md`(*[A Survey on VLA Models: An Action Tokenization Perspective](https://arxiv.org/abs/2507.01925)*)。
- 欢迎补充其他团队(1X、Skild、Galaxea、Sunday Robotics 等)。
