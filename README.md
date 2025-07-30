# Awesome VLA for Robotic Manipulation

<div style="text-align: center;">
  <img src="./pipline & timeline.png" alt="image info">
</div>


🔥 Vision-Language-Action (VLA) models have recently emerged as a transformative paradigm for robotic manipulation by tightly coupling perception, language understanding, and action generation. Built upon large-scale Vision-Language Models (VLMs), they enable robots to interpret natural language instructions, perceive complex environments, and perform diverse manipulation tasks with strong generalization.    

📍 We present **the first systematic survey on VLM-based VLA models for robotic manipulation**. This repository serves as the companion resource to our survey: ["Vision-Language-Action Models for Robotic Manipulation: A Survey"](https://arxiv.org/abs/xxxx.xxxxx), and includes all the research papers, benchmarks, and resources reviewed in the paper, organized for easy access and reference.

📌 We will keep updating this repository with newly published works to reflect the latest progress in the field. 


## Table of Contents

- [🤖 Awesome VLA for Robotic Manipulation](#awesome-vla-for-robotic-manipulation)
  - [🔍 Table of Contents](#table-of-contents)
  - [🗂️ Datasets and Benchmarks](#datasets-and-benchmarks)
    - [Real-world Robot Datasets](#real-world-robot-datasets)
    - [Simulation Environments and Benchmarks](#simulation-environments-and-benchmarks)
    - [Human Behavior Datasets](#human-behavior-datasets)
    - [Embodied Datasets and Benchmarks](#embodied-datasets-and-benchmarks)
  - [🧾 Monolithic Models](#monolithic-models)
    - [Single-System](#single-system)
    - [Dual-System](#dual-system)
  - [🧩 Hierarchical Models](#hierarchical-models)
    - [Planner Only](#planner-only)
    - [Planner + Policy](#planner--policy)
  - [🚀 Other Advanced Field](#other-advanced-field)
    - [Reinforcement Learning-based Methods](#reinforcement-learning-based-methods)
    - [Training-Free Methods](#training-free-methods)
    - [Learning from Human Videos](#learning-from-human-videos)
    - [World Model-based VLA](#world-model-based-vla)


## Datasets and Benchmarks

### Real-world Robot Datasets
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|
| 2021 | CoRL  | [Bc-z: Zero-shot task generalization with robotic imitation learning](https://proceedings.mlr.press/v164/jang22a/jang22a.) | [🌐](https://sites.google.com/view/bc-z/home) | [💻](https://github.com/google-research/tensor2robot/tree/master/research/bcz) | [📦](https://www.kaggle.com/datasets/google/bc-z-robot) |

---

### Simulation Environments and Benchmarks
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|

---

### Human Behavior Datasets
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|

---

### Embodied Datasets and Benchmarks
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|







## Monolithic Models

### Single-System
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2023 | CoRL | [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) | [🌐](https://robotics-transformer2.github.io/) | [💻]() |
| 2023 | ICRA | [RT-2-X: Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864) | [🌐](https://robotics-transformer-x.github.io/) | [💻]() |
| 2023 | NeurIPS | [RoboFlamingo: Vision-Language Foundation Models as Effective Robot Imitators](https://arxiv.org/abs/2311.01378) | [🌐](https://roboflamingo.github.io/) | [💻](https://roboflamingo.github.io/) |
| 2023 | ICML | [LEO Agent: An Embodied Generalist Agent in 3D World](https://arxiv.org/abs/2311.12871) | [🌐](https://embodied-generalist.github.io/) | [💻](https://github.com/embodied-generalist/embodied-generalist) |
| 2024 | NeurIPS | [RoboMamba: Efficient Vision-Language-Action Model for Robotic Reasoning and Manipulation](https://arxiv.org/abs/2406.04339) | [🌐](https://sites.google.com/view/robomamba-web) | [💻](https://github.com/lmzpai/roboMamba?tab=readme-ov-file) |
| 2024 | CoRL | [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) | [🌐](https://openvla.github.io/) | [💻](https://github.com/openvla/openvla?tab=readme-ov-file) |
| 2024 | CoRL | [ECOT-Lite: Robotic Control via Embodied Chain-of-Thought Reasoning](https://arxiv.org/abs/2407.08693) | [🌐](https://embodied-cot.github.io/) | [💻](https://github.com/MichalZawalski/embodied-CoT/) |
| 2024 | ICRA | [ReVLA: Reverting Visual Domain Limitation of Robotic Foundation Models](https://arxiv.org/abs/2409.15250) | [🌐](https://insait-institute.github.io/ReVLA/) | [💻]() |
| 2024 | NeurIPS | [DeeR-VLA: Dynamic Inference of Multimodal Large Language Models for Efficient Robot Execution](https://arxiv.org/abs/2411.02359) | [🌐]() | [💻](https://github.com/yueyang130/DeeR-VLA) |
| 2024 | ICLR | [TraceVLA: Visual Trace Prompting Enhances Spatial-Temporal Awareness for Generalist Robotic Policies](https://arxiv.org/abs/2412.10345) | [🌐](https://tracevla.github.io/) | [💻](https://github.com/umd-huang-lab/tracevla) |
| 2025 | CVPR | [UniAct: Universal Actions for Enhanced Embodied Foundation Models](https://arxiv.org/abs/2501.10105) | [🌐](https://2toinf.github.io/UniAct/) | [💻](https://github.com/2toinf/UniAct) |
| 2025 | - | [SpatialVLA: Exploring Spatial Representations for Visual-Language-Action Model](https://arxiv.org/abs/2501.15830) | [🌐](https://spatialvla.github.io/) | [💻](https://github.com/SpatialVLA/SpatialVLA) |
| 2025 | ICML | [UP-VLA: A Unified Understanding and Prediction Model for Embodied Agent](https://arxiv.org/abs/2501.18867) | [🌐]() | [💻](https://github.com/CladernyJorn/UP-VLA) |
| 2025 | ICLR | [VLAS: Vision-Language-Action Model with Speech Instructions for Customized Robot Manipulation](https://arxiv.org/abs/2502.13508) | [🌐]() | [💻]() |
| 2025 | - | [OpenVLA-OFT: Fine-Tuning Vision-Language-Action Models: Optimizing Speed and Success](https://arxiv.org/abs/2502.19645) | [🌐](https://openvla-oft.github.io/) | [💻](https://github.com/moojink/openvla-oft) |
| 2025 | - | [PD-VLA: Accelerating Vision-Language-Action Model Integrated with Action Chunking via Parallel Decoding](https://arxiv.org/abs/2503.02310) | [🌐]() | [💻]() |
| 2025 | - | [HybridVLA: Collaborative Diffusion and Autoregression in a Unified Vision-Language-Action Model](https://arxiv.org/abs/2503.10631) | [🌐](https://hybrid-vla.github.io/) | [💻](https://github.com/PKU-HMI-Lab/Hybrid-VLA) |
| 2025 | - | [MoLe-VLA: Dynamic Layer-Skipping Vision-Language-Action Model via Mixture-of-Layers for Efficient Robot Manipulation](https://arxiv.org/abs/2503.20384) | [🌐](https://sites.google.com/view/mole-vla) | [💻](https://github.com/RoyZry98/MoLe-VLA-Pytorch) |
| 2025 | CVPR | [CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models](https://arxiv.org/abs/2503.22020) | [🌐](https://cot-vla.github.io/) | [💻]() |
| 2025 | - | [NORA: A Small Open-Sourced Generalist Vision-Language-Action Model for Embodied Tasks](https://arxiv.org/abs/2504.19854) | [🌐](https://declare-lab.github.io/nora) | [💻](https://github.com/declare-lab/nora) |
| 2025 | - | [VTLA: Vision-Tactile-Language-Action Model with Preference Learning for Insertion Manipulation](https://arxiv.org/abs/2505.09577) | [🌐](https://sites.google.com/view/vtla) | [💻]() |
| 2025 | - | [OE-VLA: Unveiling the Potential of Vision-Language-Action Models with Open-Ended Multimodal Instructions](https://arxiv.org/abs/2505.11214) | [🌐]() | [💻]() |
| 2025 | - | [ReFineVLA: Reasoning-Aware Teacher-Guided Transfer Fine-Tuning](https://arxiv.org/abs/2505.19080) | [🌐]() | [💻]() |
| 2025 | - | [FLashVLA: Think Twice, Act Once: Token-Aware Compression and Action Reuse for Efficient Inference in Vision-Language-Action Models](https://arxiv.org/abs/2505.21200) | [🌐]() | [💻]() |
| 2025 | - | [LoHoVLA: A Unified Vision-Language-Action Model for Long-Horizon Embodied Tasks](https://arxiv.org/abs/2506.00411) | [🌐]() | [💻]() |
| 2025 | - | [FiS-VLA: Fast-in-Slow: A Dual-System Foundation Model Unifying Fast Manipulation within Slow Reasoning](https://arxiv.org/abs/2506.01953) | [🌐](https://fast-in-slow.github.io/) | [💻](https://github.com/CHEN-H01/Fast-in-Slow) |
| 2025 | - | [BitVLA: 1-Bit Vision-Language-Action Models for Robotics Manipulation](https://arxiv.org/abs/2506.07530) | [🌐]() | [💻](https://github.com/ustcwhy/BitVLA?tab=readme-ov-file) |
| 2025 | - | [BridgeVLA: Input-Output Alignment for Efficient 3D Manipulation Learning with Vision-Language Models](https://arxiv.org/abs/2506.07961) | [🌐](https://bridgevla.github.io/home_page.html) | [💻](https://github.com/BridgeVLA/BridgeVLA) |
| 2025 | - | [WorldVLA: Towards Autoregressive Action World Model](https://arxiv.org/abs/2506.21539) | [🌐]() | [💻](https://github.com/alibaba-damo-academy/WorldVLA) |
| 2025 | - | [VOTE: Vision-Language-Action Optimization with Trajectory Ensemble Voting](https://arxiv.org/abs/2507.05116) | [🌐]() | [💻]() |


---

### Dual-System
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|





## Hierarchical Models

### Planner Only
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|

---

### Planner + Policy
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|







## Other Advanced Field

### Reinforcement Learning-based Methods
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2025 | ICLR(Workshop)  | [GRAPE: Generalizing Robot Policy via Preference Alignment](https://openreview.net/pdf?id=XnwyFD1Fvw&utm_source=chatgpt.com) | [🌐](https://grape-vla.github.io/) | [💻](https://github.com/aiming-lab/grape) |
| 2025 | arXiv | [Vla-rl: Towards masterful and general robotic manipulation with scalable reinforcement learning](https://arxiv.org/abs/2505.18719) | - | [💻](https://github.com/GuanxingLu/vlarl) |
| 2025 | RSS | [ReWiND: Language-Guided Rewards Teach Robot Policies without New Demonstrations](https://openreview.net/pdf?id=a6lsCozWyM) | [🌐](https://rewind-reward.github.io/) | - |
| 2025 | RSS | [ConRFT: A Reinforced Fine-tuning Method for VLA Models via Consistency Policy](https://www.roboticsproceedings.org/rss21/p019.pdf) | [🌐](https://cccedric.github.io/conrft/) | [💻](https://github.com/cccedric/conrft) |
| 2025| arXiv | [TGRPO: Fine-tuning Vision-Language-Action Model via Trajectory-wise Group Relative Policy Optimization](https://arxiv.org/abs/2506.08440) | - | - |
---

### Training-Free Methods
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|

---

### Learning from Human Videos
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|

---

### World Model-based VLA
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
