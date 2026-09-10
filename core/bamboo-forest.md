# Bamboo Forest Scented Candle — 코어 사실 원장

시장·채널·컨셉과 무관하게 **항상 같아야 하는 사실**만 담는다.
마케팅 표현, 카피, 무드는 이 파일에 넣지 않는다.

- 대상: Bamboo Forest **센티드 캔들** (바 솝은 `bamboo-forest-bar.md`)
- 최종 갱신: 2026-09-10
- 원칙: **추측한 값은 넣지 않는다.** 확인하지 못한 항목은 `확인 필요`로 남긴다.
- **용량 · 연소시간 · 왁스 · 심지 · 제조 · 사용법 · 치수 · 가격 · 인증은
  `core/_공통-캔들.md`에 있다.** 여기에 중복 기재하지 않는다.

## 출처 표기

| 코드 | 출처 |
|---|---|
| `US` | leverden.co — https://leverden.co/products/bamboo-forest-scented-candle |
| `KR` | leverden.co.kr — 르버덴 뱀부 포레스트 센티드 캔들 |
| `US-RAW` | Shopify Admin API 추출본 — `data/shopify-core6-raw.json` (2026-09-09) |
| `KR-HTML` | Cafe24 페이지 원본 HTML (JS 미실행, 2026-09-09 저장) |
| `KR-IMG` | Cafe24 상세페이지 이미지 |
| `소영` | 소영님 직접 확인 (2026-09-09~10) |
| `도시어` | leverden Brand Dossier (2026-09-04) |

---

## 1. 제품명

| 항목 | 값 | 출처 |
|---|---|---|
| 영문 | `Bamboo Forest Scented Candle` | `US-RAW` product title |
| 한글 | `르버덴 뱀부 포레스트 센티드 캔들` | `KR-HTML` JSON-LD name, page title |
| 브랜드 표기 | `leverden` (전부 소문자) / `르버덴` | `소영`, `도시어` §11 |
| SKU | `777BFCD10` | `US-RAW` |
| 바코드 | `850034664026` | `US-RAW` |
| Shopify handle | `bamboo-forest-scented-candle` | `US-RAW` |

⚠️ `KR-IMG`에는 `센티드 향초` 형식이 쓰인 제품이 있어 **`향초` / `캔들` 표기가 매체별로 다르다.**
→ 통일 방향 **확인 필요** (공통 C7)

---

## 2. 향 노트

| 항목 | 값 | 출처 |
|---|---|---|
| 전체 노트 | Basil, Spearmint, Sage, Coriander, Immortelle, Sandalwood, Tonka, Amber | `US-RAW` SEO description `Fragrance Notes` |
| 한글 | 바질, 스피어민트, 세이지, 코리앤더, 임모르텔, 샌달우드, 통카, 앰버 | 위 항목 번역 |
| **탑 / 미들 / 베이스 구분** | **확인 필요** | — |

⚠️ 원 자료에는 **평면 목록으로만** 존재한다. 단계 구분이 문서로 확인되지 않았다.
   (부시맨 캔들·샤먼·밸리 오브 로지즈는 원문에 단계가 명시되어 있으나, 이 제품만 없다.)
   → 향료 노트 문서 확인 필요

### 원 자료에 함께 등장하나 노트로 확정되지 않은 원료

| 원료 | 등장 위치 | 판단 |
|---|---|---|
| Elemi | `US-RAW` product_info 서술형 Fragrance Notes 문단 | 확인 필요 |
| Oakmoss, Fir Balsam | `US-RAW` `About the Perfumer` 문단 | **노트 아님.** 이 문단은 캔들과 바 솝에 동일하게 복붙되어 있어 근거가 되지 못한다 |

⚠️ Oakmoss는 **바디 라인 향료** `BAMBOOM 34`(IFF 6059239)에 1.218% 포함되어 있음이
   알레르겐 선언서로 확인되었으나, **캔들 향료 문서에서는 확인되지 않았다.**
   Bamboo Forest는 캔들과 바디의 향료 회사가 아예 다르다 (Chemia vs IFF).
   상세: `docs/fragrance-registry.md`

---

## 3. 조향

| 항목 | 값 | 출처 |
|---|---|---|
| 조향사 | Christophe Laudamiel | `도시어` §03 |

⚠️ `US-RAW` 본문 `Laudimiel`은 오타. 정확한 표기는 **Laudamiel**.

---

## 4. 동봉품

| 항목 | 값 | 출처 |
|---|---|---|
| 세라믹 뚜껑 | 포함 | `소영` |
| 코리앤더 씨앗 | **동봉하지 않음** | `소영` (2026-09-10 확정) |

🔴 **양쪽 사이트에 아직 동봉 문구가 남아 있다. 삭제 대상.**

| 위치 | 문구 |
|---|---|
| `US-RAW` product_info Description | `Comes with a packet of Coriander seeds reminiscent of the Collection scent` |
| `US-RAW` Sustainable Packaging 문단 | `cultivate new life with the plant seed packets that are included and shipped in every candle` |
| `KR-HTML` JSON-LD description | `컬렉션 향을 연상시키는 코리앤더 씨를 함께 제공합니다` |

→ 동봉하지 않는데 동봉된다고 표기하는 것은 표시광고 위반이다.

---

## 5. 이 제품에만 있는 수정 대상

| 위치 | 문구 | 문제 |
|---|---|---|
| `US-RAW` 본문 | `Purifies the environment` | 공기 정화 = 효능 표현. 삭제 |
| `US-RAW` SEO / 본문 | `the most sustainable candle wax in the earth` | 최상급 무근거 주장. 삭제 |
| `US-RAW` SEO | `designed to purify the environment` | 위와 동일. 삭제 |
| `US-RAW` product_info Sustainable Packaging | light4life / Exceptional Children's Foundation 파트너십 | 4종 중 이 제품에만 기재. **현재도 유효한지 확인 필요** |
| `KR-HTML` JSON-LD description | `제품 개봉 및 사용시 교환/반품은 불가합니다`로 시작 | 검색결과 첫 문장이 반품 안내. 순서 조정 |
| `US-RAW` metafields | `custom.subheading` 등에 `lorem ipsum` 더미 텍스트 잔존 | 삭제 |
| `US-RAW` metafields | `custom.advantages_paragraph`가 **Amethyst Ki Bath Soak** 설명 | 다른 제품 내용. 삭제 |
| `US-RAW` metafields | `advantages_heading_2` = `Exfoliate`, `_4` = `Minerals` | 캔들에 각질제거·미네랄. 삭제 |
| `US-RAW` metafields | `Consicientious` | 오타 (정: Conscientious) |

---

# 확인 필요 항목 (이 제품)

| # | 항목 | 필요한 것 |
|---|---|---|
| 1 | 향 노트 탑/미들/베이스 구분 | 향료 노트 문서 (Chemia) |
| 2 | Elemi 포함 여부 | 향료사 확인 |
| 3 | light4life 파트너십 유효 여부 | 확인 후 유지/삭제 결정 |
| 4 | ~~씨앗 동봉~~ | ✅ 동봉하지 않음 확정. **양쪽 사이트 문구 삭제 필요** |
| 5 | ~~캔들용 향료 코드~~ | ✅ 기록 대상 아님 |

공통 확인 필요 항목은 `core/_공통-캔들.md` 하단 참조.
