# 🧠 大模型训练与部署深度分析

> 📘 28章 深度分析 · 交互式 HTML 课程

> **English TL;DR:** An all-Chinese 28-chapter deep analysis of **LLM training & deployment** — from the three-stage training paradigm, data engineering, tokenizer and Transformer internals, through distributed training foundations (DP/MP, AdamW/Lion/Muon, mixed precision FP16/FP8, gradient checkpointing, ZeRO), 3D parallelism (TP/PP), MoE, training stability & scaling laws, to long-context training. Then alignment (SFT, RLHF/RM, DPO & its family IPO/KTO/SimPO, PEFT LoRA/QLoRA/DoRA, GRPO reasoning RL), multimodal, model merging/distillation. Deployment side: quantization (GPTQ/AWQ/GGUF), inference optimization (KV cache, speculative, FlashAttention), engines (vLLM/SGLang, prefill-decode split), edge (llama.cpp/MNN), cluster ops/fault recovery, ending with a full from-zero 1B project (pretrain → SFT+DPO → quantized deploy).

## 📖 课程简介

本课程对**大模型训练到部署的全链路**做深度剖析：前半程专注训练——预训练数据工程、Tokenizer、Transformer 内部、分布式与 3D 并行、混合精度与显存优化、MoE、稳定性、Scaling Laws、长上下文，以及数据配比与继续预训练、SFT、RLHF/RM、DPO 系、PEFT、GRPO/推理增强与多模态；后半程聚焦落地——模型合并/蒸馏、量化、推理优化、推理引擎与服务架构（vLLM/SGLang）、端侧部署、集群运维与故障恢复，最后以「从零到一：1B 模型预训练 → SFT+DPO → 量化部署」的完整实战收束。

## 🚀 快速开始

```bash
open index.html   # macOS，纯静态即开即看
```

## 📂 项目结构

```text
llm-training-deployment-tutorial/
├── index.html / 01.html ~ 28.html / courses.json / theme.css
```

## 📖 章节分段

| 阶段 | 章节 | 核心 |
|------|------|------|
| **训练基础** | 01–06 | 全景、数据、Tokenizer、Transformer、分布式、优化器 |
| **并行与规模化** | 07–12 | 混合精度、3D 并行、MoE、稳定性、Scaling、长上下文 |
| **数据与对齐** | 13–17 | 合成数据、Mid-training、SFT、RLHF、DPO |
| **高效与多模态** | 18–22 | PEFT、RLVR/推理、多模态、合并/蒸馏 |
| **部署与推理** | 23–27 | 量化、推理优化、引擎架构、端侧、集群故障 |
| **实战** | 28 | 1B 全闭环（预训练→SFT+DPO→量化部署） |

## ✨ 亮点

- 训练 → 对齐 → 部署全链路闭环，含从零 1B 实战
- 覆盖 DPO 族（IPO/KTO/SimPO）、PEFT（LoRA/QLoRA/DoRA）、GRPO/RLVR 等最新对齐
- 推理引擎（vLLM/SGLang/RT-LLM）+ 端侧部署 + 集群容错

## 🎯 前置知识

- 适合：LLM 训练 / 推理工程师、MLOps
- 建议具备：深度学习 + PyTorch 基础

## ✨ 特色

- 「训练深度 → 落地部署」双主线，实践导向
- 即开即用纯静态 HTML

---
*本课程由 `llm-training-deployment-tutorial/` 项目维护。*