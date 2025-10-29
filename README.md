# ai_chatbot
# Wikipedia AI Chatbot

Wikipedia 문서를 검색·요약해 대화형으로 답하는 간단한 챗봇 예제.

## 주요 기능
- MediaWiki API로 위키 문서 검색/요약
- 간단한 컨텍스트 재구성(RAG-lite)
- FastAPI HTTP 엔드포인트(`/chat`)
- CLI 예제

## 빠른 시작
```bash
python -m venv .venv && source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env  # 필요한 경우 키/환경설정 입력
uvicorn app.main:app --reload
