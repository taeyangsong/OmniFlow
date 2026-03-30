<div align="center">

![TaskFlow Banner](https://picsum.photos/id/1015/1280/420)

# TaskFlow

**개발자 중심의 직관적이고 강력한 오픈소스 태스크·프로젝트 관리 도구**

Linear의 속도감 + Notion의 유연함 + GitHub Projects의 협업성을 하나로 합쳤습니다.  
실시간 협업, AI 지원, 그리고 완전한 오픈소스.

![GitHub Stars](https://img.shields.io/github/stars/taeyang-dev/taskflow?style=for-the-badge&color=10b981)
![GitHub License](https://img.shields.io/github/license/taeyang-dev/taskflow?style=for-the-badge)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white)

</div>

<br>

## ✨ 왜 TaskFlow인가?

- **빠르고 가벼움** — Linear 수준의 부드러운 UX
- **실시간 협업** — 여러 팀원이 동시에 작업해도 충돌 없음
- **AI 지원** — 자연어로 작업 생성, 우선순위 자동 추천, 요약
- **유연한 뷰** — Kanban, List, Timeline, Calendar, Spreadsheet
- **자체 호스팅 완벽 지원** — Docker 한 줄로 설치 가능
- **확장성** — Plugin 시스템 + Open API

## 📸 스크린샷

<div align="center">
  <img src="https://picsum.photos/id/1015/800/450" alt="Dashboard" width="49%" />
  <img src="https://picsum.photos/id/106/800/450" alt="Kanban Board" width="49%" />
  <img src="https://picsum.photos/id/201/800/450" alt="Timeline View" width="49%" />
  <img src="https://picsum.photos/id/237/800/450" alt="AI Command" width="49%" />
</div>

<br>

## 🛠 기술 스택

- **Frontend** — Next.js 15 (App Router) + TypeScript + Tailwind CSS + shadcn/ui
- **Backend** — tRPC + Prisma
- **Database** — PostgreSQL (Neon / Supabase 지원)
- **Auth** — NextAuth.js + Magic Link
- **Real-time** — Liveblocks 또는 Pusher
- **AI** — OpenAI GPT-4o (선택)
- **배포** — Docker + Vercel / Railway / Self-host

## 🚀 빠른 설치 (Docker)

```bash
docker run -d \
  -p 3000:3000 \
  -e DATABASE_URL="postgresql://..." \
  ghcr.io/taeyang-dev/taskflow:latest
