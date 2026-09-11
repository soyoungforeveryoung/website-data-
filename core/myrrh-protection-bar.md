# Bushman Candle Myrrh Protection Bar — 코어 사실 원장

시장·채널·컨셉과 무관하게 **항상 같아야 하는 사실**만 담는다.
마케팅 표현, 카피, 무드는 이 파일에 넣지 않는다.

- 대상: Bushman Candle **미르 프로텍션 바 솝** (캔들은 `bushman-candle.md`)
- 최종 갱신: 2026-09-10
- 원칙: **추측한 값은 넣지 않는다.** 확인하지 못한 항목은 `확인 필요`로 남긴다.
- **중량 · 제조 · 로프 · 가격 · 사용법 · 표시사항은 `core/_공통-바솝.md`에 있다.**

## 출처 표기

| 코드 | 출처 |
|---|---|
| `US` | leverden.co — https://leverden.co/products/myrrh-protection-bar |
| `KR` | leverden.co.kr — 부시맨 캔들 미르 프로텍션 바 |
| `US-RAW` | Shopify Admin API 추출본 — `data/shopify-core6-raw.json` (2026-09-09) |
| `KR-HTML` | Cafe24 페이지 원본 HTML (JS 미실행, 2026-09-09 저장) |
| `소영` | 소영님 직접 확인 (2026-09-09~10) |
| `공급사` | KCINPT 제품 도시에 + 2022년 수급 메일 (`docs/myrrh-sourcing.md`) |

---

## 1. 제품명

| 항목 | 값 | 출처 |
|---|---|---|
| 영문 | `Bushman Candle Myrrh Protection Bar` | `US-RAW` product title |
| 한글 | `르버덴 부시맨 캔들 미르 프로텍션 바` | `소영` 확정 |
| SKU | `111BCBS10` | `US-RAW` |
| 바코드 | `850034664378` | `US-RAW` |
| Shopify handle | `myrrh-protection-bar` | `US-RAW` |

제품명은 **기존 이름을 유지한다** (`소영`, 2026-09-10).
개명(Oasis 등)을 검토했으나 브랜드에 맞지 않아 원래 이름으로 확정했다.

### 🔴 `Protection`이라는 말의 사용 범위

| 안전 | 금지 |
|---|---|
| 힘바족이 사막의 햇빛과 건조함 속에서 몸에 발라온 향 | 피부를 보호합니다 / protects your skin / 자외선 차단 |

⚠️ **반드시 힘바족의 전통적 사용이라는 문화적 맥락으로 한정한다.**
   피부 보호 '효과'로 읽히게 쓰면 화장품 효능 표현이 된다.

### 🔴 채널별 표기 불일치

| 위치 | 현재 표기 |
|---|---|
| `KR-HTML` page title | `leverden \| 부시맨 캔들 미르 프로텍션 바` |
| `KR-HTML` JSON-LD name | `부시맨 캔들 미르 프로텍션 바` |

→ 이 제품만 title 형식이 다르고(`leverden |` 접두), **JSON-LD에 `르버덴`이 아예 없다.**

⚠️ `US-RAW` productType이 `barsoap`(한 단어)이다. 차콜 바는 `Bar Soap`. **통일 필요.**

---

## 2. 향 노트

| 항목 | 값 | 출처 |
|---|---|---|
| **탑 / 미들 / 베이스 구분** | **확인 필요** | — |
| 전체 노트 | **확인 필요** | — |

🔴 **이 제품은 향 노트가 문서로 확인되지 않았다.**
   `US-RAW`에 있는 것은 서술형 표현뿐이다 (`The warm, resinous Myrrh aroma`).

⚠️ **캔들의 노트를 그대로 가져다 쓰면 안 된다.** 배합이 다르다.
   특히 캔들에는 **유향(Olibanum)**, 바 솝에는 **몰약(Myrrh)**이 들어간다. 서로 다른 원료다.

---

## 3. 전성분 (INCI)

> Sodium hydroxide, Cocos nucifera (coconut) oil, Aqua (water),
> Helianthus annuus (sunflower) seed oil, Olea europaea (olive) fruit oil,
> Simmondsia chinensis (jojoba) seed oil, Ricinus communis (castor) seed oil,
> Prunus amygdalus dulcis (sweet almond) oil, Butyrospermum parkii (shea) butter,
> **Commiphora Wildii Oil**, Fragrance (parfum)

출처: `US-RAW` `custom.pdp_ingredients` (아래 정정 반영본)

### 🔴 정정 사항

| 항목 | 사이트 현재 값 | 정확한 값 |
|---|---|---|
| 몰약 학명 | `Myrrh (Commiphora myrrha) oil` | **`Commiphora Wildii Oil`** |
| 스위트 아몬드 | `Prunus armgd­alus dulcis` | `Prunus amygdalus dulcis` |

🔴 **몰약 학명이 틀렸다.** 실제 원료는 나미비아 고유종 `Commiphora wildii`(통칭 **Omumbiri**)이며,
   일반 몰약 `Commiphora myrrha`와 **다른 종이다.** 공급사 도시에로 확인됨.
   상세: `docs/myrrh-usable.md`

⚠️ 원문 `Prunus armgd­alus`에는 오타와 함께 **보이지 않는 soft hyphen 문자**가 섞여 있다.
   복사해서 쓸 때 그대로 딸려간다. 새로 타이핑할 것.

