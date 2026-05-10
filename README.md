# AssetGrow — 자산 성장 트래커

나만의 가계부 앱. 소비 습관 개선으로 목돈 마련.

## 포함된 기능

- **홈 대시보드** — 예산 바, 무지출 챌린지 스트릭, AI 피드백, Smart Sync 거래 내역
- **지출 분석** — 카테고리별 바 차트, 전달 비교, 월별 약점 트리거 자동 생성
- **목표 플래너** — 숫자패드 입력, 한글 금액 표시, 월별 저축 계획 자동 계산
- **살까 말까** — 카테고리별 현실 자각 트리거, 배달/카페/쇼핑/구독 맞춤 메시지

## 안드로이드 설치 방법 (PWA)

1. 파일 4개를 웹 서버에 올려요 (GitHub Pages, Netlify, Vercel 전부 무료)
2. 크롬에서 해당 주소 접속
3. 주소창 오른쪽 "⋮" → "홈 화면에 추가" 탭
4. 설치 완료 — 진짜 앱처럼 아이콘이 생겨요!

## GitHub Pages로 무료 배포하는 법 (가장 쉬움)

```
1. github.com 가입
2. New repository → 이름 입력 (예: assetgrow)
3. 파일 4개 업로드 (index.html, manifest.json, sw.js, icon-*.svg)
4. Settings → Pages → Branch: main → Save
5. https://[내아이디].github.io/assetgrow 접속
```

## 로컬 테스트

```bash
# Python 있으면
python3 -m http.server 8080
# 브라우저에서 http://localhost:8080 접속
```

## 파일 구조

```
assetgrow/
├── index.html      # 앱 전체 (HTML + CSS + JS 한 파일)
├── manifest.json   # PWA 설정 (앱 이름, 아이콘, 테마색)
├── sw.js           # Service Worker (오프라인 지원)
├── icon-192.svg    # 앱 아이콘 (소)
└── icon-512.svg    # 앱 아이콘 (대)
```

## 다음 단계 (실제 앱으로 발전)

- **React Native** 로 전환하면 → Google Play Store 등록 가능
- **Firebase** 연동하면 → 실제 데이터 저장/동기화
- **SMS 파싱** 추가하면 → 카드 알림 자동 입력
