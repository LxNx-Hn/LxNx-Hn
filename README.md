# 문종건

일단 해보고, 왜 안 되는지는 끝까지 보는 개발자입니다.

공식 문서를 보다가 생각보다 할 만하면 직접 짜봅니다. 모르는 건 모른다고 적어두고, AI가 만든 코드는 직접 다시 읽고 돌립니다. 잘됐다는 말보다 어떤 조건에서 됐는지, 아직 확인하지 못한 건 뭔지를 코드·테스트·로그로 남기려고 합니다.

> 왜 안 될까 → 기준점을 잡고 → 직접 돌려보고 → 더 간단한 코드가 있는지 다시 보기

예전 코드 주석에서 가져온 표현을, 제가 문제를 다룰 때 따르는 순서로 정리했습니다.

[Portfolio](https://lxnx-hn.github.io/) · [GitHub](https://github.com/LxNx-Hn) · [Email](mailto:lxnx.kiki@gmail.com)

## 지금까지 손댄 것들

| Project | What I worked on |
| --- | --- |
| [동넷](https://github.com/LxNx-Hn/KT-10) | TMAP에 빠진 부산 직행 버스를 BIMS로 보완하고, 공급원마다 달랐던 경로를 다시 합쳤습니다. 확인할 수 없는 시간과 geometry는 0이나 실제 경로인 것처럼 만들지 않았습니다. |
| [동성로 창업지원 RAG 챗봇](https://github.com/LxNx-Hn/chatbot-with-kt-dgucenter) | 질문 category와 LLM 분류를 대조한 뒤 맞는 데이터 source로 보내는 흐름을 잡고, FastAPI부터 Cloud Run·Netlify까지 이어 붙였습니다. |
| [Hot's POD](https://github.com/LxNx-Hn/Hot-s-Pod) | 벡터 검색 다음에 RDB filtering을 붙이고, filtering 뒤 사라진 similarity 순서를 다시 복원했습니다. 댓글·권한·React Query 상태도 서버와 맞췄습니다. |
| [M_RAG](https://github.com/LxNx-Hn/M_RAG) | RAGAS의 결측 평가 셀은 0으로 대체하지 않고 complete-case·null=0·null=1로 민감도를 나눠 봤습니다. penalty_additive SCD v1의 순효과가 없다는 결과와 reference_scd의 한국어 준수 개선, 아직 확정할 수 없는 RAG 품질 효과도 따로 기록했습니다. |
| [AI_FinalTerm](https://github.com/LxNx-Hn/AI_FinalTerm) | 학습량을 늘리기 전에 50K 로그를 보고 action space를 MultiDiscrete로 바꾸면서 mask를 새 branch 구조에 맞췄고, 다음 실험에서 reward farming을 제거했습니다. 대표 3개 커밋은 모두 Claude Opus 4.8 공동작성이고, 구조 개선과 실제 성능 개선은 따로 판단했습니다. |

## 일하는 방식

1. 왜 안 되는지부터 적습니다.
2. input·output·state로 쪼개고, 정상과 실패를 가를 기준점을 잡습니다.
3. 공식 문서를 보고 직접 붙여봅니다.
4. AI에는 입출력·변경 범위·검증 기준을 먼저 정한 단위로 맡깁니다.
5. test·build·API·log·실제 데이터로 확인하고, 측정하지 않은 값은 0으로 만들지 않습니다.

Copilot이나 Claude 공동작성 이력이 있는 커밋은 단독 구현과 섞지 않고 따로 적습니다.

## 공개 코드에서 확인되는 스택

- **Languages**: Python · TypeScript · JavaScript · C#
- **Backend**: FastAPI
- **Frontend**: React · Vite · TanStack Query
- **AI / Data**: PyTorch · Transformers · Sentence Transformers · ChromaDB · RAGAS · Unity ML-Agents · PPO
- **Database**: PostgreSQL · MariaDB
- **Cloud / Ops**: Docker · GitHub Actions · AWS ECS · GCP Cloud Run · Secret Manager · Netlify

배지 개수를 늘리기보다, 공개 저장소에서 실제로 확인되는 기술만 남겼습니다.