⚠️ **견과류(sweet almond) 함유.** 알레르기 고지 필요 여부 **확인 필요**.

---

## 4. 히어로 원료 — 힘바족 몰약(Omumbiri)

| 항목 | 값 | 출처 |
|---|---|---|
| 원료 | `Commiphora wildii` 오일 (Omumbiri) | `공급사` |
| 산지 | 나미비아 사막 | `공급사`, `US-RAW` |
| 수급 경로 | 힘바 커뮤니티 트러스트(KCINPT) → Opuwo Processing Facility → leverden | `공급사` (2022년 수급 메일) |
| 전통적 용법 | 힘바족이 강한 햇빛과 사막의 건조함 속에서 피부에 발라 온 원료 | `소영`, `US-RAW` |

🔑 **이 제품의 존재 이유는 두 가지다. 어느 쪽도 생략하지 않는다.**
1. 힘바족이 왜 몰약을 쓰는가 — 햇빛과 건조함
2. **직접 수급** — 중간 유통이 아니라 힘바 커뮤니티에서 직접 받는다

⚠️ 기존 표기 `in collaboration with the Himba tribe's ancestral rituals`는 **모호하다.**
   무엇을 협업했다는 것인지 알 수 없다. 위 사실관계로 교체할 것.

⚠️ `tribe` 단독 표현보다 `the Himba people` / `the Himba`를 우선한다.

⚠️ **직접 수급을 광고에 쓰려면 거래 형태(공정무역, 수익 배분 등)를
   문서로 갖고 있는 편이 안전하다.** → 확인 필요

---

## 5. 전통지식(TK) 취급 — 주의

⚠️ 힘바족의 전통적 사용에 관한 서술은 **나미비아 ABS(나고야 의정서) 법제 대상**이다.
   OPF/KCINPT가 문서화한 범위(INP-book)와 대조할 것.
   **문서화되지 않은 내용을 새로 서술하지 않는다.**

→ 상세: `docs/myrrh-sourcing.md`

---

## 6. 이 제품에만 있는 수정 대상

| 위치 | 문구 | 문제 |
|---|---|---|
| `US-RAW` 등록 중량 | **0.2 lb (약 91 g)** | 🔴 **명백한 오류. 250 g으로 수정** |
| `US-RAW` SEO description | **없음 (`null`)** | 🔴 SEO 설명 자체가 비어 있다 |
| `US-RAW` `custom.pdp_ingredients` | `Commiphora myrrha` | 🔴 학명 오류 → `Commiphora Wildii Oil` |
| `US-RAW` `custom.pdp_ingredients` | `Prunus armgd­alus` + soft hyphen | 오타 + 보이지 않는 문자 |
| `US-RAW` 본문 | `a natural way to protect the skin from harsh sunlight` | 🔴 피부 보호 효능 표현. 문화적 맥락으로 한정 |
| `US-RAW` 본문 | `delivering the soothing, moisturizing benefits` | 화장품 효능 표현. 근거 필요 |
| `US-RAW` 본문 | `Hand-poured by our artisan soap maker` | 🔴 `hand-poured`는 캔들 용어. 비누는 `handmade` |
| `US-RAW` 본문 | `Leverden` (대문자 L) | 🔴 브랜드 표기는 전부 소문자 `leverden` |
| `US-RAW` `custom.pdp_good_to_know` | `will help you feel grounded and energized` | 효능 표현. 삭제 |
| `US-RAW` `custom.pdp_why_you_ll_love_it` | `efficient skincare performance` | 효능 표현. 근거 필요 |
| `US-RAW` productType | `barsoap` | 차콜 바(`Bar Soap`)와 불일치 |
| `KR-HTML` JSON-LD description | `나미비아 데저트의 미르 를 사용한…` (32자) | 🔴 6종 중 가장 짧다 + `미르 를` 띄어쓰기 오류 |
| `KR-HTML` page title | `leverden \| ` 접두 | 다른 제품과 형식 불일치 |
| `KR-HTML` JSON-LD name | `르버덴` 누락 | 추가 |
| `KR-HTML` 상세 이미지 | **1장** (다른 제품은 3~4장) | 보강 필요 |
| `KR-HTML` 상세 이미지 alt | **`alt` 속성 자체가 없음** | 🔴 완전한 공백. 추가 |
| `KR-HTML` JSON-LD | `availability` 필드 없음 | 추가 |

🔴 **6종 중 가장 최근에 등록된 제품인데 정보가 가장 부실하다.**

---

# 확인 필요 항목 (이 제품)

| # | 항목 | 필요한 것 |
|---|---|---|
| 1 | 향 노트 전체 + 탑/미들/베이스 | 향료사 노트 문서 — **캔들 노트로 대체 금지** |
| 2 | 견과류(아몬드) 알레르기 고지 | 국가별 요건 확인 |
| 3 | 힘바족 거래 형태 문서 | 공정무역·수익 배분 명문화 가능 여부 |
| 4 | TK 문서화 범위 | OPF/KCINPT INP-book 대조 |
| 5 | Shopify 중량 | 🔴 0.2 lb → 250 g |
| 6 | SEO description | 현재 비어 있음 |

공통 확인 필요 항목은 `core/_공통-바솝.md` 하단 참조.
