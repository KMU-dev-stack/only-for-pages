# 공개 게시 허브

이 저장소는 여러 프로젝트의 공개 문서와 다운로드 파일을 GitHub Pages로 게시하기 위한 공용 저장소입니다. 특정 프로젝트 전용 저장소가 아닙니다.

공개 첫 화면: [kmu-dev-stack.github.io/only-for-pages](https://kmu-dev-stack.github.io/only-for-pages/)

## 게시 프로젝트

| 프로젝트 | 현재 게시 내용 |
|---|---|
| 온음 (Daytone) | Android QA APK, 이용약관, 개인정보처리방침, 계정 삭제 안내, Turnstile 보호 페이지 |

기존 공개 주소와 앱 설정을 깨뜨리지 않기 위해 현재 Daytone 파일은 저장소 루트에 유지합니다. 새 프로젝트 파일은 프로젝트 이름의 영문 소문자 폴더 아래에 둡니다.

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

## 게시 규칙

- 프로젝트별로 이름, 파일 용도, 현재 권장 여부, KST 갱신 시각을 함께 표시합니다.
- 다운로드 파일을 교체할 때 빌드 정보 JSON과 캐시 구분값도 함께 갱신합니다.
- 새 프로젝트는 `<project-slug>/` 폴더로 분리하고 루트 첫 화면에 프로젝트 구역을 추가합니다.
- 기존 공개 주소는 사용하는 앱과 문서를 확인하지 않고 이동하거나 삭제하지 않습니다.
