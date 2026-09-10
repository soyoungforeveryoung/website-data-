# Bamboo Forest Scented Candle — 코어 사실 원장

시장·채널·컨셉과 무관하게 **항상 같아야 하는 사실**만 담는다.
마케팅 표현, 카피, 무드는 이 파일에 넣지 않는다.

- 대상: Bamboo Forest **센티드 캔들** (바 솝은 별도 파일)
- 최종 갱신: 2026-09-10
- 원칙: **추측한 값은 넣지 않는다.** 확인하지 못한 항목은 `확인 필요`로 남긴다.

## 출처 표기

| 코드 | 출처 |
|---|---|
| `US` | leverden.co (Shopify) — https://leverden.co/products/bamboo-forest-scented-candle |
| `KR` | leverden.co.kr (Cafe24) — https://leverden.co.kr/product/르버덴-뱀부-포레스트-센티드-캔들/15/ |
| `US-RAW` | Shopify Admin API 추출본 — `data/shopify-core6-raw.json` (2026-09-09 추출) |
| `KR-HTML` | Cafe24 페이지 원본 HTML (JS 미실행, 2026-09-09 저장) |
| `KR-IMG` | Cafe24 상세페이지 이미지 |
| `소영` | 소영님 직접 확인 (대화, 2026-09-09~10) |
| `도시어` | leverden Brand Dossier (2026-09-04) |

---

## 1. 제품명

| 항목 | 값 | 출처 |
|---|---|---|
| 영문 | `Bamboo Forest Scented Candle` | `US-RAW` product title / JSON-LD name |
| 한글 | `르버덴 뱀부 포레스트 센티드 캔들` | `KR-HTML` JSON-LD name, page title |
| 브랜드 표기 | `leverden` (전부 소문자) / `르버덴` | `소영`, `도시어` §11 |

⚠️ `KR-IMG`에는 `샤먼 센티드 향초` 형식(다른 제품)이 쓰여 있어, **`향초` / `캔들` 표기가 채널·매체별로 다르다.**
→ 어느 쪽으로 통일할지 **확인 필요**

---

## 2. 용량

| 항목 | 값 | 출처 |
|---|---|---|
| 순 왁스 중량 (g) | **250 g** | `소영`, `KR-HTML` JSON-LD offers name `…센티드 캔들 250g` |
| 순 왁스 중량 (oz) | **확인 필요** | — |
| 총 중량 (배송용) | 2.3 lb (약 1,043 g) | `US-RAW` inventoryItem measurement |

⚠️ **oz 표기는 확인 필요.** 250 g의 단위 환산값은 8.82 oz이나,
   제품 라벨·패키지에 실제로 인쇄된 oz 값이 무엇인지 확인되지 않았다. 환산값을 그대로 쓰지 않는다.

⚠️ 2.3 lb는 **배송 중량**으로 보이며 순 왁스 중량과 구분해야 한다. 고객 노출값은 250 g.

---

## 3. 연소 시간

| 항목 | 값 | 출처 |
|---|---|---|
| 연소 시간 | **약 60시간** | `KR-HTML` JSON-LD description `연소 시간: 60시간` / `US-RAW` product_info `Burning time: 60 hours` / `소영` 확정 |

표기: `약 60시간` / `approx. 60 hours` — 연소 조건에 따라 달라지므로 단정 표기하지 않는다.

---

## 4. 향 노트

| 항목 | 값 | 출처 |
|---|---|---|
| 전체 노트 | Basil, Spearmint, Sage, Coriander, Immortelle, Sandalwood, Tonka, Amber | `US-RAW` SEO description `Fragrance Notes` |
| 한글 | 바질, 스피어민트, 세이지, 코리앤더, 임모르텔, 샌달우드, 통카, 앰버 | 위 항목 번역 |
| **탑 / 미들 / 베이스 구분** | **확인 필요** | — |

⚠️ 원 자료에는 **평면 목록으로만** 존재한다. 단계 구분이 문서로 확인되지 않았다.
   (Bushman Candle·Shaman·Valley of Roses는 원문에 단계가 명시되어 있으나, 이 제품만 없다.)
   → 향료 노트 문서 확인 필요

### 원 자료에 함께 등장하나 노트로 확정되지 않은 원료

| 원료 | 등장 위치 | 판단 |
|---|---|---|
| Elemi | `US-RAW` product_info 서술형 Fragrance Notes 문단 | 확인 필요 |
| Oakmoss, Fir Balsam | `US-RAW` `About the Perfumer` 문단 | **노트 아님.** 이 문단은 캔들과 바 솝에 동일하게 복붙되어 있어 근거가 되지 못한다 |

⚠️ Oakmoss는 **바디 라인 향료** `BAMBOOM 34`(IFF 6059239)에 1.218% 포함되어 있음이 알레르겐 선언서로 확인되었으나,
   **캔들 향료 문서에서는 확인되지 않았다.** 캔들과 바디는 향 배합이 다르다.

---

## 5. 원료

| 항목 | 값 | 출처 |
|---|---|---|
| 왁스 | 코코넛 왁스 + 애프리컷 씨드 오일 블렌드 | `소영`, `US-RAW` `natural coconut-apricot wax` |
| 심지 | 오가닉 코튼, 납 미사용 | `US-RAW` `lead-free organic cotton wick` |
| 심지 개수 | **1개** | `소영` |
| 향료 | 프래그런스 오일 | `KR-IMG` `천연 재료의 하이엔드 프레그런스 오일` |
| **캔들용 향료 코드** | **확인 필요** | — |
| 뚜껑 | 세라믹 | `소영` |

