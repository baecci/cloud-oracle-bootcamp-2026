# 병원 QA/QI 담당자를 위한 의료분쟁 판례 기반 검색, 통계 보조 에이전트

병원 QA/QI 담당자를 위해, 특정 진료과나 시술 시 발생할 수 있는 주요 분쟁사건 요인을 분석하고 예방할 수 있는 체크리스트를 작성해주는 AI Agent를 설계합니다. 
*클라우드 기반 AI 파이프라인 구축 강의에서 진행한 프로젝트의 레포지토리입니다.*

## 사용한 주요 기술
- Python / Oracle Cloud / RAG / LangChain / FastAPI + Uvicorn / PostgreSQL + PGVector / Claude Code

## 실행 방법
*오라클 클라우드의 VM Instance와 Object Storage, OpenAI API가 있어야 합니다*

ingest.py 실행하여 데이터를 로드, 저장하고 다음 명령어를 통해 서버를 실행합니다.

uvicorn web:app --host 0.0.0.0 --port 8000
