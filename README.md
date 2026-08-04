# 온음 QA 공개 파일

이 저장소는 QA 안내 문서와 APK를 공개합니다.

| 파일 | 용도 | 직접 링크 |
|---|---|---|
| `daytone-qa-release.apk` | 서버 없는 설치·첫 실행 확인판 (Android 빌드 2) | [local-qa APK](https://kmu-dev-stack.github.io/only-for-pages/daytone-qa-release.apk?v=2) |
| `daytone-auth-qa-release.apk` | CAPTCHA 포함 test 서버 연결 인증 기능 QA | [authenticated APK](https://kmu-dev-stack.github.io/only-for-pages/daytone-auth-qa-release.apk?v=4) |

두 APK는 같은 `com.daytone.app.qa` 패키지를 사용하므로 한 기기에 함께 설치할 수 없습니다. 나중에 설치한 판이 앞선 판을 덮어쓰며 저장값과 권한이 이어질 수 있습니다.

`authenticated` 판은 운영용이 아니며 승인된 test 계정과 이메일 일회용 코드가 필요합니다. `local-qa` 판은 서버에 연결하지 않으므로 로그인·방·녹음 공유 시험에 사용하지 않습니다.

| 문서 | 링크 |
|---|---|
| 이용약관 | [보기](https://kmu-dev-stack.github.io/only-for-pages/) |
| 개인정보처리방침 | [보기](https://kmu-dev-stack.github.io/only-for-pages/privacy.html) |
| 계정 삭제 안내 | [보기](https://kmu-dev-stack.github.io/only-for-pages/delete-account.html) |
