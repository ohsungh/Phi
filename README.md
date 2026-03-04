# PhiMir 기획 Tools

게임 및 작업물 기획서 작성을 도와주는 AI 기반 웹 도구입니다.

## ✨ 주요 기능

### 📝 3가지 기획서 템플릿
- **기본 기획안**: 배경, 장르, 스토리라인, 캐릭터, 출시 정보 등
- **화면구상**: 씬 구성, 컷씬, 대사, 게임플레이 노트, 엔딩 분기
- **밸런스 기획**: 플레이어 스탯, 스킬, 적 유닛, 보스 패턴, 아이템

### 🤖 AI 어시스턴트 (Gemini)
- 세계관 확장 제안
- 게임플레이 아이디어
- 밸런스 분석
- 대사 생성
- 내용 개선

### 💾 파일 관리
- **Markdown (.md)** 내보내기/불러오기
- **JSON** 백업/복원
- 자동 저장 (LocalStorage)

## 🚀 배포 방법

### Cloudflare Pages

1. 이 저장소를 Fork 또는 Push
2. [Cloudflare Pages](https://pages.cloudflare.com/)에서 새 프로젝트 생성
3. GitHub 연결 후 저장소 선택
4. 빌드 설정:
   - **Framework preset**: `None`
   - **Build command**: `npm run build`
   - **Build output directory**: `dist`
5. 배포!

### 로컬 개발

```bash
# 설치
npm install

# 개발 서버
npm run dev

# 빌드
npm run build
```

## 🔑 Gemini API 키 발급

1. [Google AI Studio](https://aistudio.google.com/apikey) 방문
2. "Get API Key" 클릭
3. 새 API 키 생성
4. PhiMir 기획 Tools에서 API 키 입력

## 🛠 기술 스택

- **Frontend**: React 19 + Vite
- **Styling**: Tailwind CSS 4
- **Icons**: Lucide React
- **Markdown**: react-markdown + remark-gfm
- **PDF**: jspdf + html2canvas
- **AI**: Google Gemini API

## 📁 프로젝트 구조

```
src/
├── components/
│   ├── ApiKeyModal.jsx   # API 키 입력 모달
│   ├── Header.jsx        # 상단 헤더
│   ├── Sidebar.jsx       # 좌측 네비게이션
│   ├── Editor.jsx        # 마크다운 에디터
│   └── AiPanel.jsx       # AI 어시스턴트 패널
├── hooks/
│   └── useProject.jsx    # 프로젝트 상태 관리
├── utils/
│   ├── templates.js      # 기획서 템플릿
│   ├── gemini.js         # Gemini API 호출
│   └── exportUtils.js    # 내보내기 유틸
├── App.jsx
├── main.jsx
└── index.css
```

## 📄 라이선스

MIT License

---

Made with ❤️ by PhiMir Team
