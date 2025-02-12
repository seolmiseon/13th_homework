# Board Project

## 기술 스택 및 설정

### Frontend

-   Next.js
-   TypeScript
-   GraphQL (Apollo Client)
-   CSS Module

### Backend

-   GraphQL API

## 프로젝트 구조

```bash
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
│   │   ├── hook.ts
│   │   ├── index.tsx
│   │   ├── queries.ts
│   │   ├── styles.module.css
│   │   └── types.ts
│   └── boards-detail/          # 게시글 상세 관련
│       ├── detail/             # 게시글 상세 내용
│       ├── comment-write/      # 댓글 작성
│       └── comment-list/       # 댓글 목록
└── commons/
    └── graphql/              # GraphQL 관련 파일


  ## 주요 기능

### 1. 게시글 목록 (Read - List)
* **목록 조회**
  * 게시글 목록 표시
  * 페이지네이션 구현
  * 게시글 클릭 시 상세페이지 이동
  * 넘버링 표시

* **검색 기능**
  * 제목 검색 (디바운싱 적용)
  * 날짜별 필터링
  * 검색어 하이라이트 처리

### 2. 게시글 등록/수정 (Create/Update)
* **통합 입력 폼**
  * 작성자, 비밀번호, 제목, 내용 입력
  * 유효성 검증
  * 성공/실패 처리

* **부가 기능**
  * 이미지 업로드 (최대 5MB)
  * 주소 검색 (다음 우편번호 API)
  * 유튜브 URL 등록

### 3. 게시글 상세 (Read - Detail)
* **상세 정보**
  * 게시글 내용 표시
  * 이미지 갤러리
  * 유튜브 영상 임베드
  * 주소 정보 툴팁

* **관리 기능**
  * 수정/삭제 기능
  * 비밀번호 검증

### 4. 댓글 시스템
* **기본 CRUD**
  * 댓글 작성
  * 수정/삭제 (비밀번호 검증)
  * 작성자, 내용 입력

* **UX**
  * 무한 스크롤
  * 실시간 업데이트

  # 의존성 설치
npm install
yarn install

# 개발 서버 실행
npm run dev or yarn add

# GraphQL 타입 생성
npm run codegen
```
