# Shaman Scented Candle — 코어 사실 원장

시장·채널·컨셉과 무관하게 **항상 같아야 하는 사실**만 담는다.
마케팅 표현, 카피, 무드는 이 파일에 넣지 않는다.

- 대상: Shaman 센티드 캔들
- 최종 갱신: 2026-09-10
- 원칙: **추측한 값은 넣지 않는다.** 확인하지 못한 항목은 `확인 필요`로 남긴다.
- **용량 · 연소시간 · 왁스 · 심지 · 제조 · 사용법 · 치수 · 가격 · 인증은
  `core/_공통-캔들.md`에 있다.**

## 출처 표기

| 코드 | 출처 |
|---|---|
| `US` | leverden.co — https://leverden.co/products/shaman-scented-candle |
| `KR` | leverden.co.kr — 르버덴 샤먼 센티드 캔들 |
| `US-RAW` | Shopify Admin API 추출본 — `data/shopify-core6-raw.json` (2026-09-09) |
| `KR-HTML` | Cafe24 페이지 원본 HTML (JS 미실행, 2026-09-09 저장) |
| `KR-IMG` | Cafe24 상세페이지 이미지 |
| `소영` | 소영님 직접 확인 (2026-09-09~10) |
| `도시어` | leverden Brand Dossier (2026-09-04) |

---

## 1. 제품명

| 항목 | 값 | 출처 |
|---|---|---|
| 영문 | `Shaman Scented Candle` | `US-RAW` product title |
| 한글 | `르버덴 샤먼 센티드 캔들` | `KR-HTML` page title / JSON-LD name |
| SKU | `777SMCD10` | `US-RAW` |
| 바코드 | **확인 필요** (등록 안 됨) | `US-RAW` `barcode: null` |
| Shopify handle | `shaman-scented-candle` | `US-RAW` |

🔴 `US-RAW` vendor가 `leVerden`으로 되어 있다. **구 표기. 수정 대상.**

⚠️ `KR-IMG`에 `샤먼 센티드 향초` 표기가 있다. `향초` / `캔들` 통일 **확인 필요** (공통 C7)

---

## 2. 향 노트

| 단계 | 값 | 한글 | 출처 |
|---|---|---|---|
| 탑 | Artemisia, Cypress | 아르테미시아 · 사이프러스 | `US-RAW` 본문 `The head notes of Artemisia… Cypress follows` |
| 미들 | Palo Santo, Geranium | 팔로 산토 · 제라늄 | `US-RAW` 본문 `In the heart notes, the sacred Palo Santo… Geranium` |
| 베이스 | Sandalwood, Vetiver | 샌달우드 · 베티버 | `US-RAW` 본문 `the base notes of Sandalwood and Vetiver oil` |

원문에 head/heart/base가 명시되어 있어 그대로 옮겼다. 추론 아님.

---

## 3. 팔로 산토

| 항목 | 값 | 출처 |
|---|---|---|
| 산지 | **페루** | `소영` (2026-09-10 확정) |
| 채취 방식 | 자연 낙목만 채취 (naturally fallen wood only) | `도시어` |
| 학명 | **확인 필요** | — |

### 🔴 학명 확인이 필요한 이유

`팔로 산토`로 불리는 나무는 여럿이고 **규제 지위가 다르다.**

| 학명 | 산지 | CITES |
|---|---|---|
| `Bursera graveolens` | 페루 / 에콰도르 | 규제 대상 아님 |
| `Guaiacum` spp. | — | **부속서 II 규제 대상** |

페루산은 통상 `Bursera graveolens`이나, **학명을 문서로 확인해 두어야 한다.**

### 🔴 지속가능 문구는 근거 확보 후 사용

`US-RAW` 본문에 이미 이렇게 쓰여 있다:

> `you contribute to the preservation of ancient wisdom and the sustainable harvesting of Palo Santo`

⚠️ **근거 없는 `sustainable` 표현은 그린워싱이다.** 자연 낙목 채취에 대한
   **공급처 확인서**를 받아 두어야 하며, 문구로만 두지 않는다.
   페루 수출 서류(SERFOR 등)도 함께 확인할 것.

---

## 4. 조향

| 항목 | 값 | 출처 |
|---|---|---|
| 조향사 | Antoine Lie | `도시어` §03 |

---

## 5. 동봉품

| 항목 | 값 | 출처 |
|---|---|---|
| 세라믹 뚜껑 | 포함 | `소영` |
| 씨앗 | **동봉하지 않음** | `소영` (2026-09-10 확정) |

이 제품은 양쪽 사이트에 씨앗 문구가 없다. 삭제할 것 없음.

---

## 6. 이 제품에만 있는 수정 대상

| 위치 | 문구 | 문제 |
|---|---|---|
| `US-RAW` SEO description | `Purify your environment` | 🔴 공기 정화 = 효능 표현. 삭제 |
| `US-RAW` SEO description | 부시맨 캔들과 **완전히 동일한 문장** | 제품별로 다시 쓸 것 |
| `US-RAW` SEO description | `amber incense scent` | 이 제품 노트에 앰버 없음. 내용 불일치 |
| `US-RAW` 본문 | `creating a serene and toxin-free environment` | 무독성 주장. 삭제 |
| `US-RAW` 본문 | `energize and protect, crafting a haven for positivity` | 효능 표현. 삭제 |
| `US-RAW` 본문 | `working to still your thoughts and quiet the mind` | 효능 표현. 삭제 |
| `US-RAW` vendor | `leVerden` | 🔴 구 브랜드 표기 |
| `US-RAW` metafields | `custom.advantages_paragraph` = Amethyst Ki Bath Soak 설명 | 다른 제품 내용. 삭제 |
| `US-RAW` metafields | `img_w_txt_richtext_3` = 배스 솔트 전성분 | 캔들과 무관. 삭제 |
| `US-RAW` metafields | `custom.img_w_txt_section_richtxt_5` = `lorem ipsum` | 더미 텍스트. 삭제 |
| `US-RAW` metafields | `Consicientious` | 오타 |
| `KR-HTML` JSON-LD description | `제품 개봉 및 사용시 교환/반품은 불가합니다`로 시작 | 순서 조정 |

### ⚠️ '정화'라는 말의 사용 범위

`정화`는 이 콜렉션의 **정서적 무드**이지 제품의 기능이 아니다.

| 안전 | 금지 |
|---|---|
| 마음을 정화하는 의식 / 공간을 정돈하는 향 / a ritual of purification | 공기 정화 / 살균 / 탈취 / purifies the air / antibacterial |

---

# 확인 필요 항목 (이 제품)

| # | 항목 | 필요한 것 |
|---|---|---|
| 1 | 팔로 산토 학명 | 향료사 확인 (CITES 지위가 달라짐) |
| 2 | 자연 낙목 채취 근거 | 공급처 확인서 |
| 3 | 페루 수출 서류 | SERFOR 등 |
| 4 | 바코드 | 미등록 상태 |

공통 확인 필요 항목은 `core/_공통-캔들.md` 하단 참조.
