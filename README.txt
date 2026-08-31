# 올영세일 쿠폰 계산기 — iPhone PWA

구성:
- index.html : 원본 계산기 + PWA 설정
- manifest.json : 홈 화면 앱 설정
- sw.js : 오프라인 캐시
- icon-192.png / icon-512.png : 앱 아이콘

## iPhone 설치 방법
1. 이 폴더 전체를 HTTPS 웹서버(GitHub Pages, Netlify, Vercel 등)에 업로드합니다.
2. iPhone Safari에서 `index.html`이 있는 웹주소를 엽니다.
3. 공유 버튼 → '홈 화면에 추가' → 추가합니다.
4. 홈 화면의 '쿠폰 최적화' 아이콘으로 실행합니다.

주의:
- PWA의 '홈 화면에 추가'는 일반적으로 HTTPS 주소에서 설치해야 합니다.
- 파일 앱에서 로컬 HTML을 여는 것과는 다릅니다.
- 최초 한 번 웹주소로 열어 설치하면, Service Worker가 앱 파일을 캐시하여 이후에는 오프라인에서도 계산 기능을 사용할 수 있습니다.
