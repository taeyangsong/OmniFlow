<div align="center">

![Helix Banner](https://picsum.photos/id/1015/1280/480)

# Helix

**오픈소스 멀티에이전트 지능 인프라**

**인간 수준의 협업 지능을 모든 개발자와 연구자에게.**

단일 LLM을 넘어, **수십 개의 전문 에이전트가 실시간으로 협력**하는 차세대 AI 시스템의 기반을 만듭니다.  
LangGraph + AutoGen + CrewAI의 장점만 취하고, 그 이상을 목표로 합니다.

![Stars](https://img.shields.io/github/stars/taeyang-dev/helix?style=for-the-badge&color=0ea5e9)
![License](https://img.shields.io/github/license/taeyang-dev/helix?style=for-the-badge)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![AI](https://img.shields.io/badge/Agentic_AI-10b981?style=for-the-badge)

</div>

<br>

## ✨ Helix가 해결하는 문제

- **Fragmented Agent Ecosystem** — LangChain, CrewAI, AutoGen 등이 서로 호환되지 않음
- **Evaluation Hell** — 에이전트 성능을 신뢰할 수 있는 표준 벤치마크 부족
- **Real-world Reliability** — hallucination, tool misuse, coordination failure
- **Vendor Lock-in** — OpenAI, Anthropic, Grok, Claude 등 모델을 자유롭게 오케스트레이션 불가

**Helix는 모든 AI 회사가 공통으로 사용할 수 있는 오픈 인프라**가 되는 것을 목표로 합니다.

## 🚀 핵심 기능

- **Graph-based Multi-Agent Orchestration** (LangGraph 스타일 + CRDT 실시간 협업)
- **Universal Agent Protocol** — 어떤 LLM이든, 어떤 프레임워크든 연결 가능
- **Advanced Evaluation Suite** — GAIA, WebArena, AgentBench 등 통합 벤치마크 + 커스텀
- **Safety & Alignment Layer** — Constitutional AI, Guardrails, Red-teaming 도구 내장
- **Observability & Debugging** — LangSmith + Phoenix 수준의 tracing (오픈소스)
- **Synthetic Data & Self-Improvement Loop** — 에이전트가 스스로 학습
- **Self-host & Enterprise Ready** — Docker, Kubernetes, Air-gapped 지원

## 📸 Helix in Action

<div align="center">
  <img src="https://picsum.photos/id/1015/850/480" width="49%" alt="Multi-Agent Dashboard" />
  <img src="https://picsum.photos/id/106/850/480" width="49%" alt="Agent Collaboration Graph" />
  <img src="https://picsum.photos/id/201/850/480" width="49%" alt="Evaluation Arena" />
  <img src="https://picsum.photos/id/237/850/480" width="49%" alt="Safety Guardrails" />
</div>

## 🛠 기술 스택

- **Core** — TypeScript + Python (Monorepo, Turborepo)
- **Orchestration** — Custom Graph Engine + Liveblocks (real-time)
- **Models** — OpenAI, Anthropic, Grok, Llama, Mistral, Gemini (agnostic)
- **Vector & Memory** — PgVector, Qdrant, Chroma
- **Evaluation** — Custom + Hugging Face Evaluate integration
- **Infra** — Docker Compose, Kubernetes, Helm
- **UI** — Next.js 15 + shadcn/ui + Recharts + React Flow

## 🚀 빠른 시작

```bash
# Docker로 1분 만에 실행 (추천)
docker compose up -d

# 또는 소스 빌드
git clone https://github.com/taeyang-dev/helix.git
cd helix
pnpm install
pnpm dev
