# react-gpt-memoir

AI 회고록 서비스 – GPT 기반 심리상담사 회고 작성 도우미  
React + OpenAI GPT API 기반 Web Application

## 🧠 서비스 개요

**문제**  
많은 사람들이 SNS/블로그에 회고록을 남기고 싶어하지만,  
글을 쓰는 것이 어렵고 회고 자체를 귀찮아합니다.

**가설**  
GPT가 글쓰기를 도와주고, 심리 분석 및 액션리스트까지 제공한다면  
더 높은 퀄리티의 회고와 자기 성장을 도울 수 있습니다.

**해결 방법**  
간단한 문장을 입력하면, AI가 회고록을 자동 생성하는 웹 서비스 개발

---

## 🚀 개발 진행 순서

1. ChatGPT에서 프롬프트 실험 및 최적화
2. OpenAI API Key 발급 및 연동
3. GPT API 호출 구조 구성  
   - **System**: 역할 설명 및 전제 설정 (예: "너는 심리상담사야")  
   - **User**: 사용자의 입력  
   - **Assistant**: 이전 대화를 바탕으로 이어쓰기 등

4. 주요 기능 개발
   - 사용자 입력 처리
   - GPT 응답 결과 렌더링
   - 스타일 구성 및 UI 개선 (antd + styled-components)

---

## 🛠 기술 스택

- **Frontend**: React, Vite
- **Styling**: styled-components, Ant Design
- **AI**: OpenAI GPT API

---

## ✅ 구현 체크리스트

- [ ] React 설치
- [ ] `styled-components`, `antd`, `@ant-design/icons` 설치
- [ ] 기본 예제 (카운터): `useState`, 이벤트 핸들링
- [ ] GPT API Key 발급 및 `.env` 설정
- [ ] API 호출 구현 (System/User 역할 구분)
- [ ] 사용자 입력 폼 개발
- [ ] 스타일 구성 (antd + styled-components)
- [ ] 리팩토링: 로딩, 아이콘, 에러 메시지 처리

---

## ⚠️ 주의사항

- OpenAI API 사용은 **유료**입니다.  
  👉 하루 사용량 제한 필요
- API Key는 **절대 공개 저장소에 업로드 금지**  
  👉 `.env` 파일과 `.gitignore` 설정 필수

---

## 📁 프로젝트 구조 (예시)
react-gpt-memoir/
├── public/
├── src/
│ ├── components/
│ ├── api/
│ ├── pages/
│ ├── styles/
│ └── App.jsx
├── .env
├── .gitignore
├── package.json
└── README.md

---

## 📌 향후 개선 아이디어

- 회고 결과 다운로드 기능
- 주간/월간 회고 리포트
- 다중 프롬프트 템플릿 제공
- 감정 변화 추적 그래프
