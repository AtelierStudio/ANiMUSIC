# ANiMUSIC
---
## FILES
- PSD : ANiMUSIC의 원본 PSD파일이 저장되어 있습니다.
- RESOURCES : 사용되는 모든 비트맵 리소스가 저장되어 있습니다.
- SCREENSHOTS : 스크린샷이 저장되어 있습니다.

## RESOURCES
- `btn_dock_next.png` : 독에 있는 음악 컨트롤러 중 '>>' 버튼입니다.
- `btn_dock_prev.png` : 독에 있는 음악 컨트롤러 중 '<<' 버튼입니다.
- `btn_dock_play.png` : 독에 있는 음악 컨트롤러 중 재생 버튼입니다.
- `btn_dock_stop.png` : 독에 있는 음악 컨트롤러 중 정지 버튼입니다.
- `ic_dock_sound.png` : 독에 있는 사운드 컨트롤러의 아이콘입니다.
- `ic_title_animusic.png` : 상단 타이틀 부분에 들어가는 ANiMUSIC의 로고입니다.

##ORDER
- 기본
	- 화면 기준은 `2560*1600px`로 작업하였습니다.
- 배경
	- 배경은 현재 재생중인 음악의 앨범아트를 `가우시안 블러`를 시킨 이미지를 적용하고
	- 그 위에 불투명도 `70%`인`#FFF`로 덮어 씌어 줍니다.
-  현재 재생중 (화면에서 왼편의 요소)
	- 앨범 아트의 모서리에는 `5px ~ 10px`의 둥글기 값을 적용해야 합니다.
	- 앨범 아트에는 그림자가 적용되어야 합니다.
		- `Photoshop 기준 각도 90도, 거리 30px, 크기 65px, 불투명도 18%`
	- 앨범아트와 제목 사이 디바이더의 경우 `168px * 4px, 모서리 둥글기값 2px, #424242, 불투명도 20%`로 만들어 줍니다.
	- 곡 제목등의 정보는 아래와 같이 만들어 줍니다.
		- 포맷은 `곡이름 / 아티스트 - 앨범`입니다.
		- 곡의 제목은 `#424242, 96pt`입니다.
			- 영문의 경우 폰트를 `Roboto Light`로 적용시킵니다.
			- 그 외의 경우에는 `Noto Sans CJK Light`로 적용시킵니다.
		- 곡의 아티스트와 엘범 부분은 `#424242, 48pt`입니다.
			- 영문의 경우 폰트를 `Roboto Regular`로 적용시킵니다.
			- 그 외의 경우에는 `Noto Sans CJK Regular`로 적용시킵니다.
- 곡 리스트 (화면에서 오른편의 요소)
	- 엘범 아트의 경우 `가로 세로 80px`입니다.
	- 노래 제목은 `#424242, 36pt`입니다.
		- 영문의 경우 폰트를 `Roboto Bold`로 적용시킵니다.
		- 그 외의 경우에는 `Noto Sans CJK Bold`으로 적용시킵니다.
	- 아티스트와 앨범 제목은 `#424242, 24pt, 불투명도 60%`입니다.
		- 영문의 경우 폰트를 `Roboto Medium`로 적용시킵니다.
		- 그 외의 경우에는 `Noto Sans CJK Medium`으로 적용시킵니다.
	- 리스트의 디바이더는 `앨범아트부터 화면 끝자락까지, 두께 2px, #424242, 불투명도 15%`로 만듭니다.
	- 리스트와 지금 재생중을 구분하는 화면 정가운데의 구분선은 `3px * 1128px, #424242, 불투명도 75%`로 만듭니다.
- 독 (화면 아랫쪽의 요소)
	- 독의 배경은 `2280px * 128px, #424242, 불투명도 80%, 모서리 둥글기값 20px`이며, 그림자는 `Photoshop 기준 각도 90도, 거리 10px, 크기 24px, 불투명도 24%`를 주어야 합니다.
	- 슬라이더는 아래의 속성으로 만듭니다
		- `두께 6px, #FFF, 비활성 부분의 경우 불투명도 50%`
		- 포인트는 `42px * 42px, 원, #FFF, 그림자 Photoshop 기준 각도 90도 거리 4px, 크기 9px, 불투명도 18도`
	- Shuffle과 Repeat 버튼은 아래의 속성으로 만듭니다.
		- 기본 : 배경은 `148px * 48px, 모서리 둥글기 값 10px` 글씨는 `Roboto Medium`
		- 활성화 되어 있을 경우 : 배경 `#FFF`, 글씨`#424242`
		- 비활성화 되어 있을 경우 : 외곽선 `#FFF`(배경색 없음), 글씨`#FFF`
	- 재생 슬라이더 옆의 재생시간의 경우 `00:00 / 11:11`의 포맷으로 작성합니다.