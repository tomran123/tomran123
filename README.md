# Cunzhou Ran | 冉存洲


**AI infrastructure · Inference optimization · Reliable AI applications**


[English](#english) · [中文](#中文) · [Intel portfolio](https://github.com/tomran123/intel_cunzhou) · [WealthPortfolio](https://github.com/tomran123/wealthprofolio)


## English


I'm a Computer Science and Mathematics undergraduate at **The University of Texas at Austin**, expecting to graduate in **December 2027**. Previously, I was a **Software Engineer Intern at Intel** (May-August 2026) and **Inspur Enterprise Cloud** (June-August 2025).


I work on making AI systems faster, measurable, and reliable: heterogeneous inference, model quantization, LLM serving, and AI agents with explicit transaction and audit boundaries. I'm interested in **AI infrastructure, inference engineering, and software engineering opportunities in China and the United States**.


### Featured work


#### [Intel internship portfolio](https://github.com/tomran123/intel_cunzhou)
**OpenVINO · NNCF · ONNX Runtime · CPU / GPU / NPU**


- **PaddleOCR-VL 1.5:** built isolated benchmarks and output-validation pipelines for INT8 quantization; measured approximately **2.8x end-to-end speedup** and **27% lower memory usage** versus the uncompressed OpenVINO baseline in the reported experiments.
- **PP-OCRv6:** rebuilt preprocessing, inference, and decoding; routed dynamic-shape detection to GPU and fixed-shape recognition to NPU with CPU fallback. ONNX Runtime parity testing helped diagnose a batch-correctness bug; throughput recovered from approximately **0.5 to 5.9 FPS** compared with the initial faulty port.
- **FLUX.2-klein-4B:** brought up and profiled inference on Panther Lake, with per-stage latency, load-time, peak-memory, and version-regression tooling. In the documented 1024x1024, four-step, no-CFG test, INT4 reduced transformer peak RAM from **13.57 GB to 3.88 GB**.
- Also built a [SAM3 + LaMa object-removal demo](https://github.com/tomran123/object-removal-demo) with PyTorch/OpenVINO backends and a Gradio interface.


The portfolio contains public FLUX scripts and benchmark reports. Some linked OCR and super-resolution source repositories are private. Results are specific to the documented hardware, configurations, and test samples.


#### [WealthPortfolio](https://github.com/tomran123/wealthprofolio)
**Next.js · TypeScript · FastAPI · PostgreSQL · Celery · RabbitMQ · Redis**


A full-stack asset-management application that combines portfolio accounting with reviewable AI workflows.


- Transaction event ledger, double-entry journal postings, idempotency protection, row-level locking, and rebuildable holding projections.
- An auditable AI agent with typed tools, human confirmation and stale-state checks before mutations, and atomic multi-tool database writes.
- Asynchronous agent, market-data, and document jobs with persistent state and WebSocket updates.
- PDF/image processing, OCR, and document retrieval with page-level citations and reviewable transaction drafts.


### Additional systems experience


- **OS-vLLM:** built a vLLM Prefill-Decode serving prototype on openEuler with OpenAI-compatible routing, health monitoring, session affinity, retries, and worker recovery. Evaluated 1x1 through 2x2 worker configurations using fault injection and latency/throughput benchmarks.
- **Pintos:** implemented preemptive priority scheduling, nested priority donation, synchronization, lazy loading, swap, page-fault handling, and clock-based page replacement.
- **Inspur Enterprise Cloud:** built a hospital appointment prototype using React/TypeScript, Node.js, Express, and PostgreSQL, including JWT authentication and transactional booking-conflict detection.


### Tools I use


- **Languages:** Python, C/C++, TypeScript/JavaScript, Java, SQL
- **AI and inference:** OpenVINO, NNCF, ONNX Runtime, PyTorch, vLLM
- **Applications and systems:** FastAPI, React/Next.js, PostgreSQL, Redis, RabbitMQ, Celery, Docker, Linux


---


## 中文


我是**德克萨斯大学奥斯汀分校（UT Austin）计算机科学与数学本科生**，预计于 **2027 年 12 月毕业**。曾于 **2026 年 5-8 月在 Intel 担任软件工程实习生**，并于 **2025 年 6-8 月在浪潮企业云实习**。


我关注 AI 系统的性能、可测量性与可靠性，主要方向包括异构推理、模型量化、LLM 服务，以及具备明确事务与审计边界的 AI Agent。希望寻找**中国或美国的 AI 基础设施、推理工程及软件工程岗位**。


### 核心项目与经历


#### [Intel 实习项目集](https://github.com/tomran123/intel_cunzhou)
**OpenVINO · NNCF · ONNX Runtime · CPU / GPU / NPU**


- **PaddleOCR-VL 1.5：** 搭建独立进程基准测试与输出一致性验证流程，使用 INT8 量化；在报告所述实验中，相比未压缩 OpenVINO 基线，实现约 **2.8 倍端到端加速**和 **27% 内存下降**。
- **PP-OCRv6：** 重建预处理、推理和解码流程，将动态形状检测分配至 GPU、固定形状识别分配至 NPU，并以 CPU 回退。通过 ONNX Runtime 对齐测试定位批处理正确性问题，吞吐量从初始错误移植版本的约 **0.5 FPS 恢复至 5.9 FPS**。
- **FLUX.2-klein-4B：** 完成 Panther Lake 平台适配，搭建分阶段延迟、加载时间、峰值内存与版本回归测试。在文档所述 1024x1024、4 步、关闭 CFG 的实验中，INT4 将 Transformer 峰值 RAM 从 **13.57 GB 降至 3.88 GB**。
- 构建 [SAM3 + LaMa 目标移除演示](https://github.com/tomran123/object-removal-demo)，支持 PyTorch/OpenVINO 后端与 Gradio 界面。


项目集包含公开的 FLUX 脚本与测试报告；部分 OCR 和超分辨率源码链接指向私有仓库。性能结果对应各报告中的硬件、配置与测试样本。


#### [WealthPortfolio：全栈资产管理平台](https://github.com/tomran123/wealthprofolio)
**Next.js · TypeScript · FastAPI · PostgreSQL · Celery · RabbitMQ · Redis**


将投资组合账务与可人工复核的 AI 工作流结合的全栈应用。


- 交易事件账本、复式记账分录、幂等保护、行级锁及可重建的持仓投影。
- 类型化工具驱动的可审计 AI Agent：写操作前进行人工确认与状态过期校验，多工具写入在数据库事务中原子执行。
- Agent、行情与文档任务异步执行，保留任务状态并通过 WebSocket 更新进度。
- PDF/图片处理、OCR 与文档检索，返回页级来源引用及可复核的交易草稿。


### 其他系统工程经历


- **OS-vLLM：** 在 openEuler 上构建 vLLM Prefill-Decode 服务原型，实现 OpenAI-compatible 路由、健康监控、会话亲和、重试和 Worker 恢复；通过故障注入及延迟/吞吐量基准评估 1x1 至 2x2 Worker 配置。
- **Pintos：** 实现抢占式优先级调度、嵌套优先级捐赠、同步机制、懒加载、Swap、缺页处理和 Clock 页面置换。
- **浪潮企业云：** 使用 React/TypeScript、Node.js、Express 与 PostgreSQL 开发医院预约原型，实现 JWT 鉴权及基于事务的预约冲突检测。


### 技术栈


- **语言：** Python、C/C++、TypeScript/JavaScript、Java、SQL
- **AI 与推理：** OpenVINO、NNCF、ONNX Runtime、PyTorch、vLLM
- **应用与系统：** FastAPI、React/Next.js、PostgreSQL、Redis、RabbitMQ、Celery、Docker、Linux

