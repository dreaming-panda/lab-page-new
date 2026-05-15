---
title: "InfiniAI Lab - Home"
layout: homelay
excerpt: "InfiniAI Lab at CMU."
sitemap: false
permalink: /
---

### About PI
**Beidi Chen** is an Assistant Professor at Carnegie Mellon University and Amazon Scholar. Previously, she was a visiting Research Scientist at FAIR. Before that, she was a postdoctoral scholar at Stanford University. She received her Ph.D. from Rice University. 

Her research focuses on efficient AI; specifically, she designs and optimizes algorithms on modern hardware to accelerate large machine learning systems. Her work has won best paper runner-up at ICML 2022 and best paper award at MICRO 2025. She has been recognized as a Rising Star in EECS by MIT and UIUC and is a recipient of the Google ML and Systems Junior Faculty Award as well as the Google Research Scholar Award.

### Research

InfiniAI Lab develops *efficient* and *scalable* AI models and systems by co-designing algorithms, model architectures, and hardware-aware infrastructure. Our research spans four interconnected directions:

#### 1. Sparse Model Architecture
Rethinking dense computation to unlock long-context, long-generation, and high-capacity models with better scaling laws.
- **Long-context & long-generation efficiency** — sub-quadratic attention, KV cache compression, and memory-efficient decoding for million-token workloads.
- **Capacity at constant compute** — Mixture-of-Experts (MoE), conditional computation, and modular architectures that grow parameters without growing FLOPs.
- **Scaling laws for sparsity** — empirical and theoretical studies of how sparse models scale with data, parameters, and compute.

#### 2. Scalable Agentic RL: Training & Inference
Building the systems stack for the next generation of reinforcement-learned, tool-using agents.
- **Large-scale RL training** — distributed RLHF/RLAIF, reward modeling, and stable optimization at frontier scale.
- **Asynchronous & off-policy RL** — decoupled rollout/learner pipelines that hide inference latency and maximize accelerator utilization.
- **Agentic serving** — multi-turn, multi-tool inference engines with shared prefix caches, speculative execution, and long-horizon state management.
- **Sparse attention & MoE inference** — kernel-level and scheduler-level optimizations for sparse experts and selective attention at serving time.

#### 3. Real-time & Multimodal Generation
Bringing generative AI to the interactive, multi-sensory loop where humans actually work and create.
- **Real-time generation** — streaming text, image, audio, and video synthesis with sub-second latency.
- **Multimodal models** — unified architectures across vision, language, speech, and action.
- **Human–AI collaboration** — interfaces and systems that enhance human fulfillment, creativity, and productivity rather than replace them.

#### 4. MLSys for the Post-AGI Era
Preparing infrastructure for a world where AI agents are first-class operators of the AI stack itself.
- **Self-building infrastructure** — agents that design, deploy, and tune ML systems with minimal human intervention.
- **Self-optimizing systems** — continuous, workload-aware optimization of training, serving, and data pipelines.
- **Security & robustness** — safeguards, sandboxing, and verification for autonomous AI operators.
- **Evolving AI ecosystems** — frameworks that let models, tools, and infrastructure co-evolve safely over time.
