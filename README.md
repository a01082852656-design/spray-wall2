# CRACKER Hold Selector v2

벽 사진 위에서 원하는 홀드를 클릭하고, Roboflow SAM 3 Interactive Segmentation으로 홀드 외곽선을 받아 원본 사진 위에 표시한 뒤 PNG로 저장하는 사이트입니다.

## GitHub 업로드 구조

반드시 아래 구조를 유지하세요.

```
index.html
app.js
style.css
worker.js
README.md
spray wall.jpg
```

특히 `spray wall.jpg`가 빠지면 기본 벽 사진이 표시되지 않습니다.

## GitHub Pages

Settings → Pages → Source: Deploy from a branch → Branch: main / (root)

이미 설정되어 있다면 Save를 누를 필요가 없습니다.
