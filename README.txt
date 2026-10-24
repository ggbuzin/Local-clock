CLOCK SCREEN PWA — GitHub Pages 배포

1. 이 ZIP의 파일과 폴더를 GitHub 저장소의 최상위(root)에 업로드하세요.
   기존 index.html이 있다면 이 버전으로 교체합니다.
2. GitHub 저장소 > Settings > Pages에서:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /(root)
   - Save
3. 배포가 끝난 뒤 https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/ 를 Chrome Android에서 여세요.
4. 먼저 사이트를 열고 잠시 사용한 다음 Chrome 메뉴(⋮)에서 '앱 설치' 또는 '홈 화면에 추가'를 확인하세요.
5. 설치한 앱 아이콘으로 실행해야 manifest의 fullscreen 표시 모드가 적용됩니다.

배경 사진:
- 본인 사진을 background.jpg라는 이름으로 저장소 최상위에 업로드하세요.
- 기존 background.jpg를 교체하면 됩니다.
- 이 샘플에는 테스트용 배경 이미지가 포함되어 있습니다.

화면 조정:
index.html의 :root 안에서 --date-y, --time-y, --icon-x, --icon-y, --date-size, --time-size, --spin-speed 값을 수정하세요.

주의:
- GitHub Pages 사이트는 공개됩니다. 민감한 사진은 업로드하지 마세요.
- Chrome 메뉴에 설치가 바로 나타나지 않을 수 있습니다. 매니페스트/아이콘 경로를 확인하고, 배포 후 잠시 기다렸다가 사이트를 다시 열어 보세요.
- 서비스 워커가 캐시한 이전 버전이 남으면 Chrome에서 사이트 데이터를 지우거나, sw.js의 CACHE_NAME 버전(v1)을 v2로 바꿔 재배포하세요.
