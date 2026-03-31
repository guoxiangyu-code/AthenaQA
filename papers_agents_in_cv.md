# Agents in Computer Vision: Literature Survey & Paper List

> A curated list of top conference and journal papers on agents in computer vision, covering surveys, video understanding agents, visual programming agents, GUI/embodied agents, and vision-language-action models.
>
> Last updated: 2026-03-31

---

## Table of Contents

1. [Surveys & Overviews](#1-surveys--overviews)
2. [Video Understanding Agents](#2-video-understanding-agents)
3. [Visual Programming & Tool-Use Agents](#3-visual-programming--tool-use-agents)
4. [GUI & Autonomous Visual Agents](#4-gui--autonomous-visual-agents)
5. [Visual Grounding & Prompting Agents](#5-visual-grounding--prompting-agents)
6. [Vision-Language-Action (VLA) Models](#6-vision-language-action-vla-models)
7. [Embodied Vision Agents](#7-embodied-vision-agents)
8. [Benchmarks & Evaluation](#8-benchmarks--evaluation)
9. [Curated Resource Collections](#9-curated-resource-collections)

---

## 1. Surveys & Overviews

| # | Paper | Venue | Year | Link |
|---|-------|-------|------|------|
| 1 | **Vision Language Models: A Survey of 26K Papers (CVPR, ICLR, NeurIPS)** — Fengming Lin et al. Quantitative analysis of 26,104 accepted papers across top-3 ML/CV venues (2023–2025), tracking macro-trends in multimodal VLM research, agent-centric understanding, and parameter-efficient adaptation. | arXiv | 2025 | [arXiv:2510.09586](https://arxiv.org/abs/2510.09586) |
| 2 | **A Survey of State of the Art Large Vision Language Models: Alignment, Benchmark, Evaluations and Challenges** — Zongxia Li et al. Systematic overview of large VLMs (CLIP, Claude, GPT-4V), model architectures, benchmarking, evaluation, hallucination, alignment, and safety. | CVPR Workshop | 2025 | [CVF PDF](https://openaccess.thecvf.com/content/CVPR2025W/TMM-OpenWorld/papers/Li_A_Survey_of_State_of_the_Art_Large_Vision_Language_CVPRW_2025_paper.pdf) |
| 3 | **Video Understanding with Large Language Models: A Survey** — Continuously updated survey covering Vid-LLMs, agent architectures, taxonomies, training strategies, video comprehension tasks (reasoning, summarization, temporal localization, multi-modal interaction). | IEEE TCSVT | 2025 | [GitHub](https://github.com/yunlong10/Awesome-LLMs-for-Video-Understanding) |
| 4 | **GUI Agents: A Survey** — Comprehensive survey providing a unified framework for GUI agents powered by large foundation models, covering benchmarks (Mind2Web, WebArena), evaluation metrics, architectures, and training methods. | ACL Findings | 2025 | [arXiv:2412.13501](https://arxiv.org/abs/2412.13501) |
| 5 | **Vision-Language Navigation: A Survey and Taxonomy** — Wansen Wu et al. Taxonomy of VLN tasks, agents following language-based instructions in unseen environments, goal- and route-oriented tasks, knowledge integration, and real-world transfer. | Neural Computing & Applications | 2024 | [Springer](https://link.springer.com/article/10.1007/s00521-023-09217-1) |
| 6 | **Vision-Language-Action Models: Concepts, Progress, Applications and Challenges** — Ranjan Sapkota et al. Synthesis of advances in VLA models unifying perception, language understanding, and action for robotics, AR, and autonomous systems. | arXiv | 2025 | [arXiv:2505.04769](https://huggingface.co/papers/2505.04769) |
| 7 | **Pure Vision Language Action (VLA) Models: A Comprehensive Survey** — Dapeng Zhang et al. Systematic review of advanced VLA models covering autoregression-, diffusion-, reinforcement-, and hybrid-based paradigms. | arXiv | 2025 | [arXiv:2509.19012](https://papers.cool/arxiv/2509.19012) |
| 8 | **Large Language Model-Brained GUI Agents: A Survey** — Modular architectures integrating multimodal perception, memory, chain-of-thought planning, and robust UI action execution. | arXiv | 2024 | [emergentmind](https://www.emergentmind.com/topics/large-language-model-brained-gui-agents) |
| 9 | **Embodied Intelligent Agents and Agentic AI: A Comprehensive Review** — Synthesizes advances in vision-language-action models, sense-think-act architectures, sim-to-real transfer for robotics and embodied intelligence. | arXiv | 2025 | [PDF](https://storage.googleapis.com/tecla/Embodied_Intelligent_Agents_and_Agentic_AI__A_Comprehensive_Review_of_Agent_Models_paper.pdf) |

---

## 2. Video Understanding Agents

| # | Paper | Venue | Year | Link |
|---|-------|-------|------|------|
| 1 | **VideoAgent: Long-form Video Understanding with Large Language Model as Agent** — Fan Wang, Xinhao Li et al. LLM acts as a central agent that iteratively plans, queries VLMs on selected video segments, and reflects. Achieves SOTA on EgoSchema and NExT-QA with only ~8 frames per question. | ECCV | 2024 | [arXiv:2403.10517](https://arxiv.org/abs/2403.10517), [Project](https://wxh1996.github.io/VideoAgent-Website/) |
| 2 | **VideoAgent: A Memory-Augmented Multimodal Agent for Video Understanding** — Unified memory mechanism for event/object states; interactive tool-use abilities of LLMs; competitive with Gemini 1.5 Pro. | ECCV | 2024 | [Springer](https://link.springer.com/chapter/10.1007/978-3-031-72670-5_5), [PDF](https://www.bigai.ai/wp-content/uploads/2024/09/ECCV_VideoAgent.pdf) |
| 3 | **LLoVi: A Simple LLM Framework for Long-Range Video Question-Answering** — Ce Zhang et al. Two-stage pipeline: short-term visual captioner → LLM aggregation with multi-round summarization. SOTA on EgoSchema, NExT-QA, IntentQA. Training-free. | EMNLP | 2024 | [arXiv:2312.17235](https://arxiv.org/abs/2312.17235), [Code](https://github.com/CeeZh/LLoVi) |
| 4 | **TimeChat: A Time-sensitive Multimodal Large Language Model for Long Video Understanding** — Shuhuai Ren et al. Timestamp-aware frame encoder + sliding video Q-Former for temporal reasoning; instruction-tuned on TimeIT dataset (125K instances). | CVPR | 2024 | [CVF PDF](https://openaccess.thecvf.com/content/CVPR2024/papers/Ren_TimeChat_A_Time-sensitive_Multimodal_Large_Language_Model_for_Long_Video_CVPR_2024_paper.pdf), [Code](https://github.com/RenShuhuai-Andy/TimeChat) |
| 5 | **VTimeLLM: Empower LLM to Grasp Video Moments** — Boundary-aware training for precise temporal event localization in videos; dense captioning and temporal grounding. | CVPR | 2024 | [CVF PDF](https://openaccess.thecvf.com/content/CVPR2024/papers/Huang_VTimeLLM_Empower_LLM_to_Grasp_Video_Moments_CVPR_2024_paper.pdf), [Code](https://github.com/huangb23/VTimeLLM) |
| 6 | **Streaming Long Video Understanding with Large Language Models (VideoStreaming)** — Efficient VLLM for arbitrarily long videos via streaming encoding and adaptive memory selection. | NeurIPS | 2024 | [NeurIPS PDF](https://proceedings.neurips.cc/paper_files/paper/2024/file/d7ce06e9293c3d8e6cb3f80b4157f875-Paper-Conference.pdf) |
| 7 | **Unlocking Video-LLM via Agent-of-Thoughts Distillation (AoTD)** — LLMs decompose complex video questions into sub-tasks, deploying vision models as agentic tools with chain-of-thought reasoning. | ICLR submission | 2025 | [OpenReview](https://openreview.net/forum?id=mMfDfJ8JFJ) |
| 8 | **ActiveVideoPerception (AVP)** — Iterative plan→observe→reflect loop with LLM as controller for long video QA. Uses Gemini-2.5-Pro with multi-round evidence gathering and temporal reasoning. *(This repository's base framework)* | Salesforce Research | 2024 | [GitHub](https://github.com/SalesforceAIResearch/ActiveVideoPerception) |

---

## 3. Visual Programming & Tool-Use Agents

| # | Paper | Venue | Year | Link |
|---|-------|-------|------|------|
| 1 | **ViperGPT: Visual Inference via Python Execution for Reasoning** — Frames visual reasoning as programmable Python workflows invoking vision-language APIs. Modular, interpretable, SOTA on diverse visual reasoning benchmarks without extra training. | ICCV | 2023 | [arXiv:2303.08128](https://arxiv.org/abs/2303.08128), [Project](https://viper.cs.columbia.edu/) |
| 2 | **HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in Hugging Face** — LLM as orchestrator managing multiple domain-specific AI models (vision, speech, language). Plans tasks, selects models, executes multimodal sub-tasks. | NeurIPS | 2023 | [NeurIPS PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/77c33e6a367922d003ff102ffb92b658-Paper-Conference.pdf) |
| 3 | **MM-REACT: Prompting ChatGPT for Multimodal Reasoning and Action** — Microsoft. Integrates ChatGPT with specialized "vision experts" for multi-image reasoning, spatial queries, and advanced visual understanding via language prompts. | arXiv | 2023 | [arXiv:2303.11381](https://arxiv.org/abs/2303.11381), [Code](https://github.com/microsoft/MM-REACT) |
| 4 | **TaskMatrix / Visual ChatGPT** — Attaches ChatGPT to Visual Foundation Models (GroundingDINO, SAM) for visually grounded interactions: see, talk, draw, and edit. Template-based workflows for complex tasks. | arXiv | 2023 | [Code](https://github.com/chenfei-wu/TaskMatrix) |
| 5 | **Vision is Language: Visual Understanding via LLM** — Leverages frozen vision encoders + LLMs for VQA, exploring extensions to visual-language tasks underpinning video-VQA and multimodal agents. | Stanford CS231n | 2024 | [PDF](https://cs231n.stanford.edu/2024/papers/vision-is-language-visual-understanding-via-llm.pdf) |

---

## 4. GUI & Autonomous Visual Agents

| # | Paper | Venue | Year | Link |
|---|-------|-------|------|------|
| 1 | **CogAgent: A Visual Language Model for GUI Agents** — 18B VLM specialized in GUI understanding and navigation with dual-resolution image encoders. SOTA on VQA and GUI navigation tasks. | CVPR | 2024 | [CVF PDF](https://openaccess.thecvf.com/content/CVPR2024/papers/Hong_CogAgent_A_Visual_Language_Model_for_GUI_Agents_CVPR_2024_paper.pdf) |
| 2 | **GPT-4V(ision) is a Generalist Web Agent, if Grounded (SeeAct)** — Explores GPT-4V as a tool-using web-acting agent for real-world website navigation/manipulation. Best grounding uses both HTML and image cues. | ICLR Workshop | 2024 | [OpenReview](https://openreview.net/forum?id=ndcVUVgcHS) |
| 3 | **Aguvis: Unified Pure Vision Agents for Autonomous GUI Interaction** — "Pure vision" approach: GUI agents using only image-based observations and natural language instructions for cross-platform generalization. | ICLR submission | 2025 | [OpenReview](https://openreview.net/forum?id=FHtHH4ulEQ) |
| 4 | **AppAgent: Multimodal Agents as Smartphone Users** — Autonomous agents that interact with mobile apps via visual perception and natural language, learning to navigate UIs through exploration. | arXiv | 2023 | [arXiv:2312.13771](https://arxiv.org/abs/2312.13771) |
| 5 | **Mind2Web: Towards a Generalist Agent for the Web** — Benchmark for developing generalist web agents that can follow language instructions across diverse websites. | ICML | 2023 | [arXiv:2306.06070](https://arxiv.org/abs/2306.06070) |

---

## 5. Visual Grounding & Prompting Agents

| # | Paper | Venue | Year | Link |
|---|-------|-------|------|------|
| 1 | **Set-of-Mark Prompting Unleashes Extraordinary Visual Grounding in GPT-4V** — Visual prompting with region marks (alphanumerics, masks, boxes) from SAM/SEEM enables GPT-4V to perform fine-grained zero-shot visual grounding, surpassing specialist models. | arXiv / CVPR Workshop | 2024 | [arXiv:2310.11441](https://arxiv.org/abs/2310.11441), [Code](https://github.com/microsoft/SoM) |
| 2 | **GPT-4V-AD: Exploring Grounding for Zero-Shot Anomaly Detection** — GPT-4V's visual grounding for zero-shot anomaly detection via image region division and prompt engineering. | IJCAI | 2024 | [Springer](https://link.springer.com/chapter/10.1007/978-981-97-9003-6_1), [Code](https://github.com/zhangzjn/GPT-4V-AD) |

---

## 6. Vision-Language-Action (VLA) Models

| # | Paper | Venue | Year | Link |
|---|-------|-------|------|------|
| 1 | **RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control** — Google DeepMind. Directly fine-tunes VLMs for robotic manipulation, demonstrating emergent reasoning and generalization. | arXiv | 2023 | [arXiv:2307.15818](https://arxiv.org/abs/2307.15818) |
| 2 | **OpenVLA: An Open-Source Vision-Language-Action Model** — Open-source 7B VLA trained on Open X-Embodiment for generalist robotic manipulation, achieving SOTA across 29 tasks. | CoRL | 2024 | [arXiv:2406.09246](https://arxiv.org/abs/2406.09246) |

---

## 7. Embodied Vision Agents

| # | Paper | Venue | Year | Link |
|---|-------|-------|------|------|
| 1 | **SayCan: Do As I Can, Not As I Say — Grounding Language in Robotic Affordances** — Google. Grounds LLM reasoning in robotic capabilities via affordance functions for task planning in the real world. | CoRL | 2023 | [arXiv:2204.01691](https://arxiv.org/abs/2204.01691) |
| 2 | **Inner Monologue: Embodied Reasoning through Planning with Language Models** — Embodied agent uses LLMs for step-by-step planning with grounded feedback from vision, object detection, and scene understanding. | CoRL | 2023 | [arXiv:2207.05608](https://arxiv.org/abs/2207.05608) |
| 3 | **VOYAGER: An Open-Ended Embodied Agent with Large Language Models** — Minecraft agent with automatic curriculum generation, skill library, and iterative prompting. First LLM-powered lifelong learning agent. | NeurIPS | 2023 | [arXiv:2305.16291](https://arxiv.org/abs/2305.16291) |

---

## 8. Benchmarks & Evaluation

| # | Paper / Benchmark | Description | Link |
|---|-------------------|-------------|------|
| 1 | **VisualAgentBench (VAB)** | Rigorous evaluation for large multimodal models as visual foundation agents, spanning simulation, GUI manipulation, and visual design. | [arXiv:2408.06327](https://arxiv.org/abs/2408.06327) |
| 2 | **EgoSchema** | Long-form egocentric video QA benchmark. | [arXiv:2308.09126](https://arxiv.org/abs/2308.09126) |
| 3 | **NExT-QA** | Video question answering requiring causal and temporal reasoning. | [CVPR 2021](https://arxiv.org/abs/2105.08276) |
| 4 | **WebArena** | Realistic web environment benchmark for autonomous agents. | [arXiv:2307.13854](https://arxiv.org/abs/2307.13854) |
| 5 | **LVBench** | Long video benchmark for evaluating video understanding at scale. | Used in AVP evaluation |

---

## 9. Curated Resource Collections

| # | Resource | Description | Link |
|---|----------|-------------|------|
| 1 | **Awesome-LLMs-for-Video-Understanding** | Living list of top Vid-LLMs, agents, models, and benchmarks for video understanding. | [GitHub](https://github.com/yunlong10/Awesome-LLMs-for-Video-Understanding) |
| 2 | **Awesome-GUI-Agent** | Curated list of GUI agent papers, benchmarks, datasets, and projects (AppAgent, Mind2Web, WebArena, etc.). | [GitHub](https://github.com/showlab/Awesome-GUI-Agent) |
| 3 | **Awesome-VLM-Papers-And-Models** | Comprehensive vision-language model paper collection and model links. | [GitHub](https://github.com/zli12321/Vision-Language-Models-Overview) |

---

## Key Trends & Takeaways (2023–2025)

1. **Modular Agentic Design**: LLMs as high-level "managers" orchestrating vision-language tools/adapters for flexible reasoning and efficient processing.
2. **Memory and Tool-Use**: Structured memory (events/objects) and external tool invocation improve temporal reasoning and scalability for long-form video.
3. **Active Perception**: Iterative plan→observe→reflect loops (as in AVP/VideoAgent) enable efficient processing of long videos by selectively querying relevant segments.
4. **Temporal Precision**: Fine-grained localization and temporal event awareness are central to new architectures (VTimeLLM, TimeChat).
5. **Efficient Training & Adaptation**: Parameter-efficient strategies (prompting, LoRA, adapters) dominate over training from scratch.
6. **Visual Programming**: Composing visual reasoning as executable code (ViperGPT) or tool chains (MM-REACT, HuggingGPT) enables interpretable, modular solutions.
7. **GUI & Embodied Agents**: Rapid acceleration toward autonomous visual agents that interact with digital (CogAgent, SeeAct) and physical (RT-2, SayCan) environments.
8. **Challenges**: Visual hallucination, robust alignment, real-world grounding, long-context efficiency, and ethical deployment of agentic models.

---

## Relevance to AthenaQA / ActiveVideoPerception

This repository (AthenaQA) implements an **active video perception agent** that directly embodies several of the trends above:

- **Agent-based architecture**: Controller orchestrates Planner → Observer → Reflector in an iterative loop (similar to VideoAgent)
- **Selective temporal querying**: Plans specific video regions to observe rather than processing entire videos
- **LLM as reasoning core**: Uses Gemini-2.5-Pro / Qwen models as the central reasoning engine
- **Tool-use pattern**: ffmpeg for clip extraction, VLM for visual observation, LLM for planning and synthesis
- **Memory/evidence accumulation**: Blackboard pattern stores evidence across rounds for final synthesis

The papers listed above provide theoretical foundations and alternative approaches that inform and contextualize this system's design.
