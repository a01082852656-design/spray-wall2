# CRACKER Hold Selector v1

사용자가 벽 사진에서 홀드를 클릭하면 Roboflow SAM 3 Interactive(PVS)에 point prompt를 보내고, 반환된 mask를 원본 사진 위에 색상 테두리/라벨로 표시합니다. 결과는 PNG로 저장합니다.

## GitHub Pages
index.html, style.css, app.js, worker.js, assets/wall.jpg를 업로드합니다. Pages를 켠 뒤 사이트 왼쪽 AI 연결에 Roboflow API Key를 입력하고 AI 설정 적용을 누르면 테스트할 수 있습니다.

## 공개 운영 권장
Cloudflare Worker로 worker.js를 배포하고 Worker Secret `ROBOFLOW_API_KEY`에 Roboflow 키를 넣습니다. 사이트의 Worker URL 칸에 Worker 주소를 입력하면 GitHub 코드에 API Key를 넣지 않아도 됩니다.

## 주의
API 응답 형식에 따라 mask 파싱이 달라질 수 있습니다. 현재 SAM3 PVS의 point prompt / positive-negative click 흐름에 맞춰 작성했습니다.
