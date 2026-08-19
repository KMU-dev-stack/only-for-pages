# 공개 게시 허브

이 저장소는 여러 프로젝트의 공개 문서와 다운로드 파일을 GitHub Pages로 게시하기 위한 공용 저장소입니다. 특정 프로젝트 전용 저장소가 아닙니다.

공개 첫 화면: [kmu-dev-stack.github.io/only-for-pages](https://kmu-dev-stack.github.io/only-for-pages/)

## 게시 프로젝트

| 서비스 | slug | 위치 | 현재 게시 내용 |
|---|---|---|---|
| 온음 (Daytone) | `daytone` | 저장소 루트 (아래 참고) | Android QA APK, 이용약관, 개인정보처리방침, 계정 삭제 안내, Turnstile 보호 페이지 |
| 메이플 에코 : 블록 매치 퍼즐 | `mapleeco` | `mapleeco/` | 유료 상품 안내 및 청약철회(환불) 기준 |

문서는 **서비스별로 분류**합니다. 새 서비스의 파일은 서비스 이름의 영문 소문자 폴더(`<service-slug>/`) 아래에 둡니다.

⚠ 온음(Daytone)의 파일만 저장소 루트에 남아 있습니다. 이미 공개된 주소가 앱 설정과 스토어 등재 정보에서 참조될 수 있어, 참조 지점을 모두 확인하기 전에는 옮기지 않습니다. `daytone/`로 옮기려면 최소한 아래를 먼저 확인해야 합니다.

- `privacy.html` · `terms.html` — 스토어 등재 정보(개인정보처리방침 URL 등)와 앱 내 링크에 등록되어 있는지
- `delete-account.html` — 스토어 계정 삭제 요청 URL로 등록되어 있는지
- `turnstile.html` — Cloudflare Turnstile 설정이나 앱이 **정확한 경로**로 참조하는지 (리다이렉트로 대체되지 않을 수 있음)
- APK 두 개 — 배포된 다운로드 주소. 바이너리는 HTML 리다이렉트로 대체할 수 없습니다

## 온음 (Daytone)

### Android QA 다운로드

| 상태 | 파일 | 갱신 시각 (KST) | 용도 | 다운로드·정보 |
|---|---|---|---|---|
| **현재 기능 QA 권장** | `daytone-auth-qa-release.apk` | **2026-08-05 00:59** | CAPTCHA와 test 서버를 사용하는 로그인·방·녹음·공유 기능 QA | [APK 받기](https://kmu-dev-stack.github.io/only-for-pages/daytone-auth-qa-release.apk?v=4) · [빌드 정보](https://kmu-dev-stack.github.io/only-for-pages/daytone-auth-qa-release.apk.build.json) |
| 설치 확인 전용 | `daytone-qa-release.apk` | 2026-08-18 12:28 | 서버 없이 설치·첫 실행만 확인. 방 만들기·핀 입장 버튼은 표시하지 않음 | [APK 받기](https://kmu-dev-stack.github.io/only-for-pages/daytone-qa-release.apk?v=bd3270f) · [빌드 정보](https://kmu-dev-stack.github.io/only-for-pages/daytone-qa-release.apk.build.json) |

지금 Daytone의 실제 기능을 시험할 때는 **현재 기능 QA 권장** 행의 `authenticated` APK를 사용합니다. `local-qa`는 로그인·방·녹음 공유 결과를 판정하는 파일이 아닙니다.

두 APK는 같은 `com.daytone.app.qa` 패키지를 사용하므로 한 기기에 함께 설치할 수 없습니다. 나중에 설치한 판이 앞선 판을 덮어쓰며 저장값과 권한이 이어질 수 있습니다.

`?v=4`, `?v=bd3270f`은 브라우저 캐시를 구분하는 값입니다. 실제 빌드 식별값·파일 크기·SHA-256은 각 `빌드 정보` JSON을 기준으로 확인합니다.

### 공개 문서

| 문서 | 링크 |
|---|---|
| 이용약관 | [보기](https://kmu-dev-stack.github.io/only-for-pages/terms.html) |
| 개인정보처리방침 | [보기](https://kmu-dev-stack.github.io/only-for-pages/privacy.html) |
| 계정 삭제 안내 | [보기](https://kmu-dev-stack.github.io/only-for-pages/delete-account.html) |

## 메이플 에코 : 블록 매치 퍼즐

### 공개 문서

| 문서 | 링크 |
|---|---|
| 유료 상품 안내 및 청약철회(환불) 기준 | [보기](https://kmu-dev-stack.github.io/only-for-pages/mapleeco/purchase-notice.html) |

메이플스토리 월드 크리에이터 운영 가이드 8강 「유료 상품 관리 및 환불 정책」이 요구하는 안내 4항목(상품 기본 정보 · 구매/사용 제한 · 청약철회 기준과 경로 · 확률 정보)과, "환불 세부기준을 모든 이용자가 확인할 수 있도록 안내" 의무를 충족하기 위한 문서입니다.

게시 후 이 주소를 **월드 상세 화면의 공지 사항**과 **게임 내 상점 화면**에서 닿게 해야 합니다.

## 게시 규칙

- 프로젝트별로 이름, 파일 용도, 현재 권장 여부, KST 갱신 시각을 함께 표시합니다.
- 다운로드 파일을 교체할 때 빌드 정보 JSON과 캐시 구분값도 함께 갱신합니다.
- 새 서비스는 `<service-slug>/` 폴더로 분리하고 루트 첫 화면에 서비스 구역을 추가합니다. 서비스 폴더에는 그 서비스의 문서만 둡니다.
- 기존 공개 주소는 사용하는 앱과 문서를 확인하지 않고 이동하거나 삭제하지 않습니다.
