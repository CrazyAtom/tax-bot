# 소득세법 챗봇 (Tax-Bot)

## 프로젝트 소개

소득세법 관련 질의응답을 제공하는 AI 챗봇 서비스입니다. LangChain과 OpenAI를 활용하여 정확하고 신뢰할 수 있는 소득세법 정보를 제공합니다.

## 주요 기능

- 소득세법 관련 질의응답
- 대화 이력 기반의 맥락 이해
- 법률 용어 자동 변환
- 실시간 스트리밍 응답

## 기술 스택

- **프레임워크**: Streamlit
- **AI/ML**:
  - LangChain
  - OpenAI (GPT-4, Text Embedding 3)
- **벡터 데이터베이스**: Pinecone
- **언어**: Python 3.x

## 설치 방법

1. 저장소 클론

```bash
git clone https://github.com/CrazyAtom/tax-bot.git
cd tax-bot
```

2. 가상환경 생성 및 활성화

```bash
python -m venv venv
source venv/bin/activate  # Mac/Linux
```

3. 의존성 설치

```bash
pip install -r requirements.txt
```

4. 환경변수 설정

```bash
# .env 파일 생성
OPENAI_API_KEY=your_api_key
PINECONE_API_KEY=your_api_key
PINECONE_ENVIRONMENT=your_environment
```

## 실행 방법

```bash
streamlit run chat.py
```

## 프로젝트 구조

```
tax-bot/
├── chat.py          # Streamlit UI 구현
├── llm.py           # LangChain 및 AI 로직
├── config.py        # 설정 파일
├── requirements.txt # 의존성 목록
└── .env            # 환경변수 파일
```

## 주요 컴포넌트

- **chat.py**: Streamlit을 활용한 대화형 UI 구현
- **llm.py**: LangChain 기반의 RAG 시스템 구현
- **config.py**: 시스템 설정 및 상수 정의

## 라이센스

MIT License

## 기여 방법

1. Fork the Project
2. Create your Feature Branch
3. Commit your Changes
4. Push to the Branch
5. Open a Pull Request

## 연락처

- 이메일: your.email@example.com
- GitHub: [@CrazyAtom](https://github.com/CrazyAtom)

---

**참고**: 이 프로젝트는 학습 및 연구 목적으로 제작되었으며, 실제 법률 자문을 대체할 수 없습니다.
