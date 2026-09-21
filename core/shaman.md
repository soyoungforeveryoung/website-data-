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
| 탑 | Peruvian sage (Artemisia), Cypress | 페루산 세이지(아르테미시아) · 사이프러스 | `US-RAW` 본문 + AFM PIF 원료표 |
| 미들 | Palo Santo accord, Geranium | 팔로 산토 어코드 · 제라늄 | `US-RAW` 본문 — 향의 캐릭터명, 실제 원료 아님 |
| 베이스 | Sandalwood, Vetiver | 샌달우드 · 베티버 | `US-RAW` 본문 `the base notes of Sandalwood and Vetiver oil` |

✅ 2026-09-19 정정 (소영님 확인): 아래 §3 참조.

---

## 3. 팔로 산토 — ✅ 해결됨 (2026-09-19): 원료가 아니라 콜렉션 테마다

**뱀부 포레스트가 왁스에 실제 대나무를 쓰지 않는 것과 같은 구조다.**
샤먼 캔들은 "팔로 산토 리추얼"에서 **영감을 받아 만든 향**이지,
팔로 산토가 원료로 들어가는 게 아니다.

| 항목 | 값 | 출처 |
|---|---|---|
| 실제 TOP 원료 | **페루산 아르테미시아(세이지)** | `소영` (2026-09-19 확인) |
| 팔로 산토 지위 | 콜렉션 영감/테마. 원료 아님 | `소영`, AFM PIF 원료표 대조 |
| AFM PIF 원료표 확인 결과 | `Bursera graveolens`(팔로 산토) **없음**. 주 원료는 `Juniperus Virginiana Oil`(버지니아 시더) 8.33% 등 | AFM PIF/알레르겐 문서 (2025-01-10 수신) |

### 🔴 위 발견에 따라 폐기된 이전 항목들

과거에 팔로 산토를 '원료'로 다루면서 남겨뒀던 항목들 — 원료가 아님이
확인되어 더 이상 진행하지 않는다.

- ~~자연 낙목만 채취 (naturally fallen wood only) — `도시어` 근거~~ → **삭제 대상 문구.**
  KR/EN 라이브 페이지의 "저희가 쓰는 팔로 산토는 자연적으로 쓰러진 나무에서만
  얻습니다. 베어내지 않습니다" 문장은 실제 원료가 아닌 것에 대한 구체적
  수급 주장이라 근거가 없다. **삭제.**
- ~~팔로 산토 학명 확인~~ → 원료가 아니므로 학명 확인 자체가 의미 없어짐
- ~~자연 낙목 채취 공급처 확인서~~ → 대상 없음
- ~~페루 수출 서류(SERFOR 등)~~ → 대상 없음

### ✅ 유지되는 서사

"페루 샤먼들이 팔로 산토를 태워 공간을 정돈한다"는 **문화적 전통 서술**은
그대로 유지한다 (콜렉션 영감의 출처를 설명하는 것이지, 원료 주장이 아니므로).
다만 그 뒤에 붙는 **구체적 수급 방식 문장은 삭제**하고, 실제 원료 서사는
**페루산 세이지(아르테미시아)**로 옮긴다.

---

## 4. 조향

| 항목 | 값 | 출처 |
|---|---|---|
| 조향사 | Antoine Lie | `도시어` §03 |
| 향료사 | **AFM** — Atelier Fragranze Milano (이탈리아) | `소영` |
| 향료 | `SPIRITUAL WOOD` (28782) — **캔들 향** | IFRA 인증서, `소영` |

부시맨 캔들과 같은 관계다. AFM 대표 **Luca Maffei** + 조향 **Antoine Lie**.
서류 담당은 **Mara Maghini**. AFM 내부 문서번호는 `AFM-2228782`.

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
| 1 | ~~팔로 산토 학명~~ | ✅ 해결 (2026-09-19) — 원료 아님, §3 참조 |
| 2 | ~~자연 낙목 채취 근거~~ | ✅ 해결 (2026-09-19) — 대상 없음, §3 참조 |
| 3 | ~~페루 수출 서류~~ | ✅ 해결 (2026-09-19) — 대상 없음, §3 참조 |
| 4 | 바코드 | 미등록 상태 |

공통 확인 필요 항목은 `core/_공통-캔들.md` 하단 참조.
