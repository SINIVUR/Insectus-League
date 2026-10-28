# 인섹터스 리그 v0.0.3

곤충을 잡고, 기르고, 배틀하는 곤충 육성 배틀 RPG.

## 파일 구성
- `index.html` — 게임 본체
- `manifest.webmanifest` — 앱 이름·아이콘·가로 전체화면 설정 (PWA)
- `sw.js` — 서비스 워커 (한 번 열면 인터넷 없이도 실행)
- `icons/` — 앱 아이콘
- `.nojekyll` — GitHub Pages가 파일을 그대로 올리게 하는 빈 파일

## GitHub Pages로 올리기
1. GitHub에서 **New repository** → 이름 예: `insectus-league` → **Public** → Create.
2. 저장소 화면에서 **Add file → Upload files** → 이 폴더 안의 파일과 `icons` 폴더를 통째로 끌어다 놓고 **Commit changes**.
3. **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main**, 폴더: **/(root)** → **Save**.
4. 1~2분 뒤 `https://<내 아이디>.github.io/insectus-league/` 에서 열려요.

## 폰에 앱처럼 설치하기 (PWA)
- 갤럭시(Chrome): 주소를 연 뒤 ⋮ 메뉴 → **앱 설치** 또는 **홈 화면에 추가**.
- 아이폰(Safari): 공유 버튼 → **홈 화면에 추가**.

설치한 앱은 가로 전체화면으로 열리고, 한 번 연 뒤에는 인터넷 없이도 실행돼요.

## 새 버전 올리기
새로 빌드한 파일로 저장소의 파일을 덮어쓰면 돼요. 서비스 워커 캐시 이름에 버전이 들어 있어서,
설치된 앱은 다음에 열 때 새 버전을 받아 두고 그다음 실행부터 바뀌어요.
