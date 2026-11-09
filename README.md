# YouTube Data API 증액 신청용 기본 웹사이트

공개 YouTube 메타데이터를 API 키로 조회하는 내부 저작권 모니터링 도구를 **전제**로 만든 HTML 템플릿입니다. 홈페이지·개인정보처리방침·이용약관을 포함합니다. 실제 서비스 운영사항과 다르면 그대로 제출하면 안 됩니다.

## 필수 수정

1. 세 파일에서 `[운영 조직명]`, `[회사 또는 운영 조직명 입력]`, `[실제 문의 이메일 입력]`, `[실제 담당 부서 입력]`, `[실제 게시 시행일 입력]` 등의 대괄호 항목 전부를 실제 정보로 교체하세요.
2. `privacy.html` 4절의 **데이터 갱신·삭제 주기**는 실제 구현과 일치시키세요. 30일이라는 숫자만 쓰는 것은 정책 준수의 증거가 아닙니다.
3. OAuth / 비공개 사용자 데이터 취급 여부, 외부 위탁·제공 여부, 실제 보안 통제 내용 등을 확인한 뒤 수정하세요.
4. 내부 프로그램의 실제 서비스명, 운영 조직을 반영하세요. 회사가 없다면 사실에 맞게 개인 개발·운영자로 표시합니다.
5. 적어도 `privacy.html`과 `index.html`이 공개 접근 가능해야 합니다.

## GitHub Pages 배포

1. GitHub에 새 공개(public) 저장소를 생성합니다. 예: `youtube-monitoring-policy`.
2. 이 폴더의 `index.html`, `privacy.html`, `terms.html`, `style.css` 파일을 저장소 **최상위 경로**에 업로드합니다.
3. 저장소 **Settings > Pages > Build and deployment > Source: Deploy from a branch** 선택.
4. Branch: `main` / Folder: `/ (root)` 선택 후 Save.
5. 배포된 주소는 일반적으로 다음과 같습니다.
   - 홈: `https://USERNAME.github.io/youtube-monitoring-policy/`
   - 개인정보처리방침: `https://USERNAME.github.io/youtube-monitoring-policy/privacy.html`
   - 이용약관: `https://USERNAME.github.io/youtube-monitoring-policy/terms.html`
6. 로그아웃 브라우저에서도 세 페이지와 외부 Google 링크가 열리는지 확인합니다.

## 신청서 증빙

- `index.html` 배포 URL: 서비스 홈페이지 URL.
- `privacy.html` 배포 URL: 개인정보처리방침 URL.
- 홈페이지 전체 및 개인정보처리방침의 YouTube API / Google 정책 링크 / 삭제정책이 읽히는 화면 캡처.
- 실제 내부 프로그램의 동작 화면 또는 화면 녹화는 **별도** 준비. 본 소개용 템플릿이 작동하는 프로그램의 증빙을 대체하지는 않습니다.

## 주의

이것은 제출 준비용 **초안**이며, 공식적인 법률 검토나 Google 승인 보장이 아닙니다. 개인정보처리방침이 실제 시스템의 보관·삭제 동작과 일치해야 하고, YouTube API의 최신 개발자 정책과 적용 법률을 준수해야 합니다.
