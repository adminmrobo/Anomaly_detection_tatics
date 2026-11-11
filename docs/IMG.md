# 평소와 다른 한 건 찾기 — 이미지 제작 명세서 (이상 탐지 연구실)

| 항목 | 내용 |
|---|---|
| 페이지 | index.html (+ .en .zh .ja .ru .uz .vi) |
| 모드 / 주 앵커 | 교과서 모드(인포그래픽 해설) / D 생활·현장: 점의 들판 |
| 시즌 | 기본 |
| 대결 | R(주판봇 승, 경보 15건 중 진짜 이상: 고립 숲 8건 대 칸별 Z 점수 3건) |
| 새로 그릴 그림 | P1 2장 · P2 2장 · P3 1장 |
| 재사용 | 표정 전부 (캐릭터 팩) |
| 그림이 없을 때 | 페이지는 캔버스 무대·대체 표지로 이미 완성 상태 |

## 1. 그림체와 고정 외형
- 스타일: SKILL 18-3 (16비트 RPG 픽셀아트, 굵은 외곽선, 2~3단계 명암)
- 캐릭터 고정 외형: 캐릭터 팩 18-4 (박사 · 조수 · 초파리 연구원 · 주판봇)
- 장소 영어 묘사: *a night lab where hundreds of small glowing green dots float above a long table like a starry field, with one lone red-glowing dot drifting apart from them, a small tree-shaped model made of branching glowing lines on a stand, and a horizontal amber laser line stretched across the room*
- 생물 앵커가 아니므로 현미경·초파리 해부 소품은 넣지 않음

## 2. 필요한 그림 전체

| # | 키 | 판 | 크기 | 상태 | 우선 | 들어가는 곳 | 대신 쓰는 그림 |
|---|---|---|---|---|---|---|---|
| 1 | cover_anomaly | L | 1920×1080 | 새로 (docs/COVER.md) | P1 | 맨 위 글 표지 | 대체 표지(CSS + 캐릭터 넷) |
| 2 | sc_anomaly_hero | E | 1200×800 | 새로 | P1 | 히어로 무대 | 캔버스 무대 + 캐릭터 그림 |
| 3 | sc_anomaly_outro | E | 1200×800 | 새로 | P2 | 아웃트로 | 없음(장면 생략) |
| 4 | thumb_anomaly | I | 600×400 | 새로 (표지 3:2 자르기) | P3 | 소개용 썸네일 | 없음 |
| 5 | og_anomaly | K | 1200×630 | 새로 (표지 자르기) | P3 | 공유 미리보기 | img/og.jpg (첫 화면 캡처, 임시) |
| 6 | 표정 키 전부 | A~D | 96px | 재사용 (캐릭터 팩 @5269662) | — | 말풍선·대결·등장인물 | 픽셀 지도 |
| 7 | 실험 그림 | — | — | 코드 | — | 캔버스 | — |

## 3. 새로 그릴 그림 상세

### 3-1. `cover_anomaly` — 글 표지
`docs/COVER.md`를 그대로 씁니다.

