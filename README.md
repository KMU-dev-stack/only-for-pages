# 공개 게시 허브

여러 서비스의 공개 문서와 다운로드 파일을 GitHub Pages로 게시하는 공용 저장소입니다. 특정 서비스 전용 저장소가 아닙니다.

공개 첫 화면: [kmu-dev-stack.github.io/only-for-pages](https://kmu-dev-stack.github.io/only-for-pages/)

## 게시 서비스

문서는 **서비스별 폴더**로 분류합니다.

| 서비스 | 폴더 | 게시 내용 |
|---|---|---|
| 온음 (Daytone) | [`daytone/`](https://kmu-dev-stack.github.io/only-for-pages/daytone/) | 이용약관, 개인정보처리방침, 계정 삭제 안내, 보호 페이지, Android QA APK |
| 메이플 에코 : 블록 매치 퍼즐 | [`mapleeco/`](https://kmu-dev-stack.github.io/only-for-pages/mapleeco/) | 유료 상품 안내 및 청약철회(환불) 기준, 월드 운영정책 |

## 온음 (Daytone)

### 공개 문서

| 문서 | 링크 |
|---|---|
| 이용약관 | [보기](https://kmu-dev-stack.github.io/only-for-pages/daytone/terms.html) |
| 개인정보처리방침 | [보기](https://kmu-dev-stack.github.io/only-for-pages/daytone/privacy.html) |
| 계정 삭제 안내 | [보기](https://kmu-dev-stack.github.io/only-for-pages/daytone/delete-account.html) |

### Android QA 다운로드

| 상태 | 파일 | 갱신 시각 (KST) | 용도 | 다운로드·정보 |
|---|---|---|---|---|
| **현재 기능 QA 권장** | `daytone/daytone-auth-qa-release.apk` | **2026-08-05 00:59** | CAPTCHA와 test 서버를 사용하는 로그인·방·녹음·공유 기능 QA | [APK 받기](https://kmu-dev-stack.github.io/only-for-pages/daytone/daytone-auth-qa-release.apk?v=4) · [빌드 정보](https://kmu-dev-stack.github.io/only-for-pages/daytone/daytone-auth-qa-release.apk.build.json) |
| 설치 확인 전용 | `daytone/daytone-qa-release.apk` | 2026-08-18 12:28 | 서버 없이 설치·첫 실행만 확인. 방 만들기·핀 입장 버튼은 표시하지 않음 | [APK 받기](https://kmu-dev-stack.github.io/only-for-pages/daytone/daytone-qa-release.apk?v=bd3270f) · [빌드 정보](https://kmu-dev-stack.github.io/only-for-pages/daytone/daytone-qa-release.apk.build.json) |

실제 기능을 시험할 때는 **현재 기능 QA 권장** 행의 `authenticated` APK를 사용합니다. `local-qa`는 로그인·방·녹음 공유 결과를 판정하는 파일이 아닙니다.

두 APK는 같은 `com.daytone.app.qa` 패키지를 사용하므로 한 기기에 함께 설치할 수 없습니다. 나중에 설치한 판이 앞선 판을 덮어쓰며 저장값과 권한이 이어질 수 있습니다.

`?v=4`, `?v=bd3270f`은 브라우저 캐시를 구분하는 값입니다. 실제 빌드 식별값·파일 크기·SHA-256은 각 `빌드 정보` JSON을 기준으로 확인합니다.

## 메이플 에코 : 블록 매치 퍼즐

| 문서 | 링크 |
|---|---|
| 유료 상품 안내 및 청약철회(환불) 기준 | [보기](https://kmu-dev-stack.github.io/only-for-pages/mapleeco/purchase-notice.html) |
| 월드 운영정책 | [보기](https://kmu-dev-stack.github.io/only-for-pages/mapleeco/world-policy.html) |

## 게시 규칙

- 서비스마다 `<service-slug>/` 폴더를 두고, 그 폴더에는 해당 서비스의 파일만 둡니다.
- 새 서비스를 추가하면 루트 첫 화면과 위 표에 서비스 구역을 함께 추가합니다.
- 다운로드 파일을 교체할 때 빌드 정보 JSON과 캐시 구분값도 함께 갱신합니다.
- 서비스별 폴더로 옮긴 문서는 기존 루트 주소에 리다이렉트 문서를 남겨 이전 링크가 계속 열리게 합니다.
- 이 저장소는 공개 저장소입니다. 공개할 필요가 없는 운영 메모·내부 판단 근거는 각 서비스의 비공개 저장소에 둡니다.
