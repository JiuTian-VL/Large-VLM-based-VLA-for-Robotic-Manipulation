<div align="center"> 

# Awesome VLM-based VLA for Robotic Manipulation 
[![arXiv](https://img.shields.io/badge/Arxiv-Large_VLM--based_VLA-red?logo=arxiv)](https://arxiv.org/abs/2508.13073)
[![Lab](https://img.shields.io/badge/Lab-JiuTian--VL-blue?link=https%3A%2F%2Fgithub.com%2FJiuTian-VL)](https://github.com/JiuTian-VL)
[![Contribution Welcome](https://img.shields.io/badge/Contributions-welcome-Green?logo=mercadopago&logoColor=white)](https://github.com/JiuTian-VL/Large-VLM-based-VLA-for-Robotic-Manipulation/pulls)
[![GitHub star chart](https://img.shields.io/github/stars/JiuTian-VL/Large-VLM-based-VLA-for-Robotic-Manipulation?link=https%3A%2F%2Fwww.star-history.com%2F%23JiuTian-VL%2FLarge-VLM-based-VLA-for-Robotic-Manipulation%26Date)](https://www.star-history.com/#JiuTian-VL/Large-VLM-based-VLA-for-Robotic-Manipulation&Date)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?)](LICENSE)



<h3 align="center">
  <strong>🛠️ We're still cooking — Stay tuned!🛠️<br>⭐ Give us a star if you like it! ⭐</strong>
</h3>

<img src="./pipline & timeline.png" alt="image info"> 

</div>


🔥 Large VLM-based Vision-Language-Action (VLA) models have recently emerged as a transformative paradigm for robotic manipulation by tightly coupling perception, language understanding, and action generation. Built upon large Vision-Language Models (VLMs), they enable robots to interpret natural language instructions, perceive complex environments, and perform diverse manipulation tasks with strong generalization.    

📍 We present **the first systematic survey on large VLM-based VLA models for robotic manipulation**. This repository serves as the companion resource to our survey: ["Large VLM-based Vision-Language-Action Models for Robotic Manipulation: A Survey"](https://arxiv.org/pdf/2508.13073), and includes all the research papers, benchmarks, and resources reviewed in the paper, organized for easy access and reference.

📌 We will **keep updating** this repository with newly published works to reflect the latest progress in the field. 


## Table of Contents

- [🤖 Awesome VLA for Robotic Manipulation](#awesome-vla-for-robotic-manipulation)
  - [🔍 Table of Contents](#table-of-contents)
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
  - [🗂️ Datasets and Benchmarks](#datasets-and-benchmarks)
    - [Real-world Robot Datasets](#real-world-robot-datasets)
    - [Simulation Environments and Benchmarks](#simulation-environments-and-benchmarks)
    - [Human Behavior Datasets](#human-behavior-datasets)
    - [Embodied Datasets and Benchmarks](#embodied-datasets-and-benchmarks)
  - [🔖 Citation](#citation)
  - [📧 Contact Us](#contact-us)


## Monolithic Models

### Single-System
<!-- | Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2023 | CoRL | [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) | [🌐](https://robotics-transformer2.github.io/) | [💻](-) |
| 2023 | ICRA | [RT-2-X: Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864) | [🌐](https://robotics-transformer-x.github.io/) | [💻](-) |
| 2023 | NeurIPS | [RoboFlamingo: Vision-Language Foundation Models as Effective Robot Imitators](https://arxiv.org/abs/2311.01378) | [🌐](https://roboflamingo.github.io/) | [💻](https://roboflamingo.github.io/) |
| 2023 | ICML | [LEO Agent: An Embodied Generalist Agent in 3D World](https://arxiv.org/abs/2311.12871) | [🌐](https://embodied-generalist.github.io/) | [💻](https://github.com/embodied-generalist/embodied-generalist) |
| 2024 | NeurIPS | [RoboMamba: Efficient Vision-Language-Action Model for Robotic Reasoning and Manipulation](https://arxiv.org/abs/2406.04339) | [🌐](https://sites.google.com/view/robomamba-web) | [💻](https://github.com/lmzpai/roboMamba?tab=readme-ov-file) |
| 2024 | CoRL | [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) | [🌐](https://openvla.github.io/) | [💻](https://github.com/openvla/openvla?tab=readme-ov-file) |
| 2024 | CoRL | [ECOT-Lite: Robotic Control via Embodied Chain-of-Thought Reasoning](https://arxiv.org/abs/2407.08693) | [🌐](https://embodied-cot.github.io/) | [💻](https://github.com/MichalZawalski/embodied-CoT/) |
| 2024 | ICRA | [ReVLA: Reverting Visual Domain Limitation of Robotic Foundation Models](https://arxiv.org/abs/2409.15250) | [🌐](https://insait-institute.github.io/ReVLA/) | [💻](-) |
| 2024 | NeurIPS | [DeeR-VLA: Dynamic Inference of Multimodal Large Language Models for Efficient Robot Execution](https://arxiv.org/abs/2411.02359) | [🌐](-) | [💻](https://github.com/yueyang130/DeeR-VLA) |
| 2024 | ICLR | [TraceVLA: Visual Trace Prompting Enhances Spatial-Temporal Awareness for Generalist Robotic Policies](https://arxiv.org/abs/2412.10345) | [🌐](https://tracevla.github.io/) | [💻](https://github.com/umd-huang-lab/tracevla) |
| 2025 | ICRA | [FuSe: Beyond Sight: Finetuning Generalist Robot Policies with Heterogeneous Sensors via Language Grounding](https://arxiv.org/abs/2501.04693) | [🌐](https://fuse-model.github.io/) | [💻](https://github.com/fuse-model/FuSe) |
| 2025 | CVPR | [UniAct: Universal Actions for Enhanced Embodied Foundation Models](https://arxiv.org/abs/2501.10105) | [🌐](https://2toinf.github.io/UniAct/) | [💻](https://github.com/2toinf/UniAct) |
| 2025 | arXiv | [SpatialVLA: Exploring Spatial Representations for Visual-Language-Action Model](https://arxiv.org/abs/2501.15830) | [🌐](https://spatialvla.github.io/) | [💻](https://github.com/SpatialVLA/SpatialVLA) |
| 2025 | ICML | [UP-VLA: A Unified Understanding and Prediction Model for Embodied Agent](https://arxiv.org/abs/2501.18867) | [🌐](-) | [💻](https://github.com/CladernyJorn/UP-VLA) |
| 2025 | ICLR | [VLAS: Vision-Language-Action Model with Speech Instructions for Customized Robot Manipulation](https://arxiv.org/abs/2502.13508) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [OpenVLA-OFT: Fine-Tuning Vision-Language-Action Models: Optimizing Speed and Success](https://arxiv.org/abs/2502.19645) | [🌐](https://openvla-oft.github.io/) | [💻](https://github.com/moojink/openvla-oft) |
| 2025 | arXiv | [PD-VLA: Accelerating Vision-Language-Action Model Integrated with Action Chunking via Parallel Decoding](https://arxiv.org/abs/2503.02310) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [HybridVLA: Collaborative Diffusion and Autoregression in a Unified Vision-Language-Action Model](https://arxiv.org/abs/2503.10631) | [🌐](https://hybrid-vla.github.io/) | [💻](https://github.com/PKU-HMI-Lab/Hybrid-VLA) |
| 2025 | arXiv | [MoLe-VLA: Dynamic Layer-Skipping Vision-Language-Action Model via Mixture-of-Layers for Efficient Robot Manipulation](https://arxiv.org/abs/2503.20384) | [🌐](https://sites.google.com/view/mole-vla) | [💻](https://github.com/RoyZry98/MoLe-VLA-Pytorch) |
| 2025 | CVPR | [CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models](https://arxiv.org/abs/2503.22020) | [🌐](https://cot-vla.github.io/) | [💻](-) |
| 2025 | arXiv | [NORA: A Small Open-Sourced Generalist Vision-Language-Action Model for Embodied Tasks](https://arxiv.org/abs/2504.19854) | [🌐](https://declare-lab.github.io/nora) | [💻](https://github.com/declare-lab/nora) |
| 2025 | arXiv | [VTLA: Vision-Tactile-Language-Action Model with Preference Learning for Insertion Manipulation](https://arxiv.org/abs/2505.09577) | [🌐](https://sites.google.com/view/vtla) | [💻](-) |
| 2025 | arXiv | [OE-VLA: Unveiling the Potential of Vision-Language-Action Models with Open-Ended Multimodal Instructions](https://arxiv.org/abs/2505.11214) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [ReFineVLA: Reasoning-Aware Teacher-Guided Transfer Fine-Tuning](https://arxiv.org/abs/2505.19080) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [FLashVLA: Think Twice, Act Once: Token-Aware Compression and Action Reuse for Efficient Inference in Vision-Language-Action Models](https://arxiv.org/abs/2505.21200) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [LoHoVLA: A Unified Vision-Language-Action Model for Long-Horizon Embodied Tasks](https://arxiv.org/abs/2506.00411) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [BitVLA: 1-Bit Vision-Language-Action Models for Robotics Manipulation](https://arxiv.org/abs/2506.07530) | [🌐](-) | [💻](https://github.com/ustcwhy/BitVLA?tab=readme-ov-file) |
| 2025 | arXiv | [BridgeVLA: Input-Output Alignment for Efficient 3D Manipulation Learning with Vision-Language Models](https://arxiv.org/abs/2506.07961) | [🌐](https://bridgevla.github.io/home_page.html) | [💻](https://github.com/BridgeVLA/BridgeVLA) |
| 2025 | arXiv | [UniVLA: Unified Vision-Language-Action Model](https://arxiv.org/abs/2506.17142) | [🌐](https://robertwyq.github.io/univla.github.io/) | [💻](https://github.com/baaivision/UniVLA) |
| 2025 | arXiv | [WorldVLA: Towards Autoregressive Action World Model](https://arxiv.org/abs/2506.21539) | [🌐](-) | [💻](https://github.com/alibaba-damo-academy/WorldVLA) |
| 2025 | arXiv | [4D-VLA: Spatiotemporal Vision-Language-Action Pretraining with Cross-Scene Calibration](https://arxiv.org/abs/2506.22242) | [🌐](-) | [💻](https://github.com/fudan-zvg/4D-VLA) |
| 2025 | ICCV | [VQ-VLA: Improving Vision-Language-Action Models via Scaling Vector-Quantized Action Tokenizers](https://arxiv.org/abs/2507.01016) | [🌐](https://xiaoxiao0406.github.io/vqvla.github.io/) | [💻](https://github.com/xiaoxiao0406/VQ-VLA) |
| 2025 | arXiv | [VOTE: Vision-Language-Action Optimization with Trajectory Ensemble Voting](https://arxiv.org/abs/2507.05116) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [SpecVLA: Speculative Decoding for Vision-Language-Action Models with Relaxed Acceptance](https://arxiv.org/abs/2507.22424) | [🌐](-) | [💻](-) |
| 2025 | arXiv | [ST-VLA: Spatial Traces: Enhancing VLA Models with Spatial-Temporal Understanding](https://arxiv.org/abs/2508.09032) | [🌐](https://ampiromax.github.io/ST-VLA/) | [💻](-) | -->


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2023 | CoRL | [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) | [🌐](https://robotics-transformer2.github.io/) | - |
| 2023 | ICRA | [RT-2-X: Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864) | [🌐](https://robotics-transformer-x.github.io/) | - |
| 2023 | NeurIPS | [RoboFlamingo: Vision-Language Foundation Models as Effective Robot Imitators](https://arxiv.org/abs/2311.01378) | [🌐](https://roboflamingo.github.io/) | [💻](https://roboflamingo.github.io/) |
| 2023 | ICML | [LEO Agent: An Embodied Generalist Agent in 3D World](https://arxiv.org/abs/2311.12871) | [🌐](https://embodied-generalist.github.io/) | [💻](https://github.com/embodied-generalist/embodied-generalist) |
| 2024 | NeurIPS | [RoboMamba: Efficient Vision-Language-Action Model for Robotic Reasoning and Manipulation](https://arxiv.org/abs/2406.04339) | [🌐](https://sites.google.com/view/robomamba-web) | [💻](https://github.com/lmzpai/roboMamba?tab=readme-ov-file) |
| 2024 | CoRL | [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) | [🌐](https://openvla.github.io/) | [💻](https://github.com/openvla/openvla?tab=readme-ov-file) |
| 2024 | CoRL | [ECOT-Lite: Robotic Control via Embodied Chain-of-Thought Reasoning](https://arxiv.org/abs/2407.08693) | [🌐](https://embodied-cot.github.io/) | [💻](https://github.com/MichalZawalski/embodied-CoT/) |
| 2024 | ICRA | [ReVLA: Reverting Visual Domain Limitation of Robotic Foundation Models](https://arxiv.org/abs/2409.15250) | [🌐](https://insait-institute.github.io/ReVLA/) | - |
| 2024 | NeurIPS | [DeeR-VLA: Dynamic Inference of Multimodal Large Language Models for Efficient Robot Execution](https://arxiv.org/abs/2411.02359) | - | [💻](https://github.com/yueyang130/DeeR-VLA) |
| 2024 | ICLR | [TraceVLA: Visual Trace Prompting Enhances Spatial-Temporal Awareness for Generalist Robotic Policies](https://arxiv.org/abs/2412.10345) | [🌐](https://tracevla.github.io/) | [💻](https://github.com/umd-huang-lab/tracevla) |
| 2025 | ICRA | [FuSe: Beyond Sight: Finetuning Generalist Robot Policies with Heterogeneous Sensors via Language Grounding](https://arxiv.org/abs/2501.04693) | [🌐](https://fuse-model.github.io/) | [💻](https://github.com/fuse-model/FuSe) |
| 2025 | CVPR | [UniAct: Universal Actions for Enhanced Embodied Foundation Models](https://arxiv.org/abs/2501.10105) | [🌐](https://2toinf.github.io/UniAct/) | [💻](https://github.com/2toinf/UniAct) |
| 2025 | arXiv | [SpatialVLA: Exploring Spatial Representations for Visual-Language-Action Model](https://arxiv.org/abs/2501.15830) | [🌐](https://spatialvla.github.io/) | [💻](https://github.com/SpatialVLA/SpatialVLA) |
| 2025 | ICML | [UP-VLA: A Unified Understanding and Prediction Model for Embodied Agent](https://arxiv.org/abs/2501.18867) | - | [💻](https://github.com/CladernyJorn/UP-VLA) |
| 2025 | ICLR | [VLAS: Vision-Language-Action Model with Speech Instructions for Customized Robot Manipulation](https://arxiv.org/abs/2502.13508) | - | - |
| 2025 | arXiv | [OpenVLA-OFT: Fine-Tuning Vision-Language-Action Models: Optimizing Speed and Success](https://arxiv.org/abs/2502.19645) | [🌐](https://openvla-oft.github.io/) | [💻](https://github.com/moojink/openvla-oft) |
| 2025 | arXiv | [PD-VLA: Accelerating Vision-Language-Action Model Integrated with Action Chunking via Parallel Decoding](https://arxiv.org/abs/2503.02310) | - | - |
| 2025 | arXiv | [HybridVLA: Collaborative Diffusion and Autoregression in a Unified Vision-Language-Action Model](https://arxiv.org/abs/2503.10631) | [🌐](https://hybrid-vla.github.io/) | [💻](https://github.com/PKU-HMI-Lab/Hybrid-VLA) |
| 2025 | arXiv | [MoLe-VLA: Dynamic Layer-Skipping Vision-Language-Action Model via Mixture-of-Layers for Efficient Robot Manipulation](https://arxiv.org/abs/2503.20384) | [🌐](https://sites.google.com/view/mole-vla) | [💻](https://github.com/RoyZry98/MoLe-VLA-Pytorch) |
| 2025 | CVPR | [CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models](https://arxiv.org/abs/2503.22020) | [🌐](https://cot-vla.github.io/) | - |
| 2025 | arXiv | [NORA: A Small Open-Sourced Generalist Vision-Language-Action Model for Embodied Tasks](https://arxiv.org/abs/2504.19854) | [🌐](https://declare-lab.github.io/nora) | [💻](https://github.com/declare-lab/nora) |
| 2025 | arXiv | [VTLA: Vision-Tactile-Language-Action Model with Preference Learning for Insertion Manipulation](https://arxiv.org/abs/2505.09577) | [🌐](https://sites.google.com/view/vtla) | - |
| 2025 | arXiv | [OE-VLA: Unveiling the Potential of Vision-Language-Action Models with Open-Ended Multimodal Instructions](https://arxiv.org/abs/2505.11214) | - | - |
| 2025 | arXiv | [ReFineVLA: Reasoning-Aware Teacher-Guided Transfer Fine-Tuning](https://arxiv.org/abs/2505.19080) | - | - |
| 2025 | arXiv | [FLashVLA: Think Twice, Act Once: Token-Aware Compression and Action Reuse for Efficient Inference in Vision-Language-Action Models](https://arxiv.org/abs/2505.21200) | - | - |
| 2025 | arXiv | [LoHoVLA: A Unified Vision-Language-Action Model for Long-Horizon Embodied Tasks](https://arxiv.org/abs/2506.00411) | - | - |
| 2025 | arXiv | [BitVLA: 1-Bit Vision-Language-Action Models for Robotics Manipulation](https://arxiv.org/abs/2506.07530) | - | [💻](https://github.com/ustcwhy/BitVLA?tab=readme-ov-file) |
| 2025 | arXiv | [BridgeVLA: Input-Output Alignment for Efficient 3D Manipulation Learning with Vision-Language Models](https://arxiv.org/abs/2506.07961) | [🌐](https://bridgevla.github.io/home_page.html) | [💻](https://github.com/BridgeVLA/BridgeVLA) |
| 2025 | arXiv | [UniVLA: Unified Vision-Language-Action Model](https://arxiv.org/abs/2506.17142) | [🌐](https://robertwyq.github.io/univla.github.io/) | [💻](https://github.com/baaivision/UniVLA) |
| 2025 | arXiv | [WorldVLA: Towards Autoregressive Action World Model](https://arxiv.org/abs/2506.21539) | - | [💻](https://github.com/alibaba-damo-academy/WorldVLA) |
| 2025 | arXiv | [4D-VLA: Spatiotemporal Vision-Language-Action Pretraining with Cross-Scene Calibration](https://arxiv.org/abs/2506.22242) | - | [💻](https://github.com/fudan-zvg/4D-VLA) |
| 2025 | ICCV | [VQ-VLA: Improving Vision-Language-Action Models via Scaling Vector-Quantized Action Tokenizers](https://arxiv.org/abs/2507.01016) | [🌐](https://xiaoxiao0406.github.io/vqvla.github.io/) | [💻](https://github.com/xiaoxiao0406/VQ-VLA) |
| 2025 | arXiv | [VOTE: Vision-Language-Action Optimization with Trajectory Ensemble Voting](https://arxiv.org/abs/2507.05116) | - | - |
| 2025 | arXiv | [SpecVLA: Speculative Decoding for Vision-Language-Action Models with Relaxed Acceptance](https://arxiv.org/abs/2507.22424) | - | - |
| 2025 | arXiv | [ST-VLA: Spatial Traces: Enhancing VLA Models with Spatial-Temporal Understanding](https://arxiv.org/abs/2508.09032) | [🌐](https://ampiromax.github.io/ST-VLA/) | - |
| 2025 | arXiv | [Discrete Diffusion VLA: Bringing Discrete Diffusion to Action Decoding in Vision-Language-Action Policies](https://arxiv.org/abs/2508.20072) | - | - |
| 2025 | arXiv | [LLaDA-VLA: Vision Language Diffusion Action Models](https://arxiv.org/abs/2509.06932) | [🌐](https://wenyuqing.github.io/llada-vla/) | - |
| 2025 | arXiv | [OccVLA: Vision-Language-Action Model with Implicit 3D Occupancy Supervision](https://arxiv.org/abs/2509.05578) | - | - |

---

### Dual-System
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2024 | arXiv | [A dual process vla: efficient robotic manipulation leveraging vlm](https://arxiv.org/abs/2410.15549) | - | - |
| 2024 | arXiv | [Towards synergistic, generalized, and efficient dual-system for robotic manipulation](https://arxiv.org/abs/2410.08001) | [🌐](https://robodual.github.io/) | - |
| 2024 | IROS | [From llms to actions: latent codes as bridges in hierarchical robot control](https://arxiv.org/abs/2405.04798) | - | - |
| 2025 | arXiv | [Gr00t n1: an open foundation model for generalist humanoid robots](https://arxiv.org/abs/2503.14734) | - | - |
| 2024 | arXiv | [Cogact: a foundational vision-language-action model for synergizing cognition and action in robotic manipulation](https://arxiv.org/abs/2411.19650) | [🌐](https://cogact.github.io/) | [💻](https://github.com/microsoft/CogACT) |
| 2024 | CoRL | [Hirt: enhancing robotic control with hierarchical robot transformers](https://arxiv.org/abs/2410.05273) | - | - |
| 2025 | arXiv | [GraspVLA: a Grasping Foundation Model Pre-trained on Billion-scale Synthetic Action Data](https://arxiv.org/abs/2505.03233) | [🌐](https://pku-epic.github.io/GraspVLA-web/) | [💻](https://github.com/PKU-EPIC/GraspVLA) |
| 2025 | arXiv | [Fast-in-slow: a dual-system foundation model unifying fast manipulation within slow reasoning](https://arxiv.org/abs/2506.01953) | [🌐](https://fast-in-slow.github.io/) | [💻](https://github.com/CHEN-H01/Fast-in-Slow) |
| 2025 | arXiv | [Openhelix: A short survey, empirical analysis, and open-source dual-system vla model for robotic manipulation](https://arxiv.org/abs/2505.03912) | [🌐](https://openhelix-robot.github.io/) | [💻](https://github.com/OpenHelix-robot/OpenHelix) |
| 2025 | arXiv | [Chatvla: unified multimodal understanding and robot control with vision-language-action model](https://arxiv.org/abs/2502.14420) | [🌐](https://chatvla.github.io/) | [💻](https://github.com/tutujingyugang1/ChatVLA_public) |
| 2025 | arXiv | [Chatvla-2: vision-language-action model with open-world embodied reasoning from pretrained knowledge](https://arxiv.org/abs/2505.21906) | [🌐](https://chatvla-2.github.io/) | - |
| 2025 | ICML | [Diffusionvla: scaling robot foundation models via unified diffusion and autoregression](https://arxiv.org/abs/2412.03293v1) | [🌐](https://diffusion-vla.github.io/) | [💻](https://github.com/juruobenruo/DexVLA) |
| 2025 | arXiv | [Trivla: a unified triple-system-based unified vision-language-action model for general robot control](https://arxiv.org/abs/2507.01424) | [🌐](https://zhenyangliu.github.io/TriVLA/) | - |
| 2025 | arXiv | [Information-theoretic graph fusion with vision-language-action model for policy reasoning and dual robotic control](https://arxiv.org/abs/2508.05342) | - | - |
| 2025 | arXiv | [Rationalvla: a rational vision-language-action model with dual system](https://arxiv.org/abs/2506.10826) | [🌐](https://irpn-eai.github.io/RationalVLA/) | - |
| 2025 | ICCV | [Vq-vla: improving vision-language-action models via scaling vector-quantized action tokenizers](https://arxiv.org/abs/2507.01016) | [🌐](https://xiaoxiao0406.github.io/vqvla.github.io/) | [💻](https://github.com/xiaoxiao0406/VQ-VLA) |
| 2025 | RA-L | [Tinyvla: towards fast, data-efficient vision-language-action models for robotic manipulation](https://arxiv.org/abs/2409.12514) | [🌐](https://tiny-vla.github.io/) | [💻](https://github.com/liyaxuanliyaxuan/TinyVLA) |
| 2025 | RSS | [π0: A vision-language-action flow model for general robot control](https://arxiv.org/abs/2410.24164) | [🌐](https://www.physicalintelligence.company/blog/pi0) | - |
| 2025 | RSS | [Fast: efficient action tokenization for vision-language-action models](https://arxiv.org/abs/2501.09747) | [🌐](https://www.pi.website/research/fast) | - |
| 2025 | arXiv | [π0.5: a vision language-action model with open-world generalization](https://arxiv.org/abs/2504.16054) | [🌐](https://www.pi.website/blog/pi05) | - |
| 2025 | arXiv | [Knowledge insulating vision-language-action models: train fast, run fast, generalize better](https://arxiv.org/abs/2505.23705) | [🌐](https://www.pi.website/research/knowledge_insulation) | - |
| 2025 | arXiv | [Forcevla: enhancing vla models with a force-aware moe for contact-rich manipulation](https://arxiv.org/abs/2505.22159) | [🌐](https://sites.google.com/view/forcevla2025) | - |
| 2025 | arXiv | [Smolvla: a vision-language-action model for affordable and efficient robotics](https://arxiv.org/abs/2506.01844) | - | [💻](https://github.com/huggingface/lerobot) |
| 2025 | arXiv | [Onetwovla: a unified vision-language-action model with adaptive reasoning](https://arxiv.org/abs/2505.11917) | [🌐](https://one-two-vla.github.io/) | [💻](https://github.com/Fanqi-Lin/OneTwoVLA) |
| 2025 | arXiv | [Tactile-vla: unlocking vision-language-action model’s physical knowledge for tactile generalization](https://arxiv.org/abs/2507.09160) | - | - |
| 2025 | arXiv | [Gr-3 technical report](https://arxiv.org/abs/2507.15493) | [🌐](https://seed.bytedance.com/en/GR3/) | - |
| 2025 | arXiv | [Villa-x: enhancing latent action modeling in vision-language-action models](https://arxiv.org/abs/2507.23682) | [🌐](https://microsoft.github.io/villa-x/) | [💻](https://github.com/microsoft/villa-x/) |
| 2025 | arXiv | [ThinkAct: Vision-Language-Action Reasoning via Reinforced Visual Latent Planning](https://arxiv.org/abs/2507.16815) | [🌐](https://jasper0314-huang.github.io/thinkact-vla/) | - |
| 2025 | arXiv | [F1: A Vision-Language-Action Model Bridging Understanding and Generation to Actions](https://arxiv.org/abs/2509.06951) | [🌐](https://aopolin-lv.github.io/F1-VLA/) | [💻](https://github.com/InternRobotics/F1-VLA) |

## Hierarchical Models

### Planner Only
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2023 | ICML | [PaLM-E: An embodied multimodal language model](https://proceedings.mlr.press/v202/driess23a/driess23a.pdf) | [🌐](https://palm-e.github.io/) | - |
| 2023 | arXiv | [ViLa: Look before you leap: Unveiling the power of GPT-4V in robotic vision-language planning](https://arxiv.org/abs/2311.17842) | [🌐](https://robot-vila.github.io/) | - |
| 2024 | CVPR | [MoManipVLA: Transferring vision-language-action models for general mobile manipulation](https://openaccess.thecvf.com/content/CVPR2025/papers/Wu_MoManipVLA_Transferring_Vision-language-action_Models_for_General_Mobile_Manipulation_CVPR_2025_paper.pdf) | [🌐](https://gary3410.github.io/momanipVLA/) | - |
| 2024 | CoRL | [RoboPoint: A vision-language model for spatial affordance prediction in robotics](https://proceedings.mlr.press/v270/yuan25c.html) | [🌐](https://robo-point.github.io/) | [💻](https://github.com/wentaoyuan/RoboPoint) |
| 2025 | arXiv | [ManipLVM-R1: Reinforcement learning for reasoning in embodied manipulation with large vision-language models](https://arxiv.org/abs/2505.16517) | - | - |
| 2025 | arXiv | [Embodied-Reasoner: Synergizing visual search, reasoning, and action for embodied interactive tasks](https://arxiv.org/abs/2503.21696) | [🌐](https://embodied-reasoner.github.io/) | [💻](https://github.com/zwq2018/embodied_reasoner) |
| 2025 | arXiv | [Reinforced Planning: Solving long-horizon tasks via imitation and reinforcement learning](https://arxiv.org/abs/2505.22050) | - | [💻](https://github.com/mail-taii/Reinforced-Reasoning-for-Embodied-Planning) |
| 2025 | ICRA | [Chain-of-Modality: Learning manipulation programs from multimodal human videos with vision-language-models](https://arxiv.org/abs/2504.13351) | [🌐](https://chain-of-modality.github.io/) | - |
| 2025 | arXiv | [Embodied-R: Collaborative framework for activating embodied spatial reasoning in foundation models via reinforcement learning](https://arxiv.org/abs/2504.12680) | [🌐](https://embodiedcity.github.io/Embodied-R/) | [💻](https://github.com/EmbodiedCity/Embodied-R.code) |
| 2025 | CVPR | [RoVI: Robotic Visual Instruction](https://openaccess.thecvf.com/content/CVPR2025/papers/Li_Robotic_Visual_Instruction_CVPR_2025_paper.pdf) | [🌐](https://robotic-visual-instruction.github.io/) | - |
| 2025 | arXiv | [ReLEP: Long-horizon embodied planning with implicit logical inference and hallucination mitigation](https://arxiv.org/abs/2409.15658) | - | - |
| 2025 | CVPR | [RoboBrain: A unified brain model for robotic manipulation from abstract to concrete](https://openaccess.thecvf.com/content/CVPR2025/papers/Ji_RoboBrain_A_Unified_Brain_Model_for_Robotic_Manipulation_from_Abstract_CVPR_2025_paper.pdf) | [🌐](https://superrobobrain.github.io/) | [💻](https://github.com/FlagOpen/RoboBrain2.0) |

---

### Planner + Policy
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2023 | arXiv | [Instruct2Act: Mapping multi-modality instructions to robotic actions with large language model](https://arxiv.org/abs/2305.11176) | - | [💻](https://github.com/OpenGVLab/Instruct2Act) |
| 2023 | CoRL | [VoxPoser: Composable 3D value maps for robotic manipulation with language models](https://arxiv.org/abs/2307.05973) | [🌐](https://voxposer.github.io/) | [💻](https://github.com/huangwl18/VoxPoser) |
| 2024 | CVPR | [SkillDiffuser: Interpretable hierarchical planning via skill abstractions in diffusion-based task execution](https://openaccess.thecvf.com/content/CVPR2024/papers/Liang_SkillDiffuser_Interpretable_Hierarchical_Planning_via_Skill_Abstractions_in_Diffusion-Based_Task_CVPR_2024_paper.pdf) | [🌐](https://skilldiffuser.github.io/) | [💻](https://github.com/Liang-ZX/skilldiffuser) |
| 2024 | arXiv | [RoboMatrix: A skill-centric hierarchical framework for scalable robot task planning and execution in open-world](https://arxiv.org/abs/2412.00171) | - | [💻](https://github.com/WayneMao/RoboMatrix) |
| 2024 | CoRL | [RT-Affordance: Reasoning about robotic manipulation with affordances](https://arxiv.org/abs/2411.02704) | [🌐](https://snasiriany.me/rt-affordance) | - |
| 2024 | CoRL | [LLARVA: Vision-action instruction tuning enhances robot learning](https://arxiv.org/abs/2406.11815) | [🌐](https://llarva24.github.io/) | [💻](https://github.com/Dantong88/LLARVA) |
| 2024 | CVPR | [MALMM: Multi-agent large language models for zero-shot robotics manipulation](https://arxiv.org/abs/2411.17636) | [🌐](https://malmm1.github.io/) | [💻](https://github.com/malmm1/MALMM) |
| 2024 | arXiv | [RT-H: Action Hierarchies Using Language](https://arxiv.org/abs/2403.01823) | [🌐](https://rt-hierarchy.github.io/) | - |
| 2024 | CoRL | [ReKep: Spatio-temporal reasoning of relational keypoint constraints for robotic manipulation](https://arxiv.org/abs/2409.01652) | [🌐](https://rekep-robot.github.io/) | [💻](https://github.com/huangwl18/ReKep) |
| 2025 | ICLR | [HAMSTER: Hierarchical action models for open-world robot manipulation](https://arxiv.org/abs/2503.21696) | [🌐](https://hamster-robot.github.io/) | [💻](https://github.com/liyi14/HAMSTER_beta) |
| 2025 | ICML | [HiRobot: Open-ended instruction following with hierarchical vision-language-action models](https://arxiv.org/abs/2502.19417) | [🌐](https://www.pi.website/research/hirobot) | - |
| 2025 | arXiv | [Agentic Robot: A brain-inspired framework for vision-language-action models in embodied agents](https://arxiv.org/abs/2505.23450) | [🌐](https://agentic-robot.github.io/) | [💻](https://github.com/Agentic-Robot/agentic-robot) |
| 2025 | arXiv | [DexVLA: Vision-language model with plug-in diffusion expert for general robot control](https://arxiv.org/abs/2502.05855) | [🌐](https://dex-vla.github.io/) | [💻](https://github.com/juruobenruo/DexVLA) |
| 2025 | arXiv | [PointVLA: Injecting the 3D world into vision-language-action models](https://arxiv.org/abs/2503.07511) | [🌐](https://pointvla.github.io/) | - |
| 2025 | arXiv | [A0: An affordance-aware hierarchical model for general robotic manipulation](https://arxiv.org/abs/2504.12636) | [🌐](https://a-embodied.github.io/A0/) | [💻](https://github.com/A-embodied/A0) |
| 2025 | arXiv | [From seeing to doing: Bridging reasoning and decision for robotic manipulation](https://arxiv.org/abs/2505.08548) | [🌐](https://embodied-fsd.github.io/) | [💻](https://github.com/pickxiguapi/Embodied-FSD) |
| 2025 | ICCV | [RoBridge: A hierarchical architecture bridging cognition and execution for general robotic manipulation](https://arxiv.org/abs/2505.01709) | [🌐](https://abliao.github.io/RoBridge/) | [💻](https://github.com/abliao/RoBridge) |
| 2025 | arXiv | [RoboCerebra: A large-scale benchmark for long-horizon robotic manipulation evaluation](https://arxiv.org/abs/2506.06677) | [🌐](https://robocerebra.github.io/) | - |
| 2025 | arXiv | [π0.5: A vision-language-action model with open-world generalization](https://arxiv.org/abs/2504.16054) | [🌐](https://pi.website/blog/pi05) | - |
| 2025 | arXiv | [DexGraspVLA: A vision-language-action framework towards general dexterous grasping](https://arxiv.org/abs/2502.20900) | [🌐](https://dexgraspvla.github.io/) | [💻](https://github.com/Psi-Robot/DexGraspVLA) |
| 2025 | arXiv | [HiBerNAC: Hierarchical brain-emulated robotic neural agent collective for disentangling complex manipulation](https://arxiv.org/abs/2506.08296) | - | - |
| 2025 | arXiv | [Robix: A Unified Model for Robot Interaction, Reasoning and Planning](https://arxiv.org/pdf/2509.01106) | [🌐](https://robix-seed.github.io/robix/) | - |



## Other Advanced Field

### Reinforcement Learning-based Methods
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2025 | ICLR(Workshop) | [GRAPE: Generalizing Robot Policy via Preference Alignment](https://openreview.net/pdf?id=XnwyFD1Fvw&utm_source=chatgpt.com) | [🌐](https://grape-vla.github.io/) | [💻](https://github.com/aiming-lab/grape) |
| 2025 | arXiv | [Vla-rl: Towards masterful and general robotic manipulation with scalable reinforcement learning](https://arxiv.org/abs/2505.18719) | - | [💻](https://github.com/GuanxingLu/vlarl) |
| 2025 | RSS | [ReWiND: Language-Guided Rewards Teach Robot Policies without New Demonstrations](https://openreview.net/pdf?id=a6lsCozWyM) | [🌐](https://rewind-reward.github.io/) | - |
| 2025 | RSS | [ConRFT: A Reinforced Fine-tuning Method for VLA Models via Consistency Policy](https://www.roboticsproceedings.org/rss21/p019.pdf) | [🌐](https://cccedric.github.io/conrft/) | [💻](https://github.com/cccedric/conrft) |
| 2025 | RSS | [RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning](https://www.roboticsproceedings.org/rss21/p028.pdf) | [🌐](https://generalist-distillation.github.io/) | - |
| 2025 | arXiv | [TGRPO: Fine-tuning Vision-Language-Action Model via Trajectory-wise Group Relative Policy Optimization](https://arxiv.org/abs/2506.08440) | - | - |
| 2025 | ICRA | [Improving Vision-Language-Action Model with Online Reinforcement Learning](https://arxiv.org/abs/2501.16664) | - | - |
| 2025 | CVPR(Workshop) | [Interactive Post‑Training for Vision‑Language‑Action Models](https://arxiv.org/abs/2505.17016) | [🌐](https://ariostgx.github.io/ript_vla/) | [💻](https://github.com/Ariostgx/ript-vla) |
| 2025 | arXiv | [Embodied-R1: Reinforced Embodied Reasoning for General Robotic Manipulation](https://arxiv.org/abs/2508.13998) | [🌐](https://embodied-r1.github.io/) | [💻](https://github.com/pickxiguapi/Embodied-R1) |

---

### Training-Free Methods
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2025 | arXiv | [VLA‑Cache: Towards Efficient Vision‑Language‑Action Model via Adaptive Token Caching in Robotic Manipulation](https://arxiv.org/abs/2502.02175) | - | [💻](https://github.com/siyuhsu/vla-cache) |
| 2025 | arXiv | [Accelerating Vision-Language-Action Model Integrated with Action Chunking via Parallel Decoding](https://arxiv.org/abs/2503.02310) | - | - |
| 2025 | arXiv | [Think Twice, Act Once: Token‑Aware Compression and Action Reuse for Efficient Inference in Vision‑Language‑Action Models](https://arxiv.org/abs/2505.21200) | - | - |
| 2025 | arXiv | [EfficientVLA: Training‑Free Acceleration and Compression for Vision‑Language‑Action Models](https://arxiv.org/abs/2506.10100) | - | - |
| 2025 | arXiv | [SP-VLA: A Joint Model Scheduling and Token Pruning Approach for VLA Model Acceleration](https://arxiv.org/abs/2506.12723) | - | - |
| 2025 | arXiv | [Block-wise Adaptive Caching for Accelerating Diffusion Policy](https://arxiv.org/abs/2506.13456) | - | - |
| 2025 | RSS | [FAST: Efficient Action Tokenization for Vision-Language-Action Models](https://www.roboticsproceedings.org/rss21/p012.pdf) | [🌐](https://www.pi.website/research/fast) | - |
| 2025 | arXiv | [Real-Time Execution of Action Chunking Flow Policies](https://arxiv.org/abs/2506.07339) | [🌐](https://www.pi.website/research/real_time_chunking) | - |

---

### Learning from Human Videos
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2024 | ICML | [3D‑VLA: A 3D Vision‑Language‑Action Generative World Model](https://arxiv.org/pdf/2403.09631) | [🌐](https://vis-www.cs.umass.edu/3dvla/) | [💻](https://github.com/UMass-Foundation-Model/3D-VLA) |
| 2024 | NeurIPS | [Learning an Actionable Discrete Diffusion Policy via Large‑Scale Actionless Video Pre‑Training](https://proceedings.neurips.cc/paper_files/paper/2024/file/378226e5df7eded3e401de5c9493143c-Paper-Conference.pdf) | [🌐](https://video-diff.github.io/) | [💻](https://github.com/tinnerhrhe/VPDD) |
| 2025 | CVPR | [Mitigating the Human‑Robot Domain Discrepancy in Visual Pre‑training for Robotic Manipulation](https://cvpr.thecvf.com/virtual/2025/poster/32537) | [🌐](https://jiaming-zhou.github.io/projects/HumanRobotAlign) | [💻](https://github.com/jiaming-zhou/HumanRobotAlign) |
| 2025 | RSS | [UniVLA: Learning to Act Anywhere with Task‑centric Latent Actions](https://www.roboticsproceedings.org/rss21/p014.pdf) | - | [💻](https://github.com/OpenDriveLab/UniVLA) |
| 2025 | ICLR | [Latent Action Pretraining from Videos](https://openreview.net/pdf?id=VYOe2eBQeh) | [🌐](https://latentactionpretraining.github.io/) | [💻](https://github.com/LatentActionPretraining/LAPA) |
| 2025 | arXiv | [Humanoid‑VLA: Towards Universal Humanoid Control with Visual Integration](https://arxiv.org/abs/2502.14795) | - | - |
<!-- | 2024 | ICML | [3D‑VLA: A 3D Vision‑Language‑Action Generative World Model](https://proceedings.mlr.press/v235/zhen24a.html) | [🌐](https://vis-www.cs.umass.edu/3dvla/) | [💻](https://github.com/UMass-Foundation-Model/3D-VLA) | -->
---

### World Model-based VLA
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
| 2024 | CVPR | [FoundationPose: Unified 6D Pose Estimation and Tracking of Novel Objects](https://openaccess.thecvf.com/content/CVPR2024/papers/Wen_FoundationPose_Unified_6D_Pose_Estimation_and_Tracking_of_Novel_Objects_CVPR_2024_paper.pdf) | [🌐](https://nvlabs.github.io/FoundationPose/) | [💻](https://github.com/NVlabs/FoundationPose) |
| 2024 | ICML | [3D‑VLA: A 3D Vision‑Language‑Action Generative World Model](https://arxiv.org/pdf/2403.09631) | [🌐](https://vis-www.cs.umass.edu/3dvla/) | [💻](https://github.com/UMass-Foundation-Model/3D-VLA) | 
| 2025 | arXiv | [WorldVLA: Towards Autoregressive Action World Model](https://arxiv.org/abs/2506.21539) | - | [💻](https://github.com/alibaba-damo-academy/WorldVLA) |
| 2025 | arXiv | [World4Omni: A Zero‑Shot Framework from Image Generation World Model to Robotic Manipulation](https://arxiv.org/abs/2506.23919) | [🌐](https://world4omni.github.io/) | - |
| 2025 | arXiv | [Robotic Manipulation by Imitating Generated Videos Without Physical Demonstrations](https://arxiv.org/abs/2507.00990) | [🌐](https://rigvid-robot.github.io/) | [💻](https://github.com/shivanshpatel35/rigvid) |
| 2025 | arXiv | [V‑JEPA 2: Self‑Supervised Video Models Enable Understanding, Prediction and Planning](https://arxiv.org/abs/2506.09985) | [🌐](https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/) | [💻](https://github.com/facebookresearch/vjepa2) |
| 2025 | arXiv | [FlowVLA: Thinking in Motion with a Visual Chain of Thought](https://arxiv.org/abs/2508.18269) | [🌐](https://irpn-lab.github.io/FlowVLA/) | - |
| 2025 | arXiv | [Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation](https://arxiv.org/abs/2508.05635) | [🌐](https://genie-envisioner.github.io/) | [💻](https://github.com/AgibotTech/Genie-Envisioner) | 

## Datasets and Benchmarks

### Real-world Robot Datasets
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|
| 2021 | CoRL  | [BC-Z: Zero-shot task generalization with robotic imitation learning](https://proceedings.mlr.press/v164/jang22a/jang22a.pdf) | [🌐](https://sites.google.com/view/bc-z/home) | [💻](https://github.com/google-research/tensor2robot/tree/master/research/bcz) | [📦](https://www.kaggle.com/datasets/google/bc-z-robot) |
| 2023 | RSS  | [RT‑1: Robotics Transformer for Real‑World Control at Scale](https://arxiv.org/abs/2212.06817) | [🌐](https://robotics-transformer1.github.io/) | [💻](https://github.com/google-research/robotics_transformer) | - |
| 2023 | CoRL  | [RT‑2: Vision‑Language Foundation Models as Effective Robot Imitators](https://arxiv.org/abs/2307.15818) | [🌐](https://robotics-transformer2.github.io/) | [💻](https://github.com/google-research/robotics_transformer) | - |
| 2022 | RSS  | [Bridge Data: Boosting Generalization of Robotic Skills with Cross‑Domain Datasets](https://arxiv.org/abs/2109.13396) | [🌐](https://sites.google.com/view/bridgedata) | [💻](https://github.com/yanlai00/bridge_data_imitation_learning) | [📦](https://sites.google.com/view/bridgedata) |
| 2023 | CoRL  | [BridgeData V2: A Dataset for Robot Learning at Scale](https://arxiv.org/abs/2308.12952) | [🌐](https://rail-berkeley.github.io/bridgedata/) | [💻](https://github.com/rail-berkeley/bridge_data_v2) | [📦](https://github.com/rail-berkeley/bridge_data_v2) |
| 2024 | ICRA | [RH20T: A Comprehensive Robotic Dataset for Learning Diverse Skills in One‑Shot](https://arxiv.org/abs/2307.00595) | [🌐](https://rh20t.github.io/) | [💻](https://github.com/rh20t) | [📦](https://github.com/rh20t/act_baseline) |
| 2024 | RSS | [DROID: A Large-Scale In‑The‑Wild Robot Manipulation Dataset](https://arxiv.org/abs/2403.12945) | [🌐](https://droid-dataset.github.io/) | [💻](https://github.com/droid-dataset/droid) | [📦](https://github.com/droid-dataset/droid_policy_learning) |
| 2024 | ICRA | [Open X‑Embodiment: Robotic Learning Datasets and RT‑X Models](https://arxiv.org/abs/2310.08864) | [🌐](https://robotics-transformer-x.github.io/) | [💻](https://github.com/google-deepmind/open_x_embodiment) | [📦](https://github.com/google-deepmind/open_x_embodiment) |
| 2025 | RSS | [RoboMIND: Benchmark on Multi-embodiment Intelligence Normative Data for Robot Manipulation](https://arxiv.org/abs/2412.13877) | [🌐](https://x-humanoid-robomind.github.io/) | [💻](https://github.com/x-humanoid-robomind/x-humanoid-robomind.github.io) | [📦](https://data.flopsera.com/data-detail/21181956226031626?type=open) |
| 2025 | IROS | [AgiBot World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems](https://arxiv.org/abs/2503.06669) | [🌐](https://agibot-world.com/) | [💻](https://github.com/OpenDriveLab/AgiBot-World) | [📦](https://huggingface.co/datasets/agibot-world/AgiBotWorld-Alpha) |
| 2025 | arXiv | [BRMData: Empowering Embodied Manipulation: A Bimanual-Mobile Robot Manipulation Dataset for Household Tasks](https://arxiv.org/pdf/2405.18860) | [🌐](https://embodiedrobot.github.io/) | [💻](https://github.com/Louis-ZhangLe/BRMData) | [📦](http://box.jd.com/sharedInfo/1147DC284DDAEE91DC759E209F58DD60) |

---

### Simulation Environments and Benchmarks
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|
| 2022 | CoRL | [BEHAVIOR‑1K: A Human‑Centered, Embodied AI Benchmark with 1,000 Everyday Activities and Realistic Simulation](https://arxiv.org/abs/2403.09227) | [🌐](https://behavior.stanford.edu/) | [💻](https://github.com/StanfordVL/BEHAVIOR-1K) | [📦](https://github.com/StanfordVL/BEHAVIOR-1K) |
| 2020 | CVPR | [ALFRED: A Benchmark for Interpreting Grounded Instructions for Everyday Tasks](https://arxiv.org/abs/1912.01734) | [🌐](https://askforalfred.com/) | [💻](https://github.com/askforalfred/alfred) | [📦](https://askforalfred.com/) |
| 2020 | RA-L | [RLBench: The Robot Learning Benchmark & Learning Environment](https://arxiv.org/abs/1909.12271) | [🌐](https://sites.google.com/view/rlbench) | [💻](https://github.com/stepjam/RLBench) | [📦](https://huggingface.co/datasets/hqfang/RLBench-18-Tasks) |
| 2024 | arXiv | [PerAct²: Benchmarking and Learning for Robotic Bimanual Manipulation Tasks](https://arxiv.org/abs/2407.00278) | [🌐](http://bimanual.github.io/) | [💻](https://github.com/markusgrotz/peract_bimanual) | [📦](https://bimanual.github.io/) |
| 2020 | CoRL | [Meta‑World: A Benchmark and Evaluation for Multi‑Task and Meta Reinforcement Learning](https://arxiv.org/abs/1910.10897) | [🌐](https://meta-world.github.io/) | [💻](https://github.com/Farama-Foundation/Metaworld) | [📦](https://github.com/Farama-Foundation/Metaworld) |
| 2019 | CoRL | [Relay Policy Learning: Solving Long-Horizon Tasks via Imitation and Reinforcement Learning](https://arxiv.org/abs/1910.11956) | [🌐](https://relay-policy-learning.github.io/) | [💻](https://github.com/google-research/relay-policy-learning) | [📦](https://minari.farama.org/datasets/D4RL/index.html) |
| 2023 | NeurIPS | [LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning](https://arxiv.org/abs/2306.03310) | [🌐](https://libero-project.github.io/) | [💻](https://github.com/Lifelong%E2%80%91Robot%E2%80%91Learning/LIBERO) | [📦](https://github.com/Lifelong%E2%80%91Robot%E2%80%91Learning/LIBERO) |
| 2022 | RA-L | [CALVIN: A Benchmark for Language‑Conditioned Policy Learning for Long‑Horizon Robot Manipulation Tasks](https://arxiv.org/abs/2112.03227) | [🌐](http://calvin.cs.uni-freiburg.de/) | [💻](https://github.com/mees/calvin) | [📦](https://github.com/mees/calvin) |
| 2024 | arXiv | [MIKASA: Memory, Benchmark & Robots: A Benchmark for Solving Complex Tasks with Reinforcement Learning](https://arxiv.org/abs/2502.10550) | [🌐](https://sites.google.com/view/memorybenchrobots/) | [💻](https://github.com/CognitiveAISystems/MIKASA-Robo) | [📦](https://huggingface.co/datasets/avanturist/mikasa-robo) |
| 2024 | CoRL | [SIMPLER: Evaluating Real‑World Robot Manipulation Policies in Simulation](https://arxiv.org/abs/2405.05941) | [🌐](https://simpler-env.github.io/) | [💻](https://github.com/simpler-env/SimplerEnv) | [📦](https://github.com/simpler-env/SimplerEnv) |
| 2019 | ICCV | [Habitat: A Platform for Embodied AI Research](https://arxiv.org/abs/1904.01201) | [🌐](https://aihabitat.org/) | [💻](https://github.com/facebookresearch/habitat-sim) | [📦](https://aihabitat.org/datasets/replica_cad/) |
| 2021 | NeurIPS| [Habitat 2.0: Training Home Assistants to Rearrange their Habitat](https://arxiv.org/abs/2106.14405) | [🌐](https://aihabitat.org/docs/habitat2) | [💻](https://github.com/facebookresearch/habitat-sim) | [📦](https://aihabitat.org/datasets/replica_cad/) |
| 2024 | ICLR | [Habitat 3.0: A Co‑Habitat for Humans, Avatars and Robots](https://arxiv.org/abs/2310.13724) | [🌐](https://aihabitat.org/habitat3/) | [💻](https://github.com/facebookresearch/habitat-sim) | [📦](https://aihabitat.org/datasets/replica_cad/) |
| 2020 | CVPR | [SAPIEN: A Simulated Part-based Interactive Environment](https://arxiv.org/abs/2003.08515) | [🌐](https://sapien.ucsd.edu/) | [💻](https://github.com/haosulab/SAPIEN) | [📦](https://sapien.ucsd.edu/downloads) |
| 2024 | RSS | [The Colosseum: A Benchmark for Evaluating Generalization for Robotic Manipulation](https://arxiv.org/abs/2402.08191) | [🌐](https://robot-colosseum.github.io/) | [💻](https://github.com/robot-colosseum/robot-colosseum) | [📦](https://huggingface.co/datasets/colosseum/colosseum-challenge) |
| 2025 | ICCV | [VLABench: A Large‑Scale Benchmark for Language‑Conditioned Robotics Manipulation with Long‑Horizon Reasoning Tasks](https://arxiv.org/abs/2412.18194) | [🌐](https://vlabench.github.io/) | [💻](https://github.com/OpenMOSS/VLABench) | [📦](https://huggingface.co/VLABench) |

---

### Human Behavior Datasets
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|
| 2022 | CVPR | [Ego4D: Around the World in 3,000 Hours of Egocentric Video](https://arxiv.org/abs/2110.07058) | [🌐](https://ego4d-data.org/) | [💻](https://github.com/facebookresearch/Ego4d) | [📦](https://ego4d-data.org/docs/start-here/) |
| 2024 | CVPR | [Ego‑Exo4D: Understanding Skilled Human Activity from First‑ and Third‑Person Perspectives](https://arxiv.org/abs/2311.18259) | [🌐](https://ego-exo4d-data.org/) | [💻](https://github.com/facebookresearch/Ego4d) | [📦](https://ego-exo4d-data.org/) |
| 2024 | arXiv | [EgoPlan‑Bench: Benchmarking Egocentric Embodied Planning with Multimodal Large Language Models](https://arxiv.org/abs/2312.06722) | [🌐](https://chenyi99.github.io/ego_plan/) | [💻](https://github.com/ChenYi99/EgoPlan) | [📦](https://drive.google.com/drive/folders/1qVtPzhHmCgdQ5JlMeAL3OZtvbHaXktTo) |
| 2024 | arXiv | [EgoVid‑5M: A Large‑Scale Video‑Action Dataset for Egocentric Video Generation](https://arxiv.org/abs/2411.08380) | [🌐](https://egovid.github.io/) | [💻](https://github.com/JeffWang987/EgoVid) | [📦](https://modelscope.cn/datasets/iic/EgoVid/) |
| 2018 | ECCV | [Scaling Egocentric Vision: The EPIC‑KITCHENS Dataset](https://arxiv.org/abs/1804.02748) | [🌐](http://epic-kitchens.github.io/) | [💻](http://epic-kitchens.github.io/) | [📦](https://epic-kitchens.github.io/2025#downloads) |
| 2024 | ECCV| [COM Kitchens: An Unedited Overhead‑View Video Dataset as a Vision‑Language Benchmark](https://arxiv.org/abs/2408.02272) | [🌐](https://github.com/omron-sinicx/com_kitchens) | [💻](https://github.com/omron-sinicx/com_kitchens) | [📦](https://github.com/omron-sinicx/com_kitchens) |
| 2019 | ICCV | [EgoVQA: An Egocentric Video Question Answering Benchmark Dataset](https://openaccess.thecvf.com/content_ICCVW_2019/papers/EPIC/Fan_EgoVQA_-_An_Egocentric_Video_Question_Answering_Benchmark_Dataset_ICCVW_2019_paper.pdf) | [🌐](https://github.com/YaoMarkMu/EgoVQA) | [💻](https://github.com/YaoMarkMu/EgoVQA) | [📦](http://vision.soic.indiana.edu/identifying-1st-3rd/) |
| 2022 | NeurIPS | [EgoTaskQA: Understanding Human Tasks in Egocentric Videos](https://arxiv.org/abs/2210.03929) | [🌐](https://sites.google.com/view/egotaskqa) | [💻](https://github.com/Buzz-Beater/EgoTaskQA) | [📦](https://sites.google.com/view/egotaskqa) |
| 2025 | arXiv| [EgoDex: Learning Dexterous Manipulation from Large‑Scale Egocentric Video](https://arxiv.org/abs/2505.11709) | - | - | - |
| 2024 | RSS | [DexCap: Scalable and Portable Mocap Data Collection System for Dexterous Manipulation](https://arxiv.org/abs/2403.07788) | [🌐](https://dex-cap.github.io/) | [💻](https://github.com/j96w/DexCap) | [📦](https://huggingface.co/datasets/chenwangj/DexCap-Data) |
| 2024 | arXiv | [EgoMimic: Scaling Imitation Learning via Egocentric Video](https://arxiv.org/abs/2410.24221) | [🌐](https://egomimic.github.io/) | [💻](https://github.com/SimarKareer/EgoMimic-Eve) | [📦](https://huggingface.co/datasets/gatech/EgoMimic/tree/main) |
| 2025 | CoRL | [Humanoid Policy ~ Human Policy](https://arxiv.org/abs/2503.13441) | [🌐](https://human-as-robot.github.io/) | [💻](https://github.com/RogerQi/human-policy) | [📦](https://huggingface.co/datasets/RogerQi/PH2D) |
| 2025 | arXiv | [Real2Render2Real: Scaling Robot Data Without Dynamics Simulation or Robot Hardware](https://arxiv.org/abs/2505.09601) | [🌐](https://real2render2real.com/) | [💻](https://github.com/uynitsuj/real2render2real) | - |

---

### Embodied Datasets and Benchmarks
| Year | Venue | Paper | Website | Code | Data |
|------|-------|-------|---------|------|------|
| 2018 | CVPR | [EQA: Embodied Question Answering](https://arxiv.org/abs/1711.11543) | [🌐](https://embodiedqa.org/) | [💻](https://github.com/facebookresearch/EmbodiedQA) | [📦](https://embodiedqa.org/data) |
| 2018 | CVPR | [IQA: Visual Question Answering in Interactive Environments](https://arxiv.org/abs/1712.03316) | - | [💻](https://github.com/danielgordon10/thor-iqa-cvpr-2018) | - |
| 2019 | CVPR | [MT‑EQA: Multi‑Target Embodied Question Answering](https://arxiv.org/abs/1904.04686) | [🌐](https://embodiedqa.org/) | [💻](https://github.com/facebookresearch/EmbodiedQA) | [📦](https://embodiedqa.org/data) |
| 2019 | CVPR | [Embodied Question Answering in Photorealistic Environments with Point Cloud Perception](https://arxiv.org/abs/1904.03461) | [🌐](https://embodiedqa.org/) | [💻](https://github.com/facebookresearch/EmbodiedQA) | [📦](https://embodiedqa.org/data) |
| 2023 | ICLR | [EQA‑MX: Embodied Question Answering using Multimodal Expression](https://openreview.net/pdf) | - | - | - |
| 2024 | CVPR | [OpenEQA: Embodied Question Answering in the Era of Foundation Models](https://openaccess.thecvf.com/content/CVPR2024/papers/Majumdar_OpenEQA_Embodied_Question_Answering_in_the_Era_of_Foundation_Models_CVPR_2024_paper.pdf) | [🌐](https://open-eqa.github.io/) | [💻](https://github.com/facebookresearch/open-eqa) | [📦](https://github.com/facebookresearch/open-eqa) |
| 2024 | ICLR | [LoTa‑Bench: Benchmarking Language‑oriented Task Planners for Embodied Agents](https://arxiv.org/abs/2402.08178) | [🌐](https://choi-jaewoo.github.io/LoTa-Bench/) | [💻](https://github.com/lbaa2022/LLMTaskPlanning) | [📦](https://github.com/lbaa2022/LLMTaskPlanning) |

[![Star History Chart](https://api.star-history.com/svg?repos=JiuTian-VL/Large-VLM-based-VLA-for-Robotic-Manipulation&Date)](https://www.star-history.com/#JiuTian-VL/Large-VLM-based-VLA-for-Robotic-Manipulation&Date)

## Citation

If you find this survey helpful for your research or applications, please consider citing it using the following BibTeX entry:

```
@misc{shao2025largevlmbasedvisionlanguageactionmodels,
      title={Large VLM-based Vision-Language-Action Models for Robotic Manipulation: A Survey}, 
      author={Rui Shao and Wei Li and Lingsen Zhang and Renshan Zhang and Zhiyang Liu and Ran Chen and Liqiang Nie},
      year={2025},
      eprint={2508.13073},
      archivePrefix={arXiv},
      primaryClass={cs.RO},
      url={https://arxiv.org/abs/2508.13073}, 
}
```

## Contact Us

For any questions or suggestions, please feel free to contact us at:

Email: shaorui@hit.edu.cn and liwei2024@stu.hit.edu.cn




