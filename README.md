# Board Project 📋

## 🛠 Tech Stack
### Frontend
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=Next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=TypeScript&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat&logo=GraphQL&logoColor=white)
![Apollo Client](https://img.shields.io/badge/Apollo_Client-311C87?style=flat&logo=Apollo-GraphQL&logoColor=white)
![CSS Modules](https://img.shields.io/badge/CSS_Modules-000000?style=flat&logo=CSS3&logoColor=white)

### Backend
![GraphQL API](https://img.shields.io/badge/GraphQL_API-E10098?style=flat&logo=GraphQL&logoColor=white)

## 📁 Project Structure
src/
├── app/
│   ├── boards/
│   │   ├── page.tsx               # 게시글 목록
│   │   ├── new/                   # 게시글 등록
│   │   └── [boardId]/            # 게시글 상세/수정
├── components/
│   ├── boards-list/              # 게시글 목록 관련
│   │   ├── list/                 # 게시글 목록 컴포넌트
│   │   ├── pagination/           # 페이지네이션
│   │   └── search/               # 검색 컴포넌트
│   ├── boards-write/            # 게시글 작성 관련
│   └── boards-detail/          # 게시글 상세 관련
└── commons/
└── graphql/              # GraphQL 관련 파일
## 🔍 주요 기능

### 1. 게시글 목록
- 📋 **목록 조회**
  - 페이지네이션 기반 게시글 목록
  - 게시글 상세페이지 연동
  - 동적 넘버링 시스템

- 🔍 **검색 시스템**
  - 디바운싱 적용된 제목 검색
  - 날짜 기반 필터링
  - 검색어 하이라이트 기능

### 2. 게시글 관리
- ✏️ **통합 입력 폼**
  - 사용자 정보 입력 및 검증
  - 실시간 유효성 검사
  - 상태 피드백 시스템

- 🎨 **멀티미디어 지원**
  - 이미지 업로드 (5MB 제한)
  - 다음 우편번호 API 연동
  - 유튜브 콘텐츠 통합

### 3. 상세 페이지
- 📝 **콘텐츠 표시**
  - 반응형 이미지 갤러리
  - 유튜브 영상 임베딩
  - 주소 정보 인터랙티브 툴팁

- 🔒 **보안 기능**
  - 비밀번호 기반 수정/삭제
  - 접근 권한 관리

### 4. 댓글 시스템
- 💬 **실시간 상호작용**
  - CRUD 기능 완비
  - 무한 스크롤 구현
  - 실시간 업데이트
    
## 🌟 개발 특징
### 프론트엔드 최적화
Apollo Client를 활용한 효율적인 상태 관리
CSS Modules로 스타일 격리 구현
TypeScript 기반 타입 안정성 확보

## 🚀 시작하기

```bash
# 의존성 설치
npm install
# or
yarn install

# 개발 서버 실행
npm run dev
# or
yarn dev

# GraphQL 타입 생성
npm run codegen