### 3-2. `sc_anomaly_hero` — 히어로 무대 (결과 암시 없음)
대체 글: 네 캐릭터가 초록 점의 들판 한가운데서 홀로 떨어진 붉은 점을 바라보는 연구실 장면
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, a night lab where hundreds of small glowing green dots float above a long table like a starry field, with one lone red-glowing dot drifting apart from them, a small tree-shaped model made of branching glowing lines on a stand, and a horizontal amber laser line stretched across the room, chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie at the back center with a hand on his chin, anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings on the left facing right holding a magnifying glass, boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, two small tank treads, holding a wooden abacus on the right facing left holding up an abacus bead, girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans at the side holding a clipboard, all looking at the lone red dot, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands.
```

### 3-3. `sc_anomaly_outro` — 아웃트로 (대결 후, 주판봇 승)
표정 기준(캐릭터 팩 5-8, 차이 5건 ≥ 기준): 초파리 `fly_cry`, 주판봇 `robo_happy`, 박사 `doc_front`, 조수 `asst_smile`, 인턴 시아 `sia_doze`, 인턴 모아 `moa_tea`(인턴은 선택 출연, 캐릭터 팩 1.4 C9). 대체 글: 고립 숲 나무 모형 앞에서 두 팔을 든 주판봇, 두 손으로 얼굴을 감싼 초파리 연구원, 점수판을 든 조수와 고개를 끄덕이는 박사, 뒤에서 꾸벅 조는 인턴 시아와 찻잔 쟁반을 든 인턴 모아
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, inside the same night lab, a small glowing tree model made of branching lines stands on the table with several red dots caught in its branches, the boxy robot in front raising both arms happily, the fruit fly researcher covering its face with both hands in mock despair, the girl researcher holding a blank score board, the scientist nodding; chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie; girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans; anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings; boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, two small tank treads, holding a wooden abacus; in the background, a quiet intern girl with waist-length straight jet-black hair, side-swept bangs, no hair ornament, gray eyes, small silver drop earrings, long-sleeved charcoal-black maid dress with a large gray ribbon and an ankle-length white frilled apron, dozing on a stool; a cheerful intern girl with long ash-beige hair with wavy ends, a white frilled maid headband and a white ribbon above her left ear, amber eyes, white shirt with a red-and-navy plaid ribbon tie, camel knit cardigan, white frilled apron, black skirt, carrying a tray with tea cups; no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands.
```

## 4. 일관성 지침
- 참고 이미지: 네 캐릭터 기본 그림 4장 + 인턴 시아·모아 기본 그림 2장(아웃트로) + 이 시리즈의 첫 표지
- 미공개 X1~X3은 표지·장면 그림에 넣지 않습니다(캐릭터 팩 1.4 C9: 버튼 뒤에만)
- 같은 캐릭터는 같은 세션에서 연달아 만들기
- 투명 배경이 안 되면 *solid flat #00ff00 background*

## 5. 넘겨받은 뒤 처리
1. 크기 확인 → WebP 압축(표지 1600 220 KB 이하)
2. 표지·장면 그림을 페이지의 `cover_anomaly`, `sc_anomaly_hero`, `sc_anomaly_outro` 자리에 넣고 6개 언어판에도 같이 반영
3. 페이지 그림 합계 표지 포함 600 KB 이하 확인

## 6. 매니페스트
```json
{"page":"index","anchor":"D:dot-field","season":"default","duel":{"result":"R","gap":5},
 "images":[
  {"key":"cover_anomaly","plate":"L","size":[1920,1080],"status":"new","priority":"P1","slot":"cover","fallback":"css-pixel-four","alt":"네 캐릭터가 밤의 연구실에서 수많은 초록 점 사이에 홀로 붉게 빛나는 점 하나를 돋보기와 주판으로 살피는 표지"},
  {"key":"sc_anomaly_hero","plate":"E","size":[1200,800],"status":"new","priority":"P1","slot":"hero-stage","fallback":"canvas-stage","alt":"네 캐릭터가 초록 점의 들판 한가운데서 홀로 떨어진 붉은 점을 바라보는 연구실 장면"},
  {"key":"sc_anomaly_outro","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"outro","fallback":"none","alt":"고립 숲 나무 모형 앞에서 두 팔을 든 주판봇, 두 손으로 얼굴을 감싼 초파리 연구원, 점수판을 든 조수와 고개를 끄덕이는 박사, 뒤에서 꾸벅 조는 인턴 시아와 찻잔 쟁반을 든 인턴 모아"},
  {"key":"thumb_anomaly","plate":"I","size":[600,400],"status":"new","priority":"P2","slot":"thumbnail","fallback":"none","alt":""},
  {"key":"og_anomaly","plate":"K","size":[1200,630],"status":"new","priority":"P3","slot":"og","fallback":"img/og.jpg","alt":""}]}
```
