# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

static HTML/CSS (사용자 확정: 빌드체인·프레임워크 금지). 배포: Cloudflare Pages, `linkpool.boring-km.dev`.

## Users

한국어 사용자. SEO 검색("링크 정리", "북마크 관리")과 SNS/커뮤니티 공유로 유입되는 방문자. 카톡 "나에게 보내기"와 브라우저 탭·북마크에 링크가 쌓이기만 하는 사람. 랜딩은 **데스크탑 전용** (사용자 확정 2026-08-17 — 모바일 대응 포기하고 데스크탑 경험에 올인).

## Product Purpose

링크풀(LinkPool): 링크를 무제한 깊이 중첩 폴더로 정리하는 오프라인 우선 모바일 앱(iOS/Android) + 크롬 확장. 랜딩의 일: 방문자를 앱 설치(App Store / Google Play / Chrome 웹스토어)로 전환.

## Positioning

- 오프라인 우선: 기본 저장은 내 기기, 로그인 시 클라우드 동기화
- 무제한 깊이 중첩 폴더 (세분화 파워유저 방식)
- 크롬 확장 ↔ 앱 동기화, 크롬 북마크 가져오기
- Pro (월 ₩2,900, 사용자 확정): AI 요약 메모 / 링크 무제한 저장(무료 1,000개) / 깨진 링크 검사
- 미출시 기능 언급 금지 (출시된 Pro 3축만)

## Evidence / Assets

- 스토어 URL: App Store `apps.apple.com/kr/app/id1644108674` / Play `play.google.com/store/apps/details?id=com.mr.ac_project_app&hl=ko` / Chrome `chromewebstore.google.com/detail/ekpnjdelmmlffckepgphccolelddblej?hl=ko`
- 앱 아이콘 `assets/icon.png` (보라 체인 링크). 브랜드 컬러: primary `#804DFF` (앱 `colors.dart` 기준). 앱 폰트: Pretendard
- 앱 화면은 실물 스크린샷 대신 **HTML/CSS UI 재구성** 연출 (사용자 확정)
- QR 코드 에셋: `assets/qr-appstore.png`, `assets/qr-googleplay.png`
- 지원 메일 `ts4840644804@gmail.com`, 개인정보/약관은 Notion 공개 페이지

## Brand Commitments

- 랜딩 비주얼 방향: **카테고리 정석** (사용자 확정 2026-08-17, 결정 페이지 canon 선택). 관습을 정면으로, 아이러니 없이 최고 완성도로 실행.
- 품질 기준 제품: **토스(toss.im), Raindrop.io, mymind.com** — 이 셋 옆에 놓아도 부끄럽지 않은 완성도가 기준.

## Constraints

- 한국어만. JS 최소. 외부 의존은 Pretendard CDN 정도만
- SEO 필수: JSON-LD (SoftwareApplication + FAQPage), sitemap, robots, OG 카드
- 사실 카피만 — 지표·고객 수·추천사 발명 금지
