# Bamboo Forest Charcoal Detox Bar — 코어 사실 원장

시장·채널·컨셉과 무관하게 **항상 같아야 하는 사실**만 담는다.
마케팅 표현, 카피, 무드는 이 파일에 넣지 않는다.

- 대상: Bamboo Forest **차콜 디톡스 바 솝** (캔들은 `bamboo-forest.md`)
- 최종 갱신: 2026-09-10
- 원칙: **추측한 값은 넣지 않는다.** 확인하지 못한 항목은 `확인 필요`로 남긴다.
- **중량 · 제조 · 로프 · 가격 · 사용법 · 표시사항은 `core/_공통-바솝.md`에 있다.**

## 출처 표기

| 코드 | 출처 |
|---|---|
| `US` | leverden.co — https://leverden.co/products/charcoal-bar-soap |
| `KR` | leverden.co.kr — 르버덴 뱀부 포레스트 차콜 바 솝 |
| `US-RAW` | Shopify Admin API 추출본 — `data/shopify-core6-raw.json` (2026-09-09) |
| `KR-HTML` | Cafe24 페이지 원본 HTML (JS 미실행, 2026-09-09 저장) |
| `소영` | 소영님 직접 확인 (2026-09-09~10) |
| `도시어` | leverden Brand Dossier (2026-09-04) |

---

## 1. 제품명

| 항목 | 값 | 출처 |
|---|---|---|
| 영문 | `Bamboo Forest Charcoal Detox Bar` | `US-RAW` product title |
| 한글 | `르버덴 뱀부 포레스트 차콜 디톡스 바 솝` | `소영` 확정 |
| SKU | `111BFBS10` | `US-RAW` |
| 바코드 | `00850034664101` | `US-RAW` |
| Shopify handle | `charcoal-bar-soap` | `US-RAW` |

⚠️ 바코드 앞자리 `0`이 두 개다. 다른 제품은 `850034…` 12자리.
   **GTIN 형식 통일 확인 필요.**

### 🔴 채널별 표기 불일치

| 위치 | 현재 표기 |
|---|---|
| `US-RAW` product title | `Bamboo Forest Charcoal Detox Bar` |
| `KR-HTML` page title | 르버덴 뱀부 포레스트 차콜 **바 솝** |
| `KR-HTML` JSON-LD name | 르버덴 뱀부 포레스트 차콜 **디톡스** 바 솝 |

→ 같은 페이지 안에서 title과 JSON-LD가 다르다. **통일 필요.**

### `Detox`라는 이름의 사용 범위

제품명 `Detox`는 **유지한다** (`소영`, 2026-09-10). 금지어가 아니며 통용된다.

⚠️ **단, 본문에서 아래로 넘어가면 안 된다.**

| 안전 | 금지 |
|---|---|
| 딥 클렌징 / 차콜의 스크럽 효과 / deep-cleansing | 독소 배출 / 해독 / detoxify / removes toxins |

---

## 2. 향 노트

| 항목 | 값 | 출처 |
|---|---|---|
| **탑 / 미들 / 베이스 구분** | **확인 필요** | — |
| 전체 노트 | **확인 필요** | — |

🔴 **이 제품은 향 노트가 문서로 확인되지 않았다.**
   `US-RAW`의 `Fragrance Notes` 항목은 노트 목록이 아니라 서술형 카피뿐이다
   (`Imagine the great bamboo forests of Korea…`).

⚠️ **캔들의 노트를 그대로 가져다 쓰면 안 된다.**
   Bamboo Forest는 캔들과 바디의 **향료 회사가 아예 다르다** (Chemia vs IFF).
   배합이 다르므로 노트도 다르다. 상세: `docs/fragrance-registry.md`

### 확인된 것 — 바디 라인 향료

| 항목 | 값 | 출처 |
|---|---|---|
| 향료 코드 | `BAMBOOM 34` (IFF 6059239) | 알레르겐 선언서 |
| Oakmoss 함량 | 1.218% | 알레르겐 선언서 |

⚠️ Oakmoss는 **EU에서 규제 대상 알레르겐**이다 (규정 2023/1545 확대 적용).
   함량이 규제 범위 내여도 **표시 의무**가 발생할 수 있다. → 표시 요건 확인 필요

⚠️ `US-RAW` `About the Perfumer` 문단의 `oakmoss, fir balsam, sage, bamboo sap`은
   **캔들과 바 솝에 동일하게 복붙된 문단**이므로 어느 쪽의 노트 근거도 되지 못한다.

---

## 3. 전성분 (INCI)

> Sodium hydroxide, Cocos nucifera (coconut) oil, Aqua (water),
> Helianthus annuus (sunflower) seed oil, Olea europaea (olive) fruit oil,
> Simmondsia chinensis (jojoba) seed oil, Ricinus communis (castor) seed oil,
> Tocopherol, Theobroma cacao (cacao) seed butter, Vitis vinifera (grape) seed oil,
> Bamboo salt, Lavandula angustifolia (lavender) oil, Charcoal powder,
> Citrus aurantium bergamia (bergamot) leaf oil, Pogostemon cablin oil

출처: `US-RAW` `custom.pdp_ingredients`

⚠️ 원문 `bermot`은 오타. 정확한 표기는 **bergamot**. 🔴 사이트 수정 대상.

⚠️ `Bamboo salt`, `Charcoal powder`는 정식 INCI명이 아니다. → **확인 필요**
   (죽염, 활성탄의 INCI 표기를 제조처에서 확인할 것)

