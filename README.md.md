# 따숨코치 앱 (설치형 웹앱)

이 폴더를 GitHub Pages에 올리면 핸드폰에 앱처럼 설치할 수 있어요. 무료이고, 설치한 뒤에는 인터넷 없이도 열려요.

## 1. GitHub에 올리기 (컴퓨터에서, 처음 한 번)
1. github.com 가입 → 오른쪽 위 **+** → **New repository**
2. 이름 `ttasum`, **Public** 선택 → **Create repository**
3. **uploading an existing file** 누르기 → 이 폴더 안의 파일과 `icons` 폴더를 통째로 끌어다 놓기
   (폴더 자체가 아니라 **안에 있는 것들**을 올려야 해요: index.html, manifest.webmanifest, sw.js, icons)
4. 아래 **Commit changes**
5. 저장소의 **Settings → Pages** → Source: **Deploy from a branch**, Branch: **main / (root)** → **Save**
6. 1~2분 뒤 같은 화면 위쪽에 주소가 나와요: `https://내아이디.github.io/ttasum/`

## 2. 핸드폰에 설치
- **안드로이드(크롬)**: 주소 열기 → 아래에 뜨는 **앱 설치** 또는 메뉴(⋮) → **앱 설치**
- **아이폰(사파리)**: 주소 열기 → 공유 버튼 → **홈 화면에 추가**

## 3. 고친 내용 올리기 (업데이트)
1. 바뀐 `index.html`을 같은 방법으로 다시 올리기 (같은 이름이면 덮어써요)
2. `sw.js` 맨 위 `ttasum-v1`의 숫자를 하나 올려서 함께 올리기 (예: `ttasum-v2`)
3. 핸드폰에서 앱을 한 번 열었다 닫으면 새 버전으로 바뀌어요

## 알아 둘 점
- AI 코칭·AI 채팅·라벨 사진 읽기: 앱의 ‘따숨 코치’ 칸 맨 아래 **🔑 AI 키**에서 고르고 키를 넣으면 켜져요.
  - **Claude**: claude.ai 링크와 같은 AI(같은 지시문·계산기). Anthropic 계정(Claude Platform)의 API 키(sk-ant-…)가 필요하고, 쓴 만큼 요금이 나가요.
  - **구글 Gemini**: Google AI Studio 키. 결제 수단을 등록하지 않으면 무료 한도 안에서만 동작해요.
  - 키는 그 핸드폰에만 저장돼요. **키를 index.html이나 GitHub에 절대 넣지 마세요.** 키가 없으면 기본 코치가 답해요.
- 생활 기록은 앱마다 따로 저장돼요. claude.ai에서 쓰던 기록은 ‘CSV로 내보내기’ → 앱에서 ‘CSV 불러오기’로 옮겨요.
- 기록은 핸드폰 안에만 저장되고 서버로 보내지 않아요.
