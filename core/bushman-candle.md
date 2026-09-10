# Bushman Candle Scented Candle — 코어 사실 원장

시장·채널·컨셉과 무관하게 **항상 같아야 하는 사실**만 담는다.
마케팅 표현, 카피, 무드는 이 파일에 넣지 않는다.

- 대상: Bushman Candle **센티드 캔들** (바 솝은 `myrrh-protection-bar.md`)
- 최종 갱신: 2026-09-10
- 원칙: **추측한 값은 넣지 않는다.** 확인하지 못한 항목은 `확인 필요`로 남긴다.
- **용량 · 연소시간 · 왁스 · 심지 · 제조 · 사용법 · 치수 · 가격 · 인증은
  `core/_공통-캔들.md`에 있다.**

## 출처 표기

| 코드 | 출처 |
|---|---|
| `US` | leverden.co — https://leverden.co/products/bushman-candle |
| `KR` | leverden.co.kr — 르버덴 부시맨 센티드 캔들 |
| `US-RAW` | Shopify Admin API 추출본 — `data/shopify-core6-raw.json` (2026-09-09) |
| `KR-HTML` | Cafe24 페이지 원본 HTML (JS 미실행, 2026-09-09 저장) |
| `소영` | 소영님 직접 확인 (2026-09-09~10) |
| `도시어` | leverden Brand Dossier (2026-09-04) |

---

## 1. 제품명

| 항목 | 값 | 출처 |
|---|---|---|
| 영문 | `Bushman Candle Scented Candle` | `소영` 확정 |
| 한글 | `르버덴 부시맨 캔들 센티드 캔들` | `소영` 확정 |
| SKU | `777BCCD10` | `US-RAW` |
| 바코드 | **확인 필요** (등록 안 됨) | `US-RAW` `barcode: null` |
| Shopify handle | `bushman-candle` | `US-RAW` |

### 🔴 이름 규칙 — 반드시 지킬 것

`Bushman Candle / 부시맨 캔들`은 **식물(원료) 이름**이다 (`소영`, 2026-09-10).

- 국문은 **띄어 쓴다.** `부시맨캔들` (X) → `부시맨 캔들` (O)
- 제품명에서 '캔들'이 두 번 반복되어도 **그대로 둔다.**
  앞의 '캔들'은 원료명의 일부, 뒤의 '캔들'은 제품 종류다. 생략하면 뜻이 달라진다.

### 🔴 채널별 표기 불일치

| 위치 | 현재 표기 |
|---|---|
| `US-RAW` product title | `Bushman candle  Scented Candle` (소문자 c + **공백 2칸**) |
| `US-RAW` vendor | `leVerden` — 🔴 구 표기 |
| `KR-HTML` page title | `르버덴 부시맨 센티드 캔들` (원료명 일부 누락) |
| `KR-HTML` JSON-LD name | `르버덴 부시맨 캔들 센티드 캔들` |

→ 정본은 위 표의 값. 나머지 전부 **수정 대상**.

---

## 2. 향 노트

| 단계 | 값 | 한글 | 출처 |
|---|---|---|---|
| 탑 | Olibanum, Pink Peppercorn | 유향 · 핑크 페퍼콘 | `US-RAW` 본문 `The heady blend of… awakens your senses` |
| 미들 | Bushman Candle Oil, Blue Ginger | 부시맨 캔들 오일 · 블루 진저 | `US-RAW` 본문 `leading to a heart of…` |
| 베이스 | Vetiver, Labdanum, Cedarwood | 베티버 · 라브다넘 · 시더우드 | `US-RAW` 본문 `Vetiver, Labdanum, and Cedarwood anchor…` |

원문에 탑/하트/베이스가 명시되어 있어 그대로 옮겼다. 추론 아님.

참고 용어 — **유향(乳香) = Olibanum = Frankincense.** 보스웰리아 나무의 수지.
서늘하고 은은히 달며 나무/수지 느낌. 성당·절의 향 계열.

---

## 3. 원료 산지

| 원료 | 산지 | 출처 |
|---|---|---|
| Bushman Candle Oil | 나미비아 | `소영` (2026-09-10) |
| Blue Ginger | 나미비아 | `소영` (2026-09-10) |

