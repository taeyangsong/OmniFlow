# Priority Guard

> 계획을 세우는 앱이 아니라, **계획을 지키는 앱**

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.111-green.svg)](https://fastapi.tiangolo.com/)
[![Claude API](https://img.shields.io/badge/Claude-Haiku%204.5-8A2BE2.svg)](https://www.anthropic.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 왜 만들었나

아침에 오늘 할일을 정리해도, 슬랙과 이메일로 새 요청이 쏟아지면 계획이 무너집니다.
기존 Todo 앱은 **목록 관리**만 할 뿐, *"이 요청, 지금 해야 하나?"* 는 매번 내가 판단해야 합니다.

Priority Guard는 새 요청이 들어올 때 기존 목록과 비교해 AI가 대신 판단해줍니다.

---

## 주요 기능

### 할일 관리
- 우선순위와 함께 오늘 할일 등록 · 완료 · 삭제
- **더블클릭**으로 제목 인라인 편집
- **드래그 앤 드롭**으로 순위 재배치
- 어제 미완료 항목 한 번에 오늘로 가져오기

### AI 새 요청 판단
갑자기 들어온 요청을 입력하면 Claude AI가 기존 할일 목록과 비교해 세 가지 중 하나로 판단합니다.

| 판단 | 의미 |
|---|---|
| 🔴 지금 끼워넣기 | 현재 진행 중인 작업보다 우선. 지정 순위에 자동 삽입 + 기존 항목 밀기 |
| 🔵 나중에 처리 | 오늘 중 처리하되 현재 순위보다 낮음. 목록 맨 뒤 추가 |
| ⚪ 오늘 안 해도 됨 | 내일로 미루거나 위임 가능 |

### 주간 통계 & 하루 요약
- 최근 7일 완료율 막대 차트
- AI가 오늘 완료/미완료를 분석해 하루 평가 + 내일 조언 생성

---

## 시작하기

**요구사항:** Python 3.10+ · [Anthropic API Key](https://console.anthropic.com/)

```bash
# 1. 의존성 설치
pip install -r requirements.txt

# 2. 환경변수 설정
cp .env.example .env
# .env 파일에 ANTHROPIC_API_KEY=your_key 입력

# 3. 서버 실행
python run.py
```

브라우저에서 **http://localhost:8000** 접속
API 문서는 **http://localhost:8000/docs**

---

## 프로젝트 구조

```
OmniFlow/
├── CLAUDE.md              # AI 개발 지침 & 코딩 컨벤션
├── CHANGELOG.md           # 버전별 변경 이력
├── app/
│   ├── main.py            # FastAPI 앱 진입점
│   ├── database.py        # SQLite 설정
│   ├── models.py          # Task 모델
│   └── routers/
│       ├── tasks.py       # 할일 CRUD + reorder / carry-over / stats
│       └── ai.py          # AI 판단 + 하루 요약
├── static/
│   ├── index.html
│   ├── style.css
│   └── app.js
├── docs/
│   ├── architecture.md    # 시스템 설계
│   ├── api.md             # API 레퍼런스
│   └── dev-guide.md       # 개발 가이드
├── run.py
├── requirements.txt
└── .env.example
```

---

## 기술 스택

| 영역 | 기술 |
|---|---|
| Backend | FastAPI · SQLAlchemy · SQLite |
| AI | Claude Haiku 4.5 (Anthropic) |
| Frontend | Vanilla JS · CSS (프레임워크 없음) |

---

## 문서

- [시스템 설계](docs/architecture.md)
- [API 레퍼런스](docs/api.md)
- [개발 가이드](docs/dev-guide.md)
- [변경 이력](CHANGELOG.md)

---

## License

MIT
