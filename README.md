# Next.js 16 Starter Kit

완성도 높은 Next.js 16 기반의 모던 Starter Kit입니다. TypeScript, Tailwind CSS v4, shadcn/ui, 그리고 다양한 UI 컴포넌트를 포함하고 있습니다.

## 🚀 기술 스택

- **Next.js 16** - React 기반 풀스택 프레임워크
- **React 19** - 최신 React 라이브러리
- **TypeScript** - 타입 안전성
- **Tailwind CSS v4** - 유틸리티 기반 CSS 프레임워크
- **shadcn/ui** - 재사용 가능한 컴포넌트 라이브러리
- **Radix UI** - 헤드리스 UI 프리미티브
- **lucide-react** - 아름다운 SVG 아이콘 세트
- **next-themes** - 라이트/다크 테마 지원
- **react-hook-form** - 효율적인 폼 관리
- **zod** - TypeScript 우선 스키마 검증
- **sonner** - 고급 토스트 알림
- **class-variance-authority** - 컴포넌트 변형 관리

## 📁 프로젝트 구조

```
├── src/
│   ├── app/
│   │   ├── layout.tsx         # Root Layout
│   │   ├── page.tsx           # 메인 페이지 (UI 쇼케이스)
│   │   └── globals.css        # 글로벌 스타일
│   ├── components/
│   │   ├── ui/                # shadcn/ui 컴포넌트
│   │   │   ├── button.tsx
│   │   │   ├── badge.tsx
│   │   │   ├── avatar.tsx
│   │   │   ├── dialog.tsx
│   │   │   ├── dropdown-menu.tsx
│   │   │   ├── tooltip.tsx
│   │   │   ├── input.tsx
│   │   │   ├── select.tsx
│   │   │   └── table.tsx
│   │   ├── theme-provider.tsx
│   │   └── mode-toggle.tsx
│   └── lib/
│       └── utils.ts           # 유틸리티 함수
├── public/                    # 정적 파일
├── package.json              # 의존성 관리
├── next.config.js            # Next.js 설정
├── tsconfig.json             # TypeScript 설정
├── tailwind.config.ts        # Tailwind CSS 설정
├── postcss.config.js         # PostCSS 설정
├── .eslintrc.json            # ESLint 설정
└── README.md                 # 이 파일
```

## ✨ 주요 기능

### UI 컴포넌트 쇼케이스
- **버튼** - 다양한 크기 및 스타일 (default, secondary, outline, ghost, destructive)
- **배지** - 상태 표시용 배지 컴포넌트
- **아바타** - 이미지 또는 폴백이 있는 아바타
- **Dialog** - 모달 다이얼로그
- **Dropdown Menu** - 드롭다운 메뉴
- **Tooltip** - 호버 시 나타나는 툴팁
- **Table** - 데이터 테이블
- **Input** - 입력 필드

### 폼 검증
- **react-hook-form** - 효율적인 폼 상태 관리
- **zod** - 스키마 기반 검증
- 실시간 에러 피드백

### 테마 시스템
- **라이트/다크/시스템** 테마 전환
- **next-themes** 기반 구현
- CSS 변수를 사용한 색상 관리

### 아이콘
- **lucide-react** 통합
- 500+ 고품질 아이콘 사용 가능

### 토스트 알림
- **sonner** 기반 토스트 알림
- 성공, 에러, 정보 등 다양한 타입

### 반응형 디자인
- 모바일, 태블릿, 데스크톱 모두 지원
- Tailwind CSS 반응형 클래스 활용

## 🚀 시작하기

### 1. 의존성 설치

```bash
npm install
# 또는
yarn install
# 또는
bun install
```

### 2. 개발 서버 실행

```bash
npm run dev
# 또는
yarn dev
# 또는
bun dev
```