⚠️ `Fragrance (parfum)`가 목록에 없다. 향이 있는 제품인데 향료가 누락되어 있다. → **확인 필요**

---

## 4. 히어로 원료 — 영월 죽염

| 항목 | 값 | 출처 |
|---|---|---|
| 원료 | 죽염 (bamboo salt) | `US-RAW` INCI, `소영` |
| 산지 | **강원도 영월** | `소영` |
| 만든 사람 | **최규동 장인** — 죽염 장인이자 스님 | `소영` (2026-09-11, 실명 공개 가능) |
| 제법 | **3회 구운 죽염** | `소영` (2026-09-11 확정) |

### 🔴 굽는 횟수 — 표기 주의

| 구분 | 횟수 | 명칭 |
|---|---|---|
| 일반적인 죽염 | 9회 | **자죽염** |
| **우리가 쓰는 죽염** | **3회** | 죽염 |

⚠️ **`자죽염` / `구증구포` / `아홉 번 구운` 은 쓸 수 없다.** 우리 원료는 3회다.
   9회 죽염을 뜻하는 용어를 3회 죽염에 붙이면 사실과 다른 표시가 된다.

⚠️ 3회라는 숫자 자체는 **써도 된다.** 숨길 이유가 없고, 구체적인 숫자가 오히려
   "그냥 소금이 아니다"를 설명한다. 다만 9회와 비교해 우위를 암시하지 않는다.

**표기 예시**
- 국문 — 강원도 영월에서 최규동 장인이 대나무 통에 넣어 세 번 구운 죽염을 씁니다.
- 영문 — Bamboo salt from Yeongwol, Korea, fired three times in bamboo by master salt-maker Choi Gyu-dong.

⚠️ 장인이 스님이라는 점은 사실이나, 종교적 권위를 제품 효능과 연결하지 않는다.
   출처를 밝히는 맥락에서만 쓴다.

🔑 비누 장인은 비공개지만, **죽염 장인은 실명까지 공개 가능한 서사다.**

---

## 5. 그 밖의 활성 성분

| 항목 | 값 | 출처 |
|---|---|---|
| 활성탄 (Charcoal powder) | 포함 | `US-RAW` INCI |
| 카카오 씨드 버터 | 포함 | `US-RAW` INCI |
| 코코넛 오일 | 포함 | `US-RAW` INCI |

---

## 6. 이 제품에만 있는 수정 대상

| 위치 | 문구 | 문제 |
|---|---|---|
| `US-RAW` SEO description | `Moisturize and soften your skin instantly with bamboo salt **body lotion**` | 🔴 **제품이 바 솝인데 바디로션 설명이다.** 전면 교체 |
| `US-RAW` `global.title_tag` | `Bamboo Salt Body Lotion - leverden` | 🔴 **제품명이 완전히 다르다.** 전면 교체 |
| `US-RAW` 본문 | `detoxifying… actives` | 🔴 해독 표현. 삭제 |
| `US-RAW` 본문 | `deeply hydrating body moisturizers` | 화장품 효능 표현. 근거 필요 |
| `US-RAW` `custom.pdp_why_you_ll_love_it` | `can alleviate skin problems such as blackheads` | 🔴 **의약품적 효능 표현.** 삭제 |
| `US-RAW` `custom.pdp_why_you_ll_love_it` | `100% biodegradable` | 비누 전체가 아니라 로프에 한정. 범위 수정 |
| `US-RAW` `custom.pdp_accordion_description` | `Test description for Charcoal Bar` | 🔴 **테스트 텍스트가 라이브에 남아 있다.** 삭제 |
| `US-RAW` `custom.pdp_ingredients` | `bermot` | 오타 |
| `US-RAW` `custom.pdp_about_the_perfumer` | `Laudimiel` | 오타 (정: Laudamiel) |
| `US-RAW` product_benefits `How to Use` | `in the toilet` | 화장실 변기 사용 뉘앙스. 럭셔리 카피에 부적합 |
| `US-RAW` 등록 중량 | 0.6 lb (272 g) | 250 g 기준으로 재확인 |
| `KR-HTML` 옵션명 | `255g` | 🔴 **250g으로 수정** |
| `KR-HTML` JSON-LD description | `제품 개봉 및 사용시 교환/반품은 불가합니다`로 시작 | 순서 조정 |
| `KR-HTML` 상세 이미지 alt | `가방 라벤더 색상 이미지-S1L2` × 3 | 🔴 Cafe24 템플릿 샘플값. 전면 교체 |

---

# 확인 필요 항목 (이 제품)

| # | 항목 | 필요한 것 |
|---|---|---|
| 1 | 향 노트 전체 + 탑/미들/베이스 | 향료사(IFF) 노트 문서 — **캔들 노트로 대체 금지** |
| 2 | Oakmoss 표시 의무 | EU 규정 2023/1545 대응 확인 |
| 3 | ~~죽염 제법 (굽는 횟수)~~ | ✅ **3회** 확정. `자죽염`·`구증구포` 사용 금지 |
| 4 | ~~장인 명칭 공개 가부~~ | ✅ **최규동 장인** 실명 공개 가능 |
| 5 | 죽염 · 활성탄 INCI 정식명 | 제조처 확인 |
| 6 | 전성분에 향료 누락 | 제조처 확인 |
| 7 | 바코드 GTIN 형식 | `00850034664101` 앞자리 0 두 개 |

공통 확인 필요 항목은 `core/_공통-바솝.md` 하단 참조.
