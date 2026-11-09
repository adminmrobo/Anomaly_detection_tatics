# 평소와 다른 한 건 찾기 — 이상 탐지의 다섯 도구

**비즈니스를 위한 데이터 과학 연구실 · 특강 ①**
글 · 안상선 ((주)M-Robo 대표)

수만 건의 결제·전표·센서 기록 가운데 사람이 먼저 봐야 할 "이상한 몇 건"을 어떻게 고를까? 박사·조수(하루)·초파리 연구원·주판봇이 진행하는 연구실 해설 페이지에서, 이상 탐지의 다섯 도구를 브라우저에서 직접 돌려 봅니다. 설치할 것은 없고, HTML 파일 하나를 열면 됩니다.

## 페이지

| 언어 | 파일 |
|---|---|
| 한국어 (원본) | [special01_anomaly_detection.html](special01_anomaly_detection.html) |
| English | [special01_anomaly_detection.en.html](special01_anomaly_detection.en.html) |
| 中文 | [special01_anomaly_detection.zh.html](special01_anomaly_detection.zh.html) |
| 日本語 | [special01_anomaly_detection.ja.html](special01_anomaly_detection.ja.html) |
| Русский | [special01_anomaly_detection.ru.html](special01_anomaly_detection.ru.html) |
| Oʻzbekcha | [special01_anomaly_detection.uz.html](special01_anomaly_detection.uz.html) |
| Tiếng Việt | [special01_anomaly_detection.vi.html](special01_anomaly_detection.vi.html) |

`index.html`은 한국어 페이지로 이동합니다. 페이지 위쪽의 언어 단추로 언제든 바꿀 수 있습니다. 외국어판은 원어민 검수를 거치지 않았습니다.

## 다섯 칸

| 칸 | 도구 | 예시 데이터 | 이 칸의 한계 → 다음 칸 |
|---|---|---|---|
| ① | Z 점수 (평균·표준편차 / 중앙값·MAD) | 식대 결제 200건 | 한 칸만 본다, 큰 이상치가 다른 이상치를 가린다 |
| ② | 마할라노비스 거리 | 출장 150건 (일수·출장비) | 데이터를 타원 하나로 본다 |
| ③ | 고립 숲 (Isolation Forest) | 결제 292건, 두 무리 | 칸이 많은 "모양" 데이터에 약하다 |
| ④ | 복원 오차 (직선 오토인코더) | 매장 방문객 146일 × 24시간 | 점수는 결정이 아니다 |
| ⑤ | 문턱값 (상위 p%, 평균 + kσ, 검증 F1, 검증 비용) | 결제 574건 = 검증 287 + 시험 287 | 정답(확인 결과)이 쌓여야 잘 정한다 |

**대결:** 무리가 둘인 결제에서 경보 15건으로 겨룬 결과, 진짜 이상을 고립 숲(주판봇) 8건, 칸별 Z 점수(초파리 연구원) 3건 잡아 주판봇이 이겼습니다. 시드만 바꾼 데이터 20벌에서도 고립 숲이 모두 앞섰습니다. 무리가 하나인 데이터라면 Z 점수로도 충분하다는 조건을 페이지에 함께 적었습니다.

**초보자용 장치:** 이야기로 먼저(수상한 기록 네 건), 칸마다 박사의 생각 구름, 정확도 95.8%의 함정, 문턱 피해 가기(쪼개 보내기), 자주 하는 오해 세 가지, 수식은 조수가 대신 묻는 쉬운 도입, 코드는 맨 끝 접기 상자.

모든 실험 데이터는 개념을 보여 주려고 만든 예시이며 실제 회사·카드사의 데이터가 아닙니다.

## 출처

- 「Anomaly Detection Mathematics」 인포그래픽 (작성자 미상, 소셜미디어 게시물) — 페이지의 뼈대
- Liu, F. T., Ting, K. M., & Zhou, Z.-H. (2008). Isolation Forest. *ICDM 2008*, 413–422. doi:10.1109/ICDM.2008.17
- Mahalanobis, P. C. (1936). On the generalised distance in statistics. *Proceedings of the National Institute of Sciences of India*, 2(1), 49–55.
- Chandola, V., Banerjee, A., & Kumar, V. (2009). Anomaly detection: A survey. *ACM Computing Surveys*, 41(3), Article 15. doi:10.1145/1541880.1541882
- Baldi, P., & Hornik, K. (1989). Neural networks and principal component analysis. *Neural Networks*, 2(1), 53–58. doi:10.1016/0893-6080(89)90014-2
- scikit-learn `IsolationForest` 문서 (2026-11-10 확인)
- 함께 읽기: 안상선 (2024). 금융 분야의 이상탐지 모델 보안을 위한 통계 기반의 적대적 데이터 대응 방안. *미래사회*, 15(3), 147–166. doi:10.22987/jifso.2024.15.3.147 · [연구실 해설](https://adminmrobo.github.io/my_article_04_adversarial_finance_attack/01_adversarial_finance.html)

## 함께 보기

이 특강은 강의 해설 시리즈 [비즈니스를 위한 데이터 과학 연구실](https://adminmrobo.github.io/data_science_for_business/)의 한 편입니다. 3주차(이상값 다루기), 7주차(정밀도·재현율), 14주차와 함께 보면 좋습니다. 페이지를 만드는 원본(`tools/pages/wS1.*`)과 빌드 도구는 그 저장소에 있습니다.

## 그림

표지·장면 그림 3장은 아직 없어 페이지가 대체 표지로 보입니다. 이미지 생성 지시서는 [`docs/COVER_S1.md`](docs/COVER_S1.md)(표지)와 [`docs/IMG_S1.md`](docs/IMG_S1.md)(히어로·아웃트로 장면)에 있습니다.

## 파일

```
index.html                              한국어 페이지로 이동
special01_anomaly_detection.html        한국어 원본
special01_anomaly_detection.{en,zh,ja,ru,uz,vi}.html   외국어판
docs/COVER_S1.md                        표지 그림 지시서
docs/IMG_S1.md                          이미지 제작 명세서
```