브라우저에서 [http://localhost:3000](http://localhost:3000)을 열어 결과를 확인하세요.

### 3. 빌드

```bash
npm run build
npm run start
```

## 📝 사용 가능한 스크립트

| 명령어 | 설명 |
|--------|------|
| `npm run dev` | 개발 서버 실행 (포트 3000) |
| `npm run build` | 프로덕션 빌드 |
| `npm run start` | 프로덕션 서버 실행 |
| `npm run lint` | ESLint 검사 |
| `npm run lint:fix` | ESLint 자동 수정 |

## 🎨 테마 커스터마이징

### 색상 변경

`src/app/globals.css`에서 CSS 변수를 수정하여 색상을 커스터마이징할 수 있습니다:

```css
:root {
  --primary: 0 0% 9%;
  --primary-foreground: 0 0% 100%;
  /* ... 나머지 색상 변수 ... */
}
```

### Tailwind 설정

`tailwind.config.ts`에서 Tailwind CSS를 커스터마이징할 수 있습니다:

```typescript
const config: Config = {
  theme: {
    extend: {
      colors: { /* ... */ },
      fontFamily: { /* ... */ },
    },
  },
};
```

## 📦 주요 파일 설명

### `src/app/layout.tsx`
- ThemeProvider 래핑
- 메타데이터 설정
- Root HTML 구조

### `src/app/page.tsx`
- UI 컴포넌트 쇼케이스
- 폼 검증 예제
- 테이블 예제
- 아이콘 전시

### `src/components/ui/*`
- shadcn/ui 기반 재사용 가능한 컴포넌트
- Radix UI 프리미티브 활용

### `src/components/theme-provider.tsx`
- next-themes 설정

### `src/components/mode-toggle.tsx`
- 테마 전환 드롭다운 메뉴

### `src/lib/utils.ts`
- `cn()` 함수 (className 병합)
- 유틸리티 함수 저장소

## 🔧 설정 파일

### `next.config.js`
- Next.js 기본 설정
- React Strict Mode 활성화

### `tsconfig.json`
- TypeScript 컴파일러 옵션
- `@/*` 경로 별칭 설정

### `tailwind.config.ts`
- Tailwind CSS 테마 확장
- 다크모드 설정
- 커스텀 색상/폰트 정의

### `postcss.config.js`
- PostCSS 플러그인 설정 (Tailwind, Autoprefixer)

### `.eslintrc.json`
- Next.js ESLint 규칙

## 🚀 배포

### Vercel (권장)

```bash
# Vercel CLI 설치
npm i -g vercel

# 배포
vercel
```

또는 GitHub을 연결하고 자동 배포 설정

### Netlify

```bash
# 빌드
npm run build

# 빌드 폴더: .next
# 배포 폴더: public
```

### Docker

```dockerfile
FROM node:20-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 3000
CMD ["npm", "start"]
```

## 📚 추가 리소스

- [Next.js 문서](https://nextjs.org/docs)
- [Tailwind CSS 문서](https://tailwindcss.com/docs)
- [shadcn/ui 문서](https://ui.shadcn.com)
- [Radix UI 문서](https://www.radix-ui.com)
- [react-hook-form 문서](https://react-hook-form.com)
- [zod 문서](https://zod.dev)

## 💡 팁 및 모범 사례

### 1. 컴포넌트 추가

새 UI 컴포넌트를 추가할 때:
- `src/components/ui/` 폴더에 파일 생성
- shadcn/ui 패턴 따르기
- TypeScript 인터페이스 정의

### 2. 폼 사용

폼을 추가할 때:
- `react-hook-form` 사용
- `zod`로 스키마 정의
- 에러 메시지 표시

### 3. 아이콘 사용

lucide-react에서 아이콘 가져오기:
```typescript
import { Heart, Star, Settings } from 'lucide-react';
```

### 4. 테마 변수 활용

CSS에서 테마 색상 사용:
```css
.my-element {
  @apply bg-background text-foreground;
}
```

### 5. 반응형 디자인

Tailwind 반응형 클래스 사용:
```jsx
<div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3">
  {/* Content */}
</div>
```

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다.

## 🤝 기여

버그 리포트, 기능 제안, PR은 환영합니다!

---

**Happy Coding! 🎉**
