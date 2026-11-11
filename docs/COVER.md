# 표지 지시문 — 평소와 다른 한 건 찾기 (이상 탐지 연구실)

| 항목 | 내용 |
|---|---|
| 키 · 판 | cover_anomaly · L (16:9, 가로 1920 이상) |
| 장소 (앵커) | D 생활·현장: 밤의 연구실에 펼쳐진 점의 들판 |
| 주제 은유 | 수백 개의 초록 점 사이에서 홀로 떨어진 붉은 점 하나, 가지를 뻗은 빛의 나무 모형(고립 숲), 방을 가로지르는 호박색 레이저 선(문턱값) |
| 네 캐릭터 포즈 | 박사: at the back center pointing up at the horizontal amber laser line / 조수: kneeling and counting green dots on a clipboard / 초파리 연구원: on the left facing right, peering at the lone red dot through a big magnifying glass / 주판봇: on the right facing left, holding up a small glowing tree model in one arm and an abacus in the other |
| 대체 글 (alt) | 네 캐릭터가 밤의 연구실에서 수많은 초록 점 사이에 홀로 붉게 빛나는 점 하나를 돋보기와 주판으로 살피는 표지 |
| 다른 표지와 다른 점 | 점의 들판·빛의 나무·레이저 선으로 이 페이지만의 장면을 만듦 |
| 결과 암시 | 없음 (대결 전 장면) · 이 페이지 대결 결과: R(주판봇 승, 경보 15건 중 진짜 이상: 고립 숲 8건 대 Z 점수 3건) — 표지에는 드러내지 않음 |

**참고 이미지 (함께 올리기):** 네 캐릭터 기본 그림 4장 (기준: GitHub `adminmrobo/fruitfly-lab-expressions`).

**Genspark에 붙여 넣기 ↓**
```
웹페이지 맨 위에 거는 표지 그림 1장을 만들어 줘.
- 비율 16:9, 가로 1920px 이상
- 첨부한 참고 이미지의 네 캐릭터(박사, 조수, 초파리 연구원, 주판봇)를 같은 그림체·같은 외형으로, 넷 모두 등장
- 그림 안에 글자·숫자·로고를 넣지 말 것
- 얼굴과 손은 가장자리에서 떨어진 가운데 영역에, 왼쪽 아래 구석은 어둡고 단순하게
아래 영어 프롬프트를 그대로 써 줘.

Website top cover illustration, wide 16:9.
Match the art style, proportions and colors of the attached reference images exactly
  (if there are no reference images: 16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights).
cozy night laboratory mood, purple light, soft magenta and green fluorescent accents.
Scene: a night lab where hundreds of small glowing green dots float above a long table like a starry field, with one lone red-glowing dot drifting apart from them, a small tree-shaped model made of branching glowing lines on a stand, and a horizontal amber laser line stretched across the room.
All four characters together:
  chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie, at the back center pointing up at the horizontal amber laser line;
  girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans, kneeling and counting green dots on a clipboard;
  anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, on the left facing right, peering at the lone red dot through a big magnifying glass;
  boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, two small tank treads, holding a wooden abacus, on the right facing left, holding up a small glowing tree model made of branching lines.
Visual metaphor of the topic: one lone red dot drifting apart from a field of green dots, a branching tree of light that splits the field, and a single amber line that separates "check" from "pass".
Composition: keep every face and hand inside the central safe area (12% margin left and right, 10% top, 18% bottom);
  keep the bottom-left corner dark and simple; the light falls on the lone red dot.
Mood: curious, friendly rivalry, the moment before the result.
No text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands.
```

**고칠 때 (같은 대화에서):** `Same four characters, same art style and composition. Change only: {고칠 점}. Still no text.`

**받은 뒤:** 그림 파일을 주시면 비율·글자·네 캐릭터를 확인하고 WebP(1600×900, 960×540)로 바꿔 `index.html`과 6개 언어판의 표지 자리(`cover_anomaly`)에 넣습니다. 그림이 없어도 페이지는 대체 표지(CSS + 캐릭터 넷)로 완성 상태입니다.

---

# 썸네일 지시문 — 목차 카드·SNS 작은 그림 (thumb_anomaly)

| 항목 | 내용 |
|---|---|
| 키 · 판 | thumb_anomaly · I (3:2, 600×400으로 줄여 씀 — 1536×1024로 생성) |
| 원칙 | 작게 줄여도 읽히게: 요소는 셋(초록 점 무리 · 붉은 점 하나 · 호박색 선), 캐릭터는 크게 |
| 캐릭터 | 넷 모두. 표지보다 가까이 붙여 상반신 위주 (인턴·X1~X3은 넣지 않음) |
| 대체 글 (alt) | 초록 점 무리에서 홀로 떨어진 붉은 점 하나를 돋보기로 들여다보는 초파리 연구원과, 빛의 나무를 든 주판봇, 그 뒤에서 지켜보는 박사와 조수 |
| 다른 방법 | 표지(cover_anomaly)를 받은 뒤 붉은 점·초파리 연구원·주판봇이 들어가게 3:2로 잘라도 됨 |

**Genspark에 붙여 넣기 ↓**
```
목차 카드와 SNS에 쓸 작은 썸네일 그림 1장을 만들어 줘.
- 비율 3:2 (1536×1024), 600×400으로 줄여도 알아볼 수 있게 단순하고 크게
- 첨부한 참고 이미지의 네 캐릭터(박사, 조수, 초파리 연구원, 주판봇)를 같은 그림체·같은 외형으로, 넷 모두 등장
- 그림 안에 글자·숫자·로고를 넣지 말 것
아래 영어 프롬프트를 그대로 써 줘.

Small thumbnail illustration, 3:2 landscape, must stay readable when shrunk to 600x400.
Match the art style, proportions and colors of the attached reference images exactly
  (if there are no reference images: 16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights).
Night laboratory, deep purple background, simple and uncluttered, high contrast.
Only three visual elements besides the characters:
  a loose cluster of glowing green dots on the left half,
  ONE large red-glowing dot clearly apart from the cluster, near the center-right, the brightest thing in the picture,
  one horizontal amber laser line across the upper third.
Characters, large and close to the viewer (waist-up framing for the front two):
  front left: anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, facing right, holding a big magnifying glass up to the lone red dot, surprised;
  front right: boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, facing left, holding up a small glowing tree model made of branching lines, confident;
  behind them, smaller: chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail, white lab coat over black vest and tie, pointing at the amber line;
  girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, holding a clipboard, curious.
Composition: the red dot sits between the magnifying glass and the tree model; all faces inside the central area (8% margin on every side); no tiny details.
Mood: curious, friendly rivalry.
No text, no letters, no numbers, no logos, no weapons, no blood, no real brands.
```

**고칠 때:** `Same four characters, same style and 3:2 framing. Change only: {고칠 점}. Still no text.`

**받은 뒤:** 600×400 WebP(`img/thumb_anomaly.webp`)로 줄여 넣고, `cover_manifest.json`에 `thumb_anomaly` 항목을 더합니다.
