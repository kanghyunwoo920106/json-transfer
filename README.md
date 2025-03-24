# JSON 트리 뷰어 & 변환기

JSON 데이터를 시각적으로 표현하고 다양한 형식(CSV, XML)으로 변환할 수 있는 웹 애플리케이션입니다.

## 주요 기능

### 1. JSON 데이터 시각화
- 트리 구조로 JSON 데이터 표현
- 계층 구조 펼침/접기 기능
- 데이터 타입별 색상 구분
- 실시간 JSON 유효성 검사

### 2. 다양한 형식 변환
- JSON → CSV 변환
- JSON → XML 변환
- 원본 JSON 형식 유지

### 3. 사용자 친화적 UI
- 모던한 디자인과 반응형 레이아웃
- 드래그 앤 드롭으로 파일 입력 가능
- 에러 메시지 표시
- 다크/라이트 모드 지원

## 설치 방법

1. 저장소 클론
```bash
git clone [repository-url]
cd json-transfer
```

2. 의존성 설치
```bash
pnpm install
```

3. 개발 서버 실행
```bash
pnpm dev
```

4. 브라우저에서 `http://localhost:3000` 접속

## 기술 스택

- **Frontend**: Next.js, React
- **스타일링**: Tailwind CSS
- **언어**: TypeScript
- **형식 변환**: Custom Utilities
- **패키지 관리**: pnpm

## 사용 예시

1. JSON 데이터 입력
   - 직접 텍스트 입력
   - 파일 업로드
   - 예제 데이터 사용

2. 데이터 확인
   - 트리 구조로 시각화된 데이터 확인
   - 노드 펼침/접기로 원하는 부분 탐색

3. 형식 변환 및 다운로드
   - 원하는 출력 형식 선택 (JSON/CSV/XML)
   - 다운로드 버튼 클릭
   - 변환된 파일 저장

## 주요 파일 구조

```
app/
├── dashboard/
│   ├── page.tsx              # 메인 페이지
│   ├── _components/
│   │   ├── JsonTree.tsx      # JSON 트리 뷰어 컴포넌트
│   │   └── JsonInput.tsx     # JSON 입력 컴포넌트
│   └── _utils/
│       └── converters.ts     # 형식 변환 유틸리티
```

## 개발 환경 설정

### 필수 요구사항
- Node.js 16.0.0 이상
- pnpm 8.0.0 이상