⚠️ **향료 코드 확인 필요.** Google Drive에 `Chemia 78296 CORIANDER FRAGRANCE` IFRA 인증서가 있고
   코리앤더가 이 콜렉션과 연결되나, **이 향료가 캔들용인지 바디용인지 문서로 확인되지 않았다.**

### 원 자료에 있으나 근거 미확보

| 문구 | 출처 | 상태 |
|---|---|---|
| Non-GMO | `US-RAW` | **인증서 미확보.** 사용 보류 |
| food-grade certified coconut oil | `US-RAW` | 제조사 마케팅 문구. **인증서 미확보** |
| kosher | `US-RAW` | **인증서 미확보** |
| 100% vegan, beeswax-free, paraben-free, cruelty-free | `US-RAW` | 인증 주체 확인 필요 |

---

## 6. 제조

| 항목 | 값 | 출처 |
|---|---|---|
| 제조 국가 | 미국 | `US-RAW` `made in the USA` |
| 제조 지역 | 캘리포니아 | `US-RAW` `Hand-poured in California` |
| 제조 방식 | 핸드푸어 (손으로 붓기) | `US-RAW` |
| 제조사 | Stone Candles | `소영` |
| 조향사 | Christophe Laudamiel | `도시어` §03 |

⚠️ `US-RAW` 본문에 `Laudimiel` 오타가 있다. 정확한 표기는 **Laudamiel**.

---

## 7. 동봉품

| 항목 | 값 | 출처 |
|---|---|---|
| 세라믹 뚜껑 | 포함 | `소영` |
| 코리앤더 씨앗 | **확인 필요** | — |

⚠️ 씨앗 동봉 정책이 확정되지 않았다.
   - `US-RAW`: `Comes with a packet of Coriander seeds`
   - `KR-HTML` JSON-LD: `컬렉션 향을 연상시키는 코리앤더 씨를 함께 제공합니다`
   - `소영` (2026-09-10): 상시 동봉은 아니며 주문 시 개별 대응. 문구는 당분간 유지.
   → **상시 동봉 여부를 확정해야 한다.** 표기와 실제가 다르면 표시광고 문제가 된다.

---

## 8. 사용법과 주의사항

| 항목 | 값 | 출처 |
|---|---|---|
| 첫 연소 | 표면 전체가 녹을 때까지 2~3시간 | `US-RAW` product_benefits |
| 심지 자르기 | **3~5 mm** | `US-RAW` `cut the wick to keep about 3-5mm` / `소영` 확정 |
| 1회 연소 한도 | 3시간 | `US-RAW` `do not burn your candle for more than 3 hours at a time` |
| 사용 중단 시점 | 왁스 약 1 cm 잔여 | **확인 필요** |

### 🔴 채널 간 불일치

| 항목 | US | KR 이미지 |
|---|---|---|
| 심지 자르기 | 3~5 mm | **2 mm** |

→ **3~5 mm로 확정** (`소영`, 2026-09-10). `KR-IMG`의 2 mm 표기는 **수정 대상**.

### 법정 표시사항

⚠️ 화기 안전 표시 문구는 판매 국가별 의무 사항이 다르다 (미국 / EU CLP / 한국 화학제품안전법).
→ **확인 필요**

---

## 9. 치수

| 항목 | 값 | 출처 |
|---|---|---|
| 유리 외경 | 9 cm | `소영` |
| 유리 내경 | 8 cm | `소영` |
| 전체 높이 (세라믹 뚜껑 포함) | 10 cm | `소영` |
| 유리 단독 높이 | **확인 필요** | — |
| 뚜껑 높이 | **확인 필요** | — |

기존 표기 `11 5/8 * 4 inches` (`US-RAW`, `KR-HTML`)는 라벨이 없어 오해를 부른다.
둘레(29.5 cm)와 높이(10.2 cm)로 해석되며 위 실측값과 정합한다.
→ 고객 노출은 **`지름 9cm × 높이 10cm (뚜껑 포함)`** 형식으로 통일한다.

---

## 10. 가격

| 시장 | 값 | 출처 |
|---|---|---|
| 미국 | USD 85.00 | `US-RAW` variant price |
| 한국 | KRW 127,500 | `KR-HTML` JSON-LD offers |

---

# 확인 필요 항목 정리

| # | 항목 | 필요한 것 |
|---|---|---|
| 1 | oz 표기 | 라벨·패키지 실제 인쇄값 |
| 2 | 향 노트 탑/미들/베이스 구분 | 향료 노트 문서 |
| 3 | Elemi 포함 여부 | 향료사 확인 |
| 4 | 캔들용 향료 코드 | 향료사 확인 (Chemia 78296 여부) |
| 5 | 씨앗 동봉 정책 | 상시 동봉인지 확정 |
| 6 | 유리 단독 높이 / 뚜껑 높이 | 실측 |
| 7 | 왁스 1cm 잔여 기준 | 근거 확인 |
| 8 | Non-GMO · kosher · food-grade 인증서 | Stone Candles 요청 |
| 9 | 화기 안전 표시 문구 | 국가별 의무 사항 확인 |
| 10 | `향초` / `캔들` 표기 통일 | 결정 필요 |