⚠️ **수급 경로 확인 필요.** 힘바 커뮤니티에서 직접 받는지, 향료사(AFM) 경유인지에 따라
   쓸 수 있는 문구가 달라진다.
   - 직접 수급이면 — `힘바족에게서 직접 공수받은 원료`
   - 향료사 경유면 — `나미비아산 원료`
   → **확인 전까지 `나미비아산 원료`까지만 쓴다.**

⚠️ 부시맨 캔들 식물의 학명은 `도시어`에 `Sarcocaulon mossamedense`로 기재되어 있으나,
   향료의 `Bushman Candle Oil`과 동일 원료인지 **확인 필요**.

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

🔴 **한국 사이트에 씨앗 별도 판매 문구가 남아 있다.**

| 위치 | 문구 |
|---|---|
| `KR-HTML` JSON-LD description | `컬렉션을 연상시키는 나미비아 선인장 씨앗을 별도  판매합니다` |

→ 현재 판매하지 않으므로 **삭제 대상**. (띄어쓰기 오류 `별도  판매`도 함께 있음)

---

## 6. 기부 — 확인 필요

| 항목 | 값 | 출처 | 상태 |
|---|---|---|---|
| 수익 일부를 Cheetah Conservation Fund에 기부 | — | `도시어` | **확인 필요** |

⚠️ 기부 문구는 근거가 확실해야 한다. 현재도 유효한지 확인 전까지 카피에 쓰지 않는다.

---

## 7. 전통지식(TK) 취급 — 주의

⚠️ 힘바족의 전통적 사용에 관한 서술은 **나미비아 ABS(나고야 의정서) 법제 대상**이다.
   OPF/KCINPT가 문서화한 범위(INP-book)와 대조할 것.
   **문서화되지 않은 내용을 새로 서술하지 않는다.**

→ 상세: `docs/myrrh-sourcing.md`

---

## 8. 이 제품에만 있는 수정 대상

| 위치 | 문구 | 문제 |
|---|---|---|
| `US-RAW` 본문 | `Boost your energy and ignite your creativity` | 효능 표현. 삭제 |
| `US-RAW` 본문 | `each note is chosen… for its energetic properties` | 향료 효능 주장. 삭제 |
| `US-RAW` 본문 | `sparks a surge of creativity` | 효능 표현. 삭제 |
| `US-RAW` 본문 | `creating a serene and toxin-free environment` | 무독성 주장. 삭제 |
| `US-RAW` SEO description | `Purify your environment` | 공기 정화 = 효능 표현. 삭제 |
| `US-RAW` SEO description | 4종 중 3종이 **동일한 문장**을 공유 | 제품별로 다시 쓸 것 |
| `US-RAW` vendor | `leVerden` | 🔴 구 브랜드 표기. `leverden`으로 수정 |
| `US-RAW` product title | `Bushman candle  Scented Candle` | 대소문자 + 공백 2칸 오류 |
| `US-RAW` metafields | `custom.advantages_paragraph` = Amethyst Ki Bath Soak 설명 | 다른 제품 내용. 삭제 |
| `US-RAW` metafields | `img_w_txt_richtext_3` = 배스 솔트 전성분 (`FD&C red 40` 등) | 캔들과 무관. 삭제 |
| `US-RAW` metafields | `custom.subheading` / `img_w_txt_section_richtxt_5` = `lorem ipsum` | 더미 텍스트. 삭제 |
| `US-RAW` metafields | `Consicientious` | 오타 (정: Conscientious) |
| `KR-HTML` JSON-LD description | `제품 개봉 및 사용시 교환/반품은 불가합니다`로 시작 | 순서 조정 |

---

# 확인 필요 항목 (이 제품)

| # | 항목 | 필요한 것 |
|---|---|---|
| 1 | 나미비아 원료 수급 경로 | 직접 수급 / 향료사 경유 확인 → 쓸 수 있는 문구가 달라짐 |
| 2 | 부시맨 캔들 식물 학명 | 향료사 확인 (`Sarcocaulon mossamedense` 대조) |
| 3 | Cheetah Conservation Fund 기부 | 현재 유효 여부 |
| 4 | 바코드 | 미등록 상태 |
| 5 | TK 문서화 범위 | OPF/KCINPT INP-book 대조 |

공통 확인 필요 항목은 `core/_공통-캔들.md` 하단 참조.
