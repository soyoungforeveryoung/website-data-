# Valley of Roses Scented Candle — 코어 사실 원장

시장·채널·컨셉과 무관하게 **항상 같아야 하는 사실**만 담는다.
마케팅 표현, 카피, 무드는 이 파일에 넣지 않는다.

- 대상: Valley of Roses 센티드 캔들
- 최종 갱신: 2026-09-10
- 원칙: **추측한 값은 넣지 않는다.** 확인하지 못한 항목은 `확인 필요`로 남긴다.
- **용량 · 연소시간 · 왁스 · 심지 · 제조 · 사용법 · 치수 · 가격 · 인증은
  `core/_공통-캔들.md`에 있다.**

## 출처 표기

| 코드 | 출처 |
|---|---|
| `US` | leverden.co — https://leverden.co/products/valley-of-roses-scented-candle |
| `KR` | leverden.co.kr — 르버덴 밸리오브로지즈 센티드 캔들 |
| `US-RAW` | Shopify Admin API 추출본 — `data/shopify-core6-raw.json` (2026-09-09) |
| `KR-HTML` | Cafe24 페이지 원본 HTML (JS 미실행, 2026-09-09 저장) |
| `소영` | 소영님 직접 확인 (2026-09-09~10) |
| `도시어` | leverden Brand Dossier (2026-09-04) |

---

## 1. 제품명

| 항목 | 값 | 출처 |
|---|---|---|
| 영문 | `Valley of Roses Scented Candle` | `US-RAW` product title |
| 한글 | `르버덴 밸리 오브 로지즈 센티드 캔들` | `소영` 확정 |
| SKU | `777TVRCD10` | `US-RAW` |
| 바코드 | **확인 필요** (등록 안 됨) | `US-RAW` `barcode: null` |
| Shopify handle | `valley-of-roses-scented-candle` | `US-RAW` |

⚠️ SKU만 `T` 접두가 붙어 있다 (다른 캔들은 `777BF/BC/SM`). **의도된 것인지 확인 필요.**

### 🔴 한국 사이트 표기 오류

| 위치 | 현재 | 고칠 값 |
|---|---|---|
| `KR-HTML` page title | 르버덴 **벨리**오브로지즈 | **밸리** 오브 로지즈 |
| `KR-HTML` JSON-LD offers name | `르버덴 밸리오브로지즈 센티드 캔들 250g (P000000S000B)` | 제품 코드 노출 자체를 삭제 |

🔴 `P000000S000B`는 **부시맨 캔들의 코드**다. 이 제품의 item_code는 `P00000BF000A`.
   제품명에 코드가 노출되는 것도 문제이고, 그 코드마저 틀렸다.

---

## 2. 향 노트

| 단계 | 값 | 한글 | 출처 |
|---|---|---|---|
| 탑 | Moroccan Rose Petals, Dewy Leaf accord, Elemi | 모로칸 로즈 페탈 · 듀이 리프 어코드 · 엘레미 | `US-RAW` 본문 `These head notes conjure…` |
| 미들 | Fresh Cut Moroccan Rose accord, Clove, Geranium | 갓 자른 모로칸 로즈 어코드 · 클로브 · 제라늄 | `US-RAW` 본문 `it reveals a heart of…` |
| 베이스 | Patchouli, Creamy Sandalwood, Sheer Musk, Cedarwood | 패츌리 · 크리미 샌달우드 · 쉬어 머스크 · 시더우드 | `US-RAW` 본문 `a grounding base of…` |

원문에 head/heart/base가 명시되어 있어 그대로 옮겼다. 추론 아님.

⚠️ `US-RAW` `custom.pdp_accordion_ingredients`의 `Morocccan`은 오타 (c 3개 → 2개).

---

## 3. 원료 산지

| 항목 | 값 | 출처 |
|---|---|---|
| 모로칸 로즈 오일 산지 | 모로코 장미의 계곡 (Valley of Roses) | `소영` (2026-09-10 확정) |
| 마을 | Kelaat M'Gouna (엘켈라 데 므구나) | `도시어` |
| 수급 | 장미의 계곡에서 직접 받아 사용 | `소영` |

🔑 콜렉션명 `Valley of Roses`가 **실제 산지명과 일치한다.**
   향의 모티프가 아니라 그 계곡의 로즈 오일을 실제로 쓴다.
   6종 중 이름과 원료 산지가 일치하는 유일한 제품이다.

⚠️ 공급처명과 서류(COA, 알레르겐 선언서) **확인 필요**.

---

## 4. 조향

| 항목 | 값 | 출처 |
|---|---|---|
| 조향 | 파운더 조소영(Soyoung Cho)과 조향사들의 협업 | `소영`, `도시어` §03 |

🔑 **파운더가 직접 조향에 참여한 유일한 콜렉션이다.**
   다른 3종은 외부 조향사(Christophe Laudamiel / Antoine Lie) 단독이다.

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
| `US-RAW` SEO description | `a conduit for divine blessings… ritual of love, healing, and spiritual renewal` | 🔴 `healing` = 치유 표현. 삭제 |
| `US-RAW` 본문 | `creating a serene and toxin-free environment` | 무독성 주장. 삭제 |
| `US-RAW` 본문 | `the spirit is lulled into a state of peaceful reflection` | 효능 표현. 삭제 |
| `US-RAW` `custom.pdp_accordion_ingredients` | `NON-GMO COCONUT` | 🔴 Non-GMO 사용 보류 확정. 삭제 |
| `US-RAW` `custom.pdp_accordion_ingredients` | `Morocccan` | 오타 |
| `US-RAW` `custom.pdp_about_the_perfumer` | 조향사 소개 자리에 **제품 설명**이 들어 있음 | 파운더 협업 내용으로 교체 |
| `US-RAW` metafields | `custom.advantages_paragraph` = Amethyst Ki Bath Soak 설명 | 다른 제품 내용. 삭제 |
| `US-RAW` metafields | `img_w_txt_richtext_3` = 배스 솔트 전성분 | 캔들과 무관. 삭제 |
| `US-RAW` metafields | `custom.img_w_txt_section_richtxt_5` = `lorem ipsum` | 더미 텍스트. 삭제 |
| `US-RAW` metafields | `Consicientious` | 오타 |
| `KR-HTML` page title | `벨리` | 🔴 오타 → `밸리` |
| `KR-HTML` JSON-LD offers name | `(P000000S000B)` | 🔴 다른 제품 코드. 삭제 |
| `KR-HTML` JSON-LD description | `제품 개봉 및 사용시 교환/반품은 불가합니다`로 시작 | 순서 조정 |

---

# 확인 필요 항목 (이 제품)

| # | 항목 | 필요한 것 |
|---|---|---|
| 1 | 모로칸 로즈 오일 공급처 | 공급처명 + COA + 알레르겐 선언서 |
| 2 | SKU `T` 접두 | 의도된 것인지 확인 |
| 3 | 바코드 | 미등록 상태 |
| 4 | 한국 사이트 제품 코드 | `P00000BF000A`가 맞는지 재확인 후 노출 자체를 삭제 |

공통 확인 필요 항목은 `core/_공통-캔들.md` 하단 참조.
