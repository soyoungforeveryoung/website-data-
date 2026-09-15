# 영문 상세페이지 원고 (leverden.co)

- 작성: 2026-09-15
- 기준: `cafe24-html/` 한국어 원고 6종을 영문으로 옮긴 것
- 용도: **Shopify 제품 설명(descriptionHtml)에 붙여넣기**
- 원칙: **추측한 값은 넣지 않는다.**

## 🔴 아직 사이트에 올리지 않았다

파일만 만들어 뒀다. **소영님 확인 후 제가 Shopify 에 반영한다.**
기존 영문 본문을 통째로 교체하는 작업이라 승인 없이 올리지 않았다.

| 파일 | Shopify handle |
|---|---|
| `01-bamboo-forest-candle.html` | `bamboo-forest-scented-candle` |
| `02-bushman-candle.html` | `bushman-candle` |
| `03-shaman-candle.html` | `shaman-scented-candle` |
| `04-valley-of-roses-candle.html` | `valley-of-roses-scented-candle` |
| `05-charcoal-detox-bar.html` | `charcoal-bar-soap` |
| `06-myrrh-protection-bar.html` | `myrrh-protection-bar` |

---

## 한국어판과 달라진 점

### 1. 샤먼 캔들 제목을 바꿨다

| | |
|---|---|
| 한국어 | `PURIFICATION` |
| **영문** | **`GROUNDING`** |

한국어 본문은 "샤먼들이 팔로 산토를 태워 공간을 정돈한다"는 **전통 서술**이라 문제가 없다.
그러나 영문에서 `PURIFICATION` 을 제목으로 쓰면 **제품이 공기를 정화한다는 주장**으로 읽힌다.
방금 `Purifies the environment` 를 지운 것과 같은 이유다.
본문은 "Shamans in Peru burn palo santo to settle a room" 으로 **주어를 샤먼에 두어**
전통을 서술하되 제품 효능으로 읽히지 않게 했다.

🟡 한국어 페이지의 `PURIFICATION` 도 같이 바꿀지는 **소영님 판단**. 한국어는 문맥상 안전한 편이다.

### 2. `푸드 그레이드 인증` → `food-grade`

한국어는 "푸드 그레이드 **인증** 코코넛 오일"이라고 쓴다.
영문에서는 `certified` 를 뺐다. **Stone Candles 확인서를 아직 못 받았기 때문이다.**
인증서가 오면 `certified` 를 넣는다. → `확인 필요`

🟡 같은 이유로 **한국어의 `인증` 표현도 재검토 대상**이다.

### 3. 견과류 고지를 FAQ 까지 넣었다

미르 바. 한국어와 동일하게 본문 + FAQ 두 곳에 넣었다.

### 4. 전성분을 제조사 원본으로 맞췄다

`docs/코보큐앤에이-전성분-원본.md` 기준. 한국어 페이지와 동일하다.
전성분 줄은 `Sea Salt`, 본문 스토리는 `bamboo salt` — 표기 규칙대로다.

---

## 검증 완료

| 항목 | 결과 |
|---|---|
| `Non-GMO` · `purify` · `detox` 동사 · 최상급 | ✅ 0건 |
| 250 g 표기 | ✅ 6종 전부 |
| 제조국 · 동물실험 | ✅ 6종 전부 |
| 견과류 고지 (미르 바) | ✅ 본문 + FAQ |
| `Commiphora Wildii Oil` | ✅ (`myrrha` 잔존 0) |
| 본문 분량 | 1,975 ~ 2,280자 |

📌 기존 영문 본문은 842~1,000자였다. **약 2배로 늘었다.**
   향 노트 3단 구조 · 사용법 · FAQ · 원료 스토리 · 규격이 새로 들어갔기 때문이다.

---

## 🟡 소영님 확인이 필요한 것

1. **사이트에 올릴지** — 올리라고 하시면 6종 바로 반영한다
2. **샤먼 한국어 제목** `PURIFICATION` 유지 여부
3. **`푸드 그레이드 인증`** — 한국어에서 `인증` 을 뺄지 (확인서 올 때까지)
4. **밸리 오브 로지즈 조향 크레딧** — 한국어는 "파운더 조소영이 조향사들과 함께".
   영문은 `Composed by founder Soyoung Cho with our perfumers` 로 옮겼다.
   Chemia 를 명시할지 여부는 넣지 않았다 → `확인 필요`
