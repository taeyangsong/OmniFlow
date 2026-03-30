<div align="center">

<img src="https://via.placeholder.com/1280x500/0F172A/60A5FA?text=TaskFlow&font=Inter" alt="TaskFlow Banner" width="100%" />

# TaskFlow

**팀과 개인의 생산성을 극대화하는 현대적인 업무 관리 플랫폼**

실시간 협업, 직관적인 UI, 강력한 자동화까지.  
개발자, 디자이너, PM 모두가 사랑하는 **차세대 태스크 매니저**.

![GitHub stars](https://img.shields.io/github/stars/taeyang-dev/taskflow?style=for-the-badge&logo=github&color=0ea5e9)
![GitHub forks](https://img.shields.io/github/forks/taeyang-dev/taskflow?style=for-the-badge&logo=github)
![License](https://img.shields.io/github/license/taeyang-dev/taskflow?style=for-the-badge)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white)

</div>

<br>

## ✨ 주요 기능

- **실시간 협업** — 여러 명이 동시에 같은 보드를 편집
- **AI 스마트 어시스턴트** — 작업 자동 분류, 마감일 예측, 요약 생성
- **Kanban + List + Timeline + Calendar** — 4가지 뷰 완벽 지원
- **강력한 자동화** — If-Then 규칙 기반 워크플로우
- **통합** — Slack, Notion, GitHub, Google Calendar 연동
- **모바일 완벽 지원** — PWA + 네이티브 앱 느낌

## 📸 스크린샷

<div align="center">
  <img src="https://via.placeholder.com/800x480/1E2937/60A5FA?text=Dashboard+Preview" width="49%" alt="Dashboard" />
  <img src="https://via.placeholder.com/800x480/1E2937/60A5FA?text=Kanban+Board" width="49%" alt="Kanban" />
  <img src="https://via.placeholder.com/800x480/1E2937/60A5FA?text=AI+Assistant" width="49%" alt="AI Assistant" />
  <img src="https://via.placeholder.com/800x480/1E2937/60A5FA?text=Timeline+View" width="49%" alt="Timeline" />
</div>

<br>

## 🛠 기술 스택

| Layer           | Technology                              |
|----------------|-----------------------------------------|
| **Frontend**   | Next.js 15 (App Router), TypeScript, Tailwind CSS, shadcn/ui, Zustand, TanStack Query |
| **Backend**    | Next.js API Routes + tRPC               |
| **Database**   | PostgreSQL + Prisma ORM                 |
| **Auth**       | NextAuth.js (OAuth + Credentials)       |
| **AI**         | OpenAI GPT-4o + LangChain               |
| **Real-time**  | Pusher / Socket.io                      |
| **Deployment** | Vercel + Neon Postgres                  |
| **CI/CD**      | GitHub Actions                          |

## 🚀 빠른 시작

```bash
# 1. 저장소 클론
git clone https://github.com/taeyang-dev/taskflow.git
cd taskflow

# 2. 의존성 설치
pnpm install

# 3. 환경 변수 설정
cp .env.example .env.local

# 4. 데이터베이스 마이그레이션
pnpm prisma migrate dev

# 5. 개발 서버 실행
pnpm dev
