# 후쿠오카·유후인 가족여행

2026.10.04~10.07 일정표, 예약 현황, 점검 포인트, 준비물을 담은 정적 페이지입니다.

- 사이트: https://fukuoka-m4fy.vercel.app
- 구성: `index.html` 한 장 + `vercel.json` (빌드 과정 없음)

## 배포

Vercel 프로젝트가 이 GitHub 레포와 연결되어 있습니다.
`main` 브랜치에 push 또는 merge 하면 자동으로 배포됩니다.
다른 브랜치는 Preview 주소만 만들어지고 실서비스에는 반영되지 않습니다.

## 살 것 리스트 (캡처)

일정 탭의 "🛒 살 것"에 쇼핑 캡처를 모아 둡니다. 체크하면 이미지가 접힙니다.

- 이미지는 `shopping/` 폴더에 JPG(가로 900px 이하)로 둡니다.
- `index.html`의 `<script type="application/json" id="buy-data">` 배열에 항목을 추가합니다.
  `{"id":"b1","img":"shopping/b1.jpg","title":"이름","note":"메모","w":900,"h":1948}`
- 체크 상태는 `id`별로 폰 브라우저에 저장되므로 한 번 쓴 `id`는 바꾸지 않습니다.
