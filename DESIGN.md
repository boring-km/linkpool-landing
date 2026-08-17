---
name: 링크풀 랜딩 (LinkPool Landing)
description: 흰 바탕과 잉크 타이포 위에 보라 #804DFF를 집중 투입하는 데스크톱 전용 카테고리 정석 랜딩
colors:
  primary: "#804DFF"
  primary-deep: "#5F2EE0"
  primary-tint: "#F3EFFF"
  ink: "#191F28"
  sub: "#4E545C"
  bg: "#FFFFFF"
  surface: "#F7F8FA"
  border: "#E6EAF1"
  ok: "#14804A"
  bad: "#C7362B"
typography:
  display:
    fontFamily: "Pretendard Variable, Pretendard, -apple-system, BlinkMacSystemFont, Apple SD Gothic Neo, Noto Sans KR, sans-serif"
    fontSize: "5rem"
    fontWeight: 800
    lineHeight: 1.14
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Pretendard Variable, Pretendard, sans-serif"
    fontSize: "2.3rem"
    fontWeight: 800
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Pretendard Variable, Pretendard, sans-serif"
    fontSize: "1.55rem"
    fontWeight: 800
  body:
    fontFamily: "Pretendard Variable, Pretendard, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Pretendard Variable, Pretendard, sans-serif"
    fontSize: "0.82rem"
    fontWeight: 600
    lineHeight: 1.5
rounded:
  sm: "9px"
  md: "12px"
  lg: "14px"
  xl: "16px"
  window: "18px"
  drench: "28px"
  pill: "999px"
spacing:
  gap-card: "14px"
  pad-panel: "20px"
  gutter: "32px"
  gap-column: "72px"
  section: "120px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.lg}"
    padding: "17px 30px"
  button-primary-hover:
    backgroundColor: "{colors.primary-deep}"
  button-nav:
    backgroundColor: "{colors.ink}"
    textColor: "#FFFFFF"
    rounded: "10px"
    padding: "9px 18px"
  button-nav-hover:
    backgroundColor: "{colors.primary-deep}"
  chip-pro:
    backgroundColor: "{colors.primary-tint}"
    textColor: "{colors.primary-deep}"
    rounded: "{rounded.pill}"
    padding: "4px 12px"
  card-link:
    backgroundColor: "{colors.bg}"
    rounded: "{rounded.md}"
    padding: "15px 16px"
  card-pro:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.drench}"
    padding: "56px 48px"
  toast:
    backgroundColor: "{colors.ink}"
    textColor: "#FFFFFF"
    rounded: "{rounded.md}"
    padding: "12px 18px"
  faq-item:
    backgroundColor: "{colors.bg}"
    rounded: "{rounded.lg}"
    padding: "17px 20px"
---

# Design System: 링크풀 랜딩

## Overview

**Creative North Star: "카테고리의 정석 (The Canon)"**

