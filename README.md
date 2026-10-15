# Awesome-AI-Model-Evaluation

# Top AI Model Evaluation Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Benchmark Harnesses, LLM-as-Judge & Agent Evaluation*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Model Evaluation**. These tools enable teams to systematically measure model quality—running standardized benchmarks, scoring outputs with LLM judges, evaluating agent trajectories, and catching regressions before they reach production.

**Examples** include Scale AI, Snorkel, Braintrust, LangSmith, Arize Phoenix, Patronus AI, TruEra, Fiddler AI, Humanloop, and DeepEval (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, benchmark harnesses, and open evaluation frameworks—ideal for ML engineers, AI researchers, and developers seeking transparent, vendor-independent evaluation.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Braintrust](https://www.braintrust.dev/)**  
  **Eval-first observability platform with CI/CD quality gates.** Trusted by Notion, Stripe, Vercel, Dropbox, and Coursera. **Freemium**: Starter free (1 GB logs/month, 14-day retention, 10k eval runs/month), Pro at $249/month (5 GB, 30-day retention, 50k evals), Enterprise with self-hosted/BYOC options . **AI-assisted Loop Agent** automates optimization of prompts and evaluations.

- **[LangSmith](https://smith.langchain.com/)**  
  LangChain's observability and evaluation platform with detailed tracing of every LLM call, chain execution, and agent step. **Free Developer plan** (1 seat, 5k base traces/month), **Plus at $39/seat/month** (10k base traces, 1 free serverless deployment), Enterprise with self-hosted/hybrid options.

- **[Scale AI](https://scale.com/)**  
  Data platform for AI with annotation, curation, and model evaluation services. Features **human evaluation** at scale, **RLHF preference data collection**, and **model benchmarking** against expert graders.

- **[Snorkel Flow](https://snorkel.ai/)**  
  Enterprise data development platform built on the open-source Snorkel library. Supports **programmatic labeling**, data curation, model training, and evaluation.

- **[Patronus AI](https://www.patronus.ai/)**  
  **Hosted evaluation API with configurable evaluators** for hallucination (Lynx), toxicity, PII, prompt injection, and custom judging. Single `/v1/evaluate` endpoint runs multiple evaluators per request with pass/fail verdicts and explanations. **Free Developer tier**.

- **[Fiddler AI](https://www.fiddler.ai/)**  
  Enterprise AI observability and model performance monitoring with explainability, bias detection, and LLM evaluation. **Experiments** feature supports A/B testing prompts, model version comparison, regression testing, safety validation, and RAG system evaluation.

- **[Humanloop](https://humanloop.com/)**  
  LLM Evals Platform for Enterprises with prompt engineering, evaluation, and observability. **Free tier**: 2 members, 50 eval runs, 10K logs/month.

- **[TruEra](https://truera.com/)**  
  AI quality management platform with testing, monitoring, and explainability. **Acquired by Snowflake (2024)**.

## Open-Source GitHub Projects

- **[DeepEval](https://github.com/confident-ai/deepeval)**  
  **Simple-to-use open-source LLM evaluation framework** (Apache-2.0), similar to Pytest but specialized for unit testing LLM outputs. **The most practical open-source eval framework for CI/CD integration.** Features **large variety of ready-to-use metrics** powered by ANY LLM or local NLP models: G-Eval, Summarization, Answer Relevancy, Faithfulness, Contextual Recall, Contextual Precision, RAGAS, Hallucination, Toxicity, Bias. **Red teaming** for 40+ safety vulnerabilities with 10+ attack enhancement strategies. Evaluate entire datasets in bulk in under 20 lines of Python code in parallel. **Integrates seamlessly with ANY CI/CD environment.** Benchmarks any LLM on MMLU, HellaSwag, BIG-Bench Hard, TruthfulQA, HumanEval, GSM8K in under 10 lines of code.

- **[TruLens](https://github.com/truera/trulens)**  
  **The most comprehensive open-source evaluation and tracking framework for LLM experiments and RAG pipelines** (Apache-2.0). **3,000+ GitHub stars.** **OpenTelemetry-native**—instrument any app with a decorator, score every step with LLM judges that explain themselves, compare versions, and ship the one that earns it. **Seven purpose-built evaluators for agentic systems** (LogicalConsistency, ExecutionEfficiency, PlanAdherence, PlanQuality, ToolSelection, etc.). **Judges are graded against human annotations out of the box**: **95% agent errors caught with Agent GPA on TRAIL/GAIA** (vs 55% baseline), **0.81 Groundedness F1 on LLM-AggreFact**. Adopted by **Walmart Global Tech, Cisco, J.P. Morgan Chase, Equinix, VMware by Broadcom, Hitachi Digital Services, Thomson Reuters** .

- **[DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness)**  
  **The official open-source evaluation harness for DeepSeek models** (open-source, Python 3.12+). **The reference implementation for evaluating frontier models.** Features **live progress UI** (per-sample pass/fail dots, task progress bar, running accuracy), **built-in task suite** covering reasoning benchmarks and instruction-following evaluation, **multi-model comparison** (two models on same task suite, both accuracies plotted), **OpenAI-compatible API** with `dsh eval` CLI . **Metrics are comparable only when using the same harness on the same tasks on the same machine** —DeepSeek explicitly warns against comparing numbers from different harnesses . **Resume support** for interrupted evaluations. **The canonical harness for reproducible model evaluation.**

- **[Arize Phoenix](https://github.com/Arize-ai/phoenix)**  
  **Open-source AI observability platform** (Elastic License 2.0) designed for experimentation, evaluation, and troubleshooting. Features **tracing** via OpenTelemetry-based instrumentation, **evaluation** using LLMs to benchmark performance, **datasets** for versioned examples, **experiments** for tracking prompt/model/retrieval changes, **playground** for prompt optimization and model comparison, and **prompt management** with version control. **2.5M+ monthly downloads**, **10,800+ GitHub stars**.

- **[Ragas](https://github.com/vibrantlabsai/ragas)**  
  **The leading open-source RAG evaluation framework** (Apache-2.0). Features **objective metrics** (LLM-based and traditional), **test data generation**, **seamless integrations** with LangChain and major observability tools, and **feedback loops** leveraging production data. CLI quickstart: `ragas quickstart rag_eval` creates complete RAG evaluation project.

- **[Promptfoo](https://github.com/promptfoo/promptfoo)**  
  **Open-source LLM testing and red-teaming framework** (MIT). **20,000+ GitHub stars.** Listed as one of five tools people actually use for LLM evaluation alongside Braintrust, LangSmith, Inspect, and Ragas.

- **[Inspect](https://github.com/UKGovernmentBEIS/inspect_ai)**  
  **Open-source framework for large language model evaluations from UK AI Safety Institute**. **The most authoritative open-source evaluation framework from a government AI safety body.**

- **[AgentCompass](https://github.com/open-compass/AgentCompass)**  
  **Unified open-source evaluation infrastructure for agents** (Apache-2.0, EMNLP 2026 Demo Track). **30+ public benchmarks and 10+ agent harnesses** including Claude Code, Codex, OpenHands, and OpenClaw. **Composable architecture** decouples Model, Benchmark, Harness, and Environment. **Traceable and reproducible** with trajectory recording, tool calls, and failure analysis.

- **[ContextForge Eval](https://pypi.org/project/contextforge-eval/)**  
  **Open-source evaluation framework for agentic systems**. **Framework-agnostic**—adapters translate framework events into traces, graders operate only on traces. **Memory hygiene detection** catches stale context, missed facts, and contradictory fragments.

- **[Langfuse](https://github.com/langfuse/langfuse)**  
  **Open-source LLM engineering platform** (MIT core) with tracing, evaluations, prompt management, and datasets. **35,000+ GitHub stars**. Self-hostable. **Acquired by ClickHouse in January 2026 with commitment to keep it open source**.

- **[Comet Opik](https://github.com/comet-ml/opik)**  
  **Fully-permissive Apache-2.0 rival to Langfuse**. **22,000+ GitHub stars**. Full platform—backend included—free to self-host.

- **[OpenAI Evals](https://github.com/openai/evals)**  
  **Open-source framework for evaluating LLMs and LLM systems** (MIT). The original evaluation framework from OpenAI.

- **[LM Evaluation Harness (EleutherAI)](https://github.com/EleutherAI/lm-evaluation-harness)**  
  **The standard open-source harness for evaluating language models on academic benchmarks** (MIT). **Used by Hugging Face Open LLM Leaderboard, BigScience, and countless research papers.** Features 60+ standard academic benchmarks (MMLU, HellaSwag, GSM8K, TruthfulQA, etc.), multi-GPU support, and reproducible evaluations.

### Additional Strong Open-Source Options

- **[Helm (Stanford CRFM)](https://github.com/stanford-crfm/helm)** — Holistic Evaluation of Language Models (Apache-2.0). **The most comprehensive academic evaluation framework** covering accuracy, calibration, robustness, fairness, bias, toxicity, and efficiency across 30+ scenarios.
- **[BIG-bench](https://github.com/google/BIG-bench)** — Beyond the Imitation Game benchmark (Apache-2.0). **204 tasks contributed by 450 authors** covering reasoning, knowledge, and capabilities.
- **[clean-evals](https://pypi.org/project/clean-evals/)** — Open-source eval platform with blind review, golden answer locking, and LLM judge calibration.
- **[OpenAI Cookbook](https://github.com/openai/openai-cookbook)** — Includes evaluation recipes and patterns.
- **[Anthropic Cookbook](https://github.com/anthropics/anthropic-cookbook)** — Includes evaluation recipes and patterns for Claude applications.
- **[LLM-as-a-Judge](https://github.com/lm-sys/llm-as-a-judge)** — Research implementations for using LLMs to evaluate LLMs.
- **[AlpacaEval](https://github.com/tatsu-lab/alpaca_eval)** — Automatic evaluator for instruction-following models.
- **[FastChat (LMSYS)](https://github.com/lm-sys/FastChat)** — Includes MT-Bench and Chatbot Arena evaluation.
- Community **n8n** workflows for evaluation pipeline automation and regression alerting.

**Frameworks for building custom systems**: Combine **DeepEval** for CI/CD-integrated testing with **TruLens** for comprehensive experiment tracking, **DeepSeek Harness** for reproducible model benchmarking, **Arize Phoenix** for OpenTelemetry-native tracing, **Ragas** for RAG-specific metrics, and **AgentCompass** for agent evaluation—creating a fully self-hosted, enterprise-grade AI model evaluation platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- AI evaluation platforms handling prompts and traces must comply with data protection regulations (GDPR, CCPA, etc.), especially when traces contain PII.
- **Metrics are comparable only when using the same harness on the same tasks on the same machine.** DeepSeek explicitly warns: "跨 harness 或机器的数字不可比" (numbers across different harnesses or machines are not comparable) . **Always report the harness, task suite, and hardware configuration alongside results.**
- **"Open source" means different things in this category.** DeepEval, TruLens, Ragas, Promptfoo, Inspect, LM Evaluation Harness, and Helm are genuinely open source (Apache-2.0/MIT). Arize Phoenix uses Elastic License 2.0 (source-available, not OSI-approved). LangSmith is closed SaaS with open SDKs. **Check the LICENSE file, not the marketing page** .
- **Observability is not evaluation.** Tracing tells you what happened; evaluation tells you whether it was good. Most tools ship both—which makes it easy to buy one and never configure the other. **Tracing alone will not catch quality drift.**
- **Evaluation judges are themselves LLMs.** Their scores are probabilistic and should be validated against human annotations for high-stakes decisions. TruLens grades its judges against human annotations out of the box—a practice every evaluation deployment should follow .
- **Agent evaluation is fundamentally harder than model evaluation.** Agents take multi-step actions, use tools, and make decisions under uncertainty. AgentCompass and ContextForge Eval address this with trajectory recording, failure analysis, and memory hygiene detection. **Traditional single-turn benchmarks are insufficient.**
- Self-hosted open-source solutions require proper security hardening, LLM infrastructure (or API keys), and ongoing maintenance. Evaluation is infrastructure—budget for it accordingly.

---

**Made for ML engineers, AI researchers, and developers building transparent AI model evaluation solutions.**  
Let's make AI Model Evaluation more open, data-driven, and reproducible.
