# 토픽 듣기 카드

엑셀(xlsx)을 올리면 행마다 카드 한 장을 만들고, TTS로 읽어 주는 정적 웹앱입니다.

- 첫 행 = 머리글, 이후 각 행 = 카드. 같은 행에 있는 그림은 그 카드 아래에 붙습니다.
- 재생 / 속도 / 연속(다 읽으면 다음 카드) / 줄을 누르면 그 줄부터 읽기.
- 마지막으로 읽은 카드·줄을 시트별로 기억했다가 "이어 듣기"로 재개합니다.
- 올린 파일과 진도는 **이 기기의 브라우저 안에만** 저장됩니다(서버 전송 없음).

## 사용 팁
- 모바일에서 화면이 꺼지면 브라우저가 읽기를 멈출 수 있습니다(재생 중에는 화면 꺼짐 방지를 요청합니다).
- 목소리·읽을 칸·제목 칸은 `설정`에서 바꿀 수 있습니다.
- 키보드: ← → 카드 이동, Space 재생/일시정지.

## GitHub Pages 배포
1. github.com에서 새 저장소 생성(예: `topic-tts-cards`).
2. 이 폴더에서:
   ```
   git remote add origin https://github.com/<아이디>/topic-tts-cards.git
   git push -u origin main
   ```
   (또는 저장소 웹 화면에서 `index.html`을 드래그해 업로드)
3. 저장소 Settings → Pages → Branch `main` / `/ (root)` → Save.
4. `https://<아이디>.github.io/topic-tts-cards/` 로 접속.