링크 관리 카테고리의 관습을 아이러니 없이 정면으로, 최고 완성도로 실행하는 세계다. 품질 기준선은 토스(toss.im)·Raindrop.io·mymind.com — 이 셋 옆에 놓아도 부끄럽지 않아야 한다. 흰 바탕 위에 잉크(#191F28)의 대형 타이포가 말하고, 브랜드 보라(#804DFF)는 데모 UI의 액센트·CTA·포커스·Pro 카드에만 집중 투입된다. 앱 화면은 실물 스크린샷 대신 전부 HTML/CSS로 재구성한 "테마드 브라우저 창"으로 연출한다 — 이 재구성 UI가 제품의 증명이다.

밀도는 낮고 호흡은 길다. 섹션은 120px 수직 패딩으로 넉넉히 떨어지고, 흰 바탕(#FFFFFF)과 옅은 회색 면(#F7F8FA)이 교대로 깔리며 섹션 리듬을 만든다. 이 랜딩은 **데스크톱 전용**(`min-width: 1080px`, 반응형 브레이크포인트 없음)이며, 유일한 미디어 쿼리는 `prefers-reduced-motion` 분기다. 명시적으로 거부하는 것: 폰 목업 스크린샷 나열.

**Key Characteristics:**
- 잉크 온 화이트 대형 타이포 + 집중 투입되는 보라 액센트
- 앱 화면은 100% HTML/CSS 재구성 (래스터 스크린샷 금지)
- 로드 시 1회만 재생되는 단일 오케스트레이션 모션
- 데스크톱 전용, 미디어 쿼리는 reduced-motion 하나뿐
- 사실 카피만 — 발명된 지표·추천사 없음 (PRODUCT.md 확정 제약)

## Colors

거의 무채색인 잉크·회색 베이스 위에 브랜드 보라 한 계열만 목소리를 내는 절제된 팔레트다.

### Primary
- **브랜드 보라** (`#804DFF`, `--primary`): 앱 아이콘에서 온 브랜드색 (앱 `colors.dart` 기준). Primary CTA 배경, 데모 UI의 폴더 아이콘·AI 배지, 텍스트 선택(::selection), 포커스 링, 스크롤바 호버, Pro 드렌치 카드 배경에 쓰인다.
- **딥 보라** (`#5F2EE0`, `--primary-deep`): 보라의 인터랙션·텍스트 단계. 버튼 hover 배경, 틴트 면 위의 텍스트, 본문 속 링크 색. 흰 바탕에서 보라로 "글자"를 써야 할 때는 항상 이쪽을 쓴다.
- **보라 틴트** (`#F3EFFF`, `--primary-tint`): 보라의 면(面) 단계. 선택된 폴더 행 배경, Pro 태그 칩, AI 메모 블록, feat UI 뒤에 깔리는 오프셋 백킹 슬랩.

### Neutral
- **잉크** (`#191F28`, `--ink`): 제목·본문의 기본 글자색이자 다크 서피스(토스트, 내비 CTA 버튼) 배경. 토스 계열의 블루-블랙.
- **서브** (`#4E545C`, `--sub`): 보조 문단, 캡션, 내비 링크, 푸터. 잉크보다 낮은 위계의 모든 텍스트.
- **바탕** (`#FFFFFF`, `--bg`): 페이지와 카드의 기본 바탕.
- **면** (`#F7F8FA`, `--surface`): 교대 섹션 배경(features, closing), 브라우저 창의 크롬 바·사이드바 배경.
- **경계** (`#E6EAF1`, `--border`): 1px 실선 보더 전용. 카드·창·섹션 경계 모두 이 한 값.

### Semantic
- **정상 그린** (`#14804A`, `--ok`): 깨진 링크 검사 UI의 통과 체크 아이콘 전용.
- **경고 레드** (`#C7362B`, `--bad`): 죽은 링크 행의 텍스트·아이콘. 배경은 전용 틴트 `#FDF1F0`.

### Named Rules
**보라 집중 투입 규칙 (The Concentrated Purple Rule).** 보라는 넓게 바르지 않고 좁게 꽂는다: CTA, 포커스, 데모 UI 액센트, 그리고 단 하나의 풀-드렌치 서피스(Pro 카드). 본문 텍스트나 섹션 배경을 보라로 칠하지 않는다.

**딥 포 텍스트 규칙 (The Deep-for-Text Rule).** 흰·틴트 바탕 위 보라 텍스트는 `#804DFF`가 아니라 항상 `#5F2EE0`(primary-deep)이다. `#804DFF`는 흰 글자를 얹는 배경과 아이콘에만 쓴다.

## Typography

**Display/Body Font:** Pretendard Variable (Pretendard, -apple-system, Apple SD Gothic Neo, Noto Sans KR 폴백) — jsDelivr CDN dynamic subset, 단일 폰트 패밀리.

**Character:** 한 서체가 웨이트 대비만으로 전체 위계를 만든다. 헤딩은 전부 ExtraBold(800)에 음수 자간, 본문은 Regular(400)에 1.65 행간. 한국어 조판 규칙이 전역 적용된다: `word-break: keep-all`, 헤딩 `text-wrap: balance`, 리드 문단 `text-wrap: pretty`.

### Hierarchy
- **Display** (800, 5rem, 1.14, -0.02em): 히어로 h1 전용. 두 줄로 꺾이는 대형 선언.
- **Headline** (800, 2.3rem, -0.01em): 섹션 h2 (features/faq/closing). 중앙 정렬.
- **Title** (800, 1.55rem): feat 항목 h3.
- **Body** (400, 1rem 기준, 1.65): 기본 본문. feat 문단은 1.03rem/sub색/최대 26rem, 히어로 서브는 1.2rem/sub색/최대 40rem.
- **Label** (600–800, 0.72–0.95rem): 재구성 UI 내부 텍스트, 캡션, 칩. 칩·배지는 800에 양수 자간(0.02–0.03em)으로 소형에서 힘을 유지한다.

### Named Rules
**웨이트로 말하기 규칙 (The Weight-Does-The-Work Rule).** 위계는 폰트 교체가 아니라 800↔600↔400 웨이트 대비와 잉크↔서브 색 대비로만 만든다. 이탤릭·세리프·모노 서체는 이 세계에 없다.

## Layout

중앙 정렬 단일 컬럼 세계. 컨테이너 최대폭은 콘텐츠 성격별 계단: 내비·히어로 1120px, feat 행 1020px, 데모 창 960px, FAQ 720px, 문서 페이지 640px, Pro 카드 520px. 좌우 거터는 전 구간 32px.

- **섹션 리듬**: 수직 패딩 120px(닫는 섹션 104px), 섹션 h2 아래 88px. 흰 바탕 ↔ `--surface` 면이 1px 보더를 사이에 두고 교대한다.
- **feat 행**: `grid-template-columns: 1fr 1fr`, gap 72px, 카피와 UI 재구성이 좌우 교차(`.rev`가 order 반전). 행 간 마진 104px.
- **재구성 데모 창**: 250px 사이드바 + 1fr 본문 그리드, 본문은 2열 카드 그리드(gap 14px, 패딩 20px).
- **내비**: sticky, `rgba(255,255,255,0.88)` + `backdrop-filter: blur(12px)`, 하단 반투명 보더.
- **데스크톱 전용**: `body { min-width: 1080px }`. 반응형 브레이크포인트 없음 — 이는 사용자 확정 결정이다 (PRODUCT.md 2026-08-17).

## Elevation & Depth

그림자는 구조가 아니라 공기다: 큰 blur·낮은 알파의 앰비언트 섀도가 "떠 있는 정도"를 말하고, 실제 경계는 항상 1px `--border`가 담당한다. 그리고 그림자는 요소 자신의 색을 따른다 — 흰 서피스는 잉크 그림자, 보라 서피스는 보라 그림자.

### Shadow Vocabulary
- **창 부양** (`box-shadow: 0 24px 80px rgba(25, 31, 40, 0.14)`): 히어로 재구성 데모 창. 페이지에서 가장 높은 잉크 그림자.
- **패널 부양** (`box-shadow: 0 12px 40px rgba(25, 31, 40, 0.08)`): feat UI 재구성 패널(tree/ext-pop/ai-card/check-list) 공통.
- **토스트** (`box-shadow: 0 10px 30px rgba(25, 31, 40, 0.3)`): 다크 서피스의 진한 잉크 그림자.
- **보라 글로우** (`box-shadow: 0 8px 24px rgba(128, 77, 255, 0.32)`): Primary CTA 기본. hover 시 `0 12px 32px rgba(128, 77, 255, 0.4)`로 상승.
- **보라 드렌치 글로우** (`box-shadow: 0 24px 64px rgba(128, 77, 255, 0.35)`): Pro 카드.

### Named Rules
**동색 그림자 규칙 (The Same-Hue Shadow Rule).** 그림자 색은 요소의 색에서 온다. 보라 요소는 `rgba(128,77,255,…)`, 그 외 서피스는 잉크 `rgba(25,31,40,…)`. 중립 검정 `rgba(0,0,0,…)` 그림자는 쓰지 않는다.

**보더가 경계, 그림자가 높이 규칙 (The Border-Edges Rule).** 흰 바탕 위 흰 카드는 그림자만으로 구분하지 않는다 — 1px `--border`가 항상 먼저 경계를 긋고, 그림자는 높이감만 더한다.

## Shapes

전면 라운드 사각 언어이며, 반지름은 요소의 스케일을 따라 계단식으로 커진다: 마이크로 요소 6–8px(파비콘 칩, 아이콘) → 리스트 행 9–10px → 카드·토스트 12px → 버튼·FAQ·QR 프레임 14px → 재구성 패널 16px → 브라우저 창 18px → Pro 드렌치 카드 28px. 태그·배지·상태 필은 완전 pill(999px)이다.

시그니처 실루엣이 둘 있다:
- **브라우저 창 실루엣**: `border-radius: 18px 18px 0 0; border-bottom: 0`으로 상단만 둥글고 하단이 섹션 경계에 잘려 나가는 창 — "화면 아래로 계속된다"는 암시.
- **오프셋 틴트 슬랩**: feat UI 패널 뒤 `::before`가 `inset: 22px -22px -22px 22px`, radius 22px의 `--primary-tint` 면으로 오른쪽-아래로 어긋나게 깔린다. 재구성 패널의 공통 받침이다.

아이콘은 전부 인라인 stroke SVG다: `fill="none"`, stroke `currentColor`, stroke-width 1.6–2, round cap/join, 17–22px. 아이콘 폰트·글리프 문자·외부 아이콘 패키지는 쓰지 않는다.

## Components

### Buttons
- **Primary CTA** (`.btn-primary`): 보라 배경 + 흰 텍스트(700, 1.08rem), radius 14px, padding 17px 30px, 좌측 22px stroke 아이콘, 보라 글로우 그림자. Hover: `--primary-deep` 배경 + `translateY(-2px)` + 그림자 상승, active에서 translate 복귀. 전환은 `0.18s var(--ease)`.
- **Nav CTA** (`.nav-cta`): 잉크 배경 + 흰 텍스트(700, 0.9rem), radius 10px, padding 9px 18px. Hover 시 배경이 `--primary-deep`으로 — 잉크 버튼도 인터랙션 순간엔 보라가 된다.
- **CTA 짝 규칙**: Primary CTA는 항상 QR 페어(iPhone/Android 설치 QR 프레임 2개)와 한 행(gap 36px)으로 다닌다. 히어로와 클로징에서 동일 구성이 반복된다.

### Chips
- **Pro 태그 / AI 배지**: pill(999px), 800 웨이트, 양수 자간. Pro 태그는 틴트 배경+딥 보라 텍스트, AI 배지는 보라 배경+흰 텍스트. 상태 필("연결 안 됨")은 `border: 1px solid currentColor` 아웃라인 pill.

### Cards / Containers
- **링크 카드** (`.demo-card`): 흰 배경, 1px 보더, radius 12px, padding 15px 16px, 그림자 없음(창 내부라서). 구조: 파비콘 칩(20px, radius 6px, 이니셜 레터) + 700 제목 → sub색 메모 → 딥 보라 600 URL.
- **재구성 패널** (tree/ext-pop/ai-card/check-list): 흰 배경, 1px 보더, radius 16px, 폭 360–400px 고정, 패널 부양 그림자, 뒤에 오프셋 틴트 슬랩.
- **Pro 드렌치 카드**: 이 페이지에서 유일하게 보라를 면으로 쓰는 서피스. radius 28px, padding 56px 48px, 보라 드렌치 글로우, 흰 텍스트, mask 기반 흰 체크 원 불릿.

### 재구성 데모 창 (시그니처)
앱 화면의 HTML/CSS 재구성. 크롬 바(surface 배경, 11px 회색 dot 3개 + 창 제목) + 사이드바(폴더 트리, 보라 폴더 아이콘, 카운트) + 2열 링크 카드 그리드. `role="img"` + aria-label로 하나의 그림으로 선언된다. **단일 오케스트레이션 모션**이 여기서만 재생된다: 창 상승(0.9s, delay 0.15s) → 카드 6장 스태거 인(0.25s부터 0.07s 간격) → 카톡 토스트 드롭(0.9s 시점) → 대상 폴더 하이라이트 점멸(1.15s) → 카운트 10→11 크로스페이드(1.3s). 전 구간 `cubic-bezier(0.16, 1, 0.3, 1)`(`--ease`), `backwards` fill로 1회만.

### Toast
잉크 배경, 흰 텍스트(0.88rem), radius 12px, 토스트 그림자. 내부 액센트는 다크 전용 밝은 톤: 체크 아이콘 `#7CE3A8`, 강조 텍스트 `#CDB9FF`.

### FAQ (details/summary)
흰 카드(1px 보더, radius 14px, padding 17px 20px, 간격 10px). summary는 700 웨이트, 마커 대신 우측에 보라 2px 보더 셰브론(9px)이 `0.25s var(--ease)`로 회전. 열리면 sub색 답변 문단.

### Navigation
sticky 반투명 화이트 + blur(12px). 브랜드(아이콘 28px radius 7px + 800 워드마크) / 앵커 링크(600, sub색, hover 시 잉크) / 우측 Nav CTA. 페이지 내 앵커 스크롤은 `scroll-behavior: smooth`(reduced-motion 시 auto).

### 모션 문법 (전역)
- 로드 오케스트레이션은 히어로 데모 창 1회뿐. 스크롤 트리거·루프 애니메이션 없음.
- 인터랙션 마이크로: hover 색 전환 0.18s, CTA `translateY(-2px)`, FAQ 셰브론 0.25s. 모두 `--ease` 사용.
- `prefers-reduced-motion: reduce` 분기 완비: 모든 애니메이션 제거 + 오케스트레이션의 **최종 정착 상태**(새 카운트 11 표시)로 렌더.

## Do's and Don'ts

### Do:
- **Do** 앱 화면이 필요하면 HTML/CSS로 재구성한다 — 테마드 브라우저 창, 재구성 패널, 오프셋 틴트 슬랩 문법으로.
- **Do** 아이콘은 인라인 stroke SVG(currentColor, stroke-width 1.6–2, round cap)로 그린다.
- **Do** 새 애니메이션엔 `--ease`(`cubic-bezier(0.16,1,0.3,1)`)와 reduced-motion 분기를 함께 붙이고, 정착 상태가 정보상 완결이 되게 한다.
- **Do** 한국어 텍스트 블록엔 `word-break: keep-all`을, 헤딩엔 `text-wrap: balance`를 유지한다.
- **Do** 설치 CTA는 Chrome 확장 primary + QR 페어 구성을 그대로 복제한다.

### Don't:
- **Don't** 폰 목업·실물 스크린샷을 나열하지 않는다 (THESIS의 명시적 거부).
- **Don't** 보라를 본문 텍스트(`#804DFF` 그대로)나 넓은 섹션 배경에 쓰지 않는다 — 풀-드렌치는 Pro 카드 하나뿐.
- **Don't** 반응형 브레이크포인트·모바일 레이아웃을 추가하지 않는다 — 데스크톱 전용은 확정 결정이다.
- **Don't** 루프·스크롤 트리거 애니메이션을 넣지 않는다 — 모션은 로드 시 1회 오케스트레이션과 hover 마이크로뿐.
- **Don't** 중립 검정 그림자, 아이콘 폰트, 제2의 폰트 패밀리를 들이지 않는다.
