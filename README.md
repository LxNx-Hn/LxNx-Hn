# 문종건

문제를 작은 단위로 구조화하고, 데이터·AI·Cloud를 조합해 실제로 동작하는 서비스 형태까지 구현합니다.

설계와 판단은 직접 하고, 범위가 명확한 구현에는 AI를 활용한 뒤 코드·테스트·로그를 다시 확인합니다.

[Portfolio](https://lxnx-hn.github.io/) · [GitHub](https://github.com/LxNx-Hn) · [Email](mailto:lxnx.kiki@gmail.com)

## Selected projects

| Project | What I worked on |
| --- | --- |
| [동넷](https://github.com/LxNx-Hn/KT-10) | 부산 이동취약자 맞춤 경로 추천, TMAP 누락 버스의 BIMS 보완, 다중 공급원 경로 병합, 후보 재평가와 철도 데이터 정합성 |
| [동성로 창업지원 RAG 챗봇](https://github.com/LxNx-Hn/chatbot-with-kt-dgucenter) | 질문 category와 데이터 source를 연결하는 RAG 상담 구조, FastAPI–React 연결, Cloud Run·Netlify 배포와 secret·비용 설정 |
| [Hot's POD](https://github.com/LxNx-Hn/Hot-s-Pod) | Keyword·Vector·RDB 하이브리드 검색, similarity 정렬 복원, 계층형 댓글 transaction, React Query 상태 동기화 |
| [M_RAG](https://github.com/LxNx-Hn/M_RAG) | 한국어 질문·영어 논문 RAG에서 HyDE·CAD·SCD 비교, null 결과 보존, RAGAS 복구와 실험 provenance 관리 |
| [AI_FinalTerm](https://github.com/LxNx-Hn/AI_FinalTerm) | Unity ML-Agents PPO의 action space·reward·action mask를 50K 학습 로그와 코드로 반복 개선 |

## How I work

1. 사용자의 문제와 제약조건을 먼저 정의합니다.
2. input·output·state·interface를 나눠 작은 단위로 설계합니다.
3. 범위가 명확한 반복 구현은 AI에 위임합니다.
4. 생성된 코드의 상태 변화와 side effect를 직접 읽습니다.
5. test·build·API·log·실제 데이터로 결과를 확인합니다.
6. 문제가 남은 함수만 다시 좁혀 수정합니다.

AI 또는 bot이 작성에 참여한 커밋은 직접 구현과 섞지 않고 공동작성 이력을 구분해 설명합니다.

## Stack used in public projects

- **Languages**: Python · TypeScript · JavaScript · C#
- **Backend**: FastAPI
- **Frontend**: React · Vite · TanStack Query
- **AI / Data**: PyTorch · Transformers · Sentence Transformers · ChromaDB · RAGAS · Unity ML-Agents · PPO
- **Database**: PostgreSQL · MariaDB
- **Cloud / Ops**: Docker · GitHub Actions · AWS ECS · GCP Cloud Run · Secret Manager · Netlify

위 목록은 공개 저장소의 코드와 본인 작성 또는 명시적 공동작성 커밋에서 확인되는 기술만 정리했습니다.
