# Carnet de mots

프랑스어 핵심 어휘 440개(A1–B2)를 예문, 한국어 해석, 영어 직역과 함께 익히고 간격 반복으로 복습하는 웹앱입니다. 빌드 과정 없이 정적 파일만으로 동작합니다.

## GitHub Pages로 배포

1. GitHub에서 새 저장소를 만듭니다. (예: `carnet-de-mots`, Public)
2. **Add file → Upload files**에서 이 폴더의 파일을 모두 올리고 커밋합니다. 파일들이 저장소 맨 위(루트)에 있어야 합니다.
3. **Settings → Pages**에서 Source를 `Deploy from a branch`, Branch를 `main` / `/ (root)`로 두고 저장합니다.
4. 1–2분 뒤 `https://<사용자명>.github.io/<저장소명>/`에서 열립니다.

## 아이폰에서 앱처럼 쓰기

Safari로 위 주소를 열고 공유 버튼 → **홈 화면에 추가**를 누르면 아이콘이 생기고, 한 번 연 뒤에는 오프라인에서도 동작합니다.

## 알아 둘 점

- 학습 기록은 각 기기의 브라우저에 저장됩니다. 기기 간에 옮기려면 앱의 설정 → 학습 기록 백업에서 내보내기/불러오기를 사용하세요.
- `index.html`을 수정해서 다시 올릴 때는 `sw.js` 첫 줄의 `VERSION` 값을 바꿔 주세요. (예: `carnet-v1` → `carnet-v2`) 그래야 홈 화면 앱이 새 버전을 받습니다.

## 파일

| 파일 | 역할 |
| --- | --- |
| `index.html` | 앱 전체 (단어 데이터 포함) |
| `manifest.webmanifest` | 홈 화면 앱 이름, 아이콘 설정 |
| `sw.js` | 오프라인 캐시 |
| `apple-touch-icon.png`, `icon-*.png` | 앱 아이콘 |
