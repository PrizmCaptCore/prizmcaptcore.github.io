---
title: "Relay — AI 회의 인텔리전스 (익명화)"
tags:
  - AI
  - Real-time STT
  - vLLM
  - Rust / Tauri
  - Django
  - LLMOps
tech_stack: "Rust, Tauri, Next.js/React, vLLM, NeMo, PyTorch, Django, DRF, Celery, AWS ECS/CloudFront"
status: "제품 개발 (Product) 🟢"
github_url: "https://github.com/PrizmCaptCore/portfolio"
case_study_url: "/relay/"
order: 0
---

실시간 회의 인텔리전스 제품을 **혼자서 전 계층** 설계·구현했습니다 — 회의를 실시간 전사하고,
요약·결정·액션을 뽑아 검색 가능한 지식으로 만드는 제품입니다. (제품/조직명은 익명화 처리)

- **데스크톱(실시간 STT)**: Tauri(Rust) + 온디바이스 CTC partial + 클라우드 최종 전사, VAD·채널 분리 — 동시 150 세션 검증
- **GPU 서빙**: vLLM 요약/임베딩/번역, duty cycle 기반 always-on / scale-to-zero 로 idle 비용 제거
- **커스텀 ASR**: Parakeet 영어 encoder 이식 + 2단계 학습으로 한국어 CTC 모델
- **웹 플랫폼**: Django/DRF/Celery/React, ECS/CloudFront, 마이그레이션 경계를 지키는 아키텍처 테스트
- **지식그래프**: LLM(좁은 판단) + 결정론적 규칙으로 회의 사건 그래프 증분 빌드, 결정 reversal 자동 감지

**→ 자세한 케이스 스터디는 아래 "케이스 스터디 보기" 버튼**에서 확인하실 수 있습니다.
