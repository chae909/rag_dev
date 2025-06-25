# 소득세 챗봇 프로젝트

이 프로젝트는 소득세 관련 질문에 대해 AI가 답변해주는 챗봇 및 RAG(Retrieval-Augmented Generation) 기반 문서 검색 시스템입니다.

## 주요 기능

- Streamlit 기반 웹 챗봇 UI 제공
- LangChain, OpenAI, Pinecone를 활용한 문서 임베딩 및 검색
- `.docx` 세법 문서로부터 자동 청킹 및 벡터화
- 사용자 질문에 맞는 답변 생성 및 사전 기반 질문 변환

## 폴더 구조

- `app.py` : Streamlit 챗봇 웹앱
- `llm.py` : LLM 및 RAG 체인 관련 함수
- `config.py` : 예시 질문/답변 등 설정
- `requirements.txt` : 필수 패키지 목록
- `tax.docx` : 세법 문서
- `01_tax_rag.ipynb`, `01_tax_rag_copy.ipynb` : RAG 실험/구현 노트북
- `tests/` : 테스트 코드

## 설치 및 실행 방법

1. Python 3.11+ 환경 준비
2. 필수 패키지 설치
   ```bash
   pip install -r requirements.txt
   ```
3. 환경 변수 파일(.env)에 OpenAI, Pinecone API 키 등 입력
4. Streamlit 앱 실행
   ```bash
   streamlit run app.py
   ```

## 사용 예시

- "연봉 5천만원인 거주자의 종합소득세는?"
- "소득세의 과세 기간은 어떻게 되나요?"

## 참고

- LangChain, OpenAI, Pinecone 공식 문서
- 프로젝트 내 Jupyter 노트북 참고
