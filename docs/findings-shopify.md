# Shopify (leverden.co) 데이터 조사 결과

- 조사일: 2026-09-09
- 대상: 코어 6종
- 원본: `data/shopify-core6-raw.json`

## 🔴 심각 — 고객에게 잘못된 정보가 노출 중

### 1. 바 솝 페이지에 바디로션 SEO 정보
`Bamboo Forest Charcoal Detox Bar`의 SEO 타이틀·설명이 **전혀 다른 제품**의 것.

```
현재 title : Bamboo Salt Body Lotion - leverden
현재 desc  : Moisturize and soften your skin instantly with bamboo salt body lotion...
```
→ 검색결과와 SNS 공유 카드에 "바디로션"으로 뜬다.

### 2. Shaman 캔들에 Bushman 캔들 SEO 정보
`Shaman Scented Candle`과 `Bushman Candle Scented Candle`의 SEO 타이틀·설명이 **완전히 동일**.

```
양쪽 모두 : Coconut Wax, Apricot Oil and Namibian Incense Scented Candle - leVerden
```
→ Namibian Incense는 Bushman 콜렉션 설명. Shaman에는 맞지 않음.
→ 게다가 이 문구에 폐기된 표기 `leVerden`이 들어있음.

### 3. 캔들 4종에 배스솔트 성분표가 들어가 있음
캔들 4종 모두 `custom.img_w_txt_richtext_3`(COMPOSITION 섹션)에 아래 값이 들어있다.

```
Sodium Chloride, Fragrance, Magnesium Sulfate, Water, Propylene Glycol,
FD&C red 40, FD&C blue 1, FD&C yellow 5, Linalool, Eugenol, Limonene, Cinnamal
```
→ 이것은 **Amethyst Ki 배스솔트**의 성분. 캔들 성분이 아니다.
→ 같은 자리 `advantages_paragraph`, `img_w_txt_richtext_2`에도 배스솔트 카피가 복사되어 있음.
→ 인공색소(FD&C) 표기가 캔들에 붙어 있는 상태라 클레임 리스크가 있다.

### 4. Lorem ipsum 더미 텍스트가 라이브
캔들 4종 공통.
```
custom.subheading                  : loremloremloremloremlorem...
custom.img_w_txt_section_richtxt_5 : Lorem ipsum dolor sit amet, consectetur...
```

### 5. 테스트 문구 라이브
```
Bamboo Forest Charcoal Detox Bar
custom.pdp_accordion_description : "Test description for Charcoal Bar"
```

## 🟡 일관성 — 코어팩트 위반

| 항목 | 현재 상태 | 조치 |
|---|---|---|
| 브랜드명 | `leverden` / `leVerden` 혼재 (Bushman·Shaman 캔들이 `leVerden`) | 전부 `leverden` |
| Product type | `Bar Soap` / `barsoap` 혼재 | 전부 `Bar Soap` |
| 제품명 | `Bushman candle  Scented Candle` — 공백 2칸 + 소문자 c | `Bushman Candle Scented Candle` |
| Barcode | 캔들 4종 중 1종만 등록 (Bamboo Forest) | 4종 전부 등록 |
| Barcode 형식 | Charcoal Bar만 `00850034664101` (앞 0 두 개) | GTIN 자릿수 통일 |
| SKU 형식 | Valley of Roses만 `777TVRCD10` (T 접두) | 의도 확인 후 통일 |
| SEO | Myrrh Protection Bar는 타이틀·설명 아예 없음 | 작성 |
| 바 솝 중량 | Charcoal 0.6 lb vs Myrrh 0.2 lb (3배 차이) | **Myrrh Bar가 오류.** 2종 모두 순중량 **255g** 확정 → Myrrh 등록 중량 수정 필요 |

## 🔴 캔들 라인과 바디 라인의 향 정보가 섞여 있음

`About the Perfumer` 문단이 **Bamboo Forest 캔들과 바 솝에 동일하게 복붙**되어 있고,
그 안의 원료명(Oakmoss, Fir Balsam)이 캔들 노트인 것처럼 읽힌다.

→ 캔들과 바디는 향 배합이 서로 다르다. 같은 콜렉션명이라도 노트를 공유하지 않는다.
→ 조향 서사 문단과 노트 목록을 분리하고, 라인별로 다르게 작성해야 한다.
→ 향료사에 캔들/바디 각각의 배합 확인 요청 필요.

## 🟡 오타

| 위치 | 현재 | 정정 |
|---|---|---|
| 캔들 4종 `advantages_heading_3` | Consicientious | Conscientious |
| Valley of Roses SEO | Morocccan | Moroccan |
| Charcoal Bar 성분 | bermot | bergamot |
| Myrrh Bar 성분 | Prunus armgd­alus (보이지 않는 soft hyphen 포함) | Prunus amygdalus |
| 조향사 소개 본문 | Laudimiel | Laudamiel |

## 🔴 씨앗 동봉 문구 — 실제로는 동봉 안 함

씨앗 패킷 동봉은 **중단되었으나** Bamboo Forest 캔들에 아래 문구가 그대로 살아있다.

```
Comes with a packet of Coriander seeds reminiscent of the Collection scent
...cultivate new life with the plant seed packets that are included and shipped in every candle
```

→ 동봉하지 않는데 동봉된다고 표기 중. **표시광고 위반이자 실제 클레임 사유**다.
→ 최우선 삭제 대상.

## 🔴 왁스 표기 — 제조사 사양과 불일치

제조사 Stone Candles 공개 사양에는 **soy wax와 stearic acid가 포함**되어 있으나
현재 카피는 코코넛과 애프리컷만 언급한다. 상세: `data/supplier/stone-candles-wax.md`

| 항목 | 제조사 원문 | 현재 표기 | 조치 |
|---|---|---|---|
| 구성 | coconut apricot wax, **soy wax, stearic acid**, apricot oil | 소이·스테아릭산 누락 | 배합비 확인 후 정정 |
| non-GMO | **coconut**에 한정 | 인증 근거 없음 | 인증서 확보 전까지 문구 내림 |
| food grade | **coconut oil**에 한정 | `food-grade coconut wax` | `푸드 그레이드 인증 코코넛 오일 사용`으로 정정 |

⚠️ **"소이가 아니라 코코넛"식 차별화 문구는 쓰면 안 된다.** 소이가 들어간다.
⚠️ 인증 문구(non-GMO·kosher·food grade)는 제조사 마케팅 문구일 뿐 인증서가 아니다.
   leverden 이름으로 쓰려면 발급기관·번호가 있는 실제 인증서를 받아야 한다.

## 🟡 사양 변경 미반영

- 캔들 용량이 **250g**으로 변경되었으나 사이트에 반영 안 됨. → 6종 전체 수정 필요
- `Burning time: 60 hours` → 유효. 그대로 유지하되 `약(approx.)` 표기 추가.
- `Dimensions: 11 5/8 * 4 inches` → 둘레×높이였음. `지름 9cm × 높이 10cm (뚜껑 포함)`으로 교체.
- 세라믹 뚜껑·싱글 오가닉 코튼 심지·80% 충전 → **전부 누락**. 추가 필요.

## 🟡 리뷰 데이터 이중화

같은 제품에 두 개의 리뷰 앱 데이터가 서로 다른 값으로 존재.

| 제품 | Junip | Judge.me |
|---|---|---|
| Bamboo Forest Charcoal Detox Bar | 평점 5.0 / 2건 | 평점 4.86 / 59건 |
| Bamboo Forest Scented Candle | 평점 4.73 / 15건 | — |

→ 어느 앱을 정본으로 쓸지 결정하고 한쪽으로 통합해야 한다.

## ✅ 확정됨 — 원산지

| 라인 | 원산지 | 영문 표기 | 국문 표기 |
|---|---|---|---|
| 캔들 4종 | 미국 | `Hand-poured in California, USA` | 미국 캘리포니아 제조 |
| 바 솝 2종 | 한국 | `Handmade in Korea` | 한국 제조 |

⚠️ 라인별로 원산지가 다르다. **세트 상품**(Mini Ritual Set 등)은 구성품별로 각각 표기해야 한다.
⚠️ 현재 Charcoal Bar에는 원산지 표기가 아예 없다 → 추가 필요.

## ✅ 확정됨 — 캔들 베슬 사양

| 항목 | 값 |
|---|---|
| 전체 높이 (세라믹 뚜껑 포함) | 10 cm |
| 유리 외경 / 내경 | 9 cm / 8 cm (벽 두께 약 5mm) |
| 내부 깊이 | 약 7 cm |
| 왁스 | 250 g · 높이 약 5.5 cm · **80% 충전** |
| 뚜껑 | 세라믹 |

⚠️ 현재 Shopify에는 이 정보가 **하나도** 없거나 틀리게 들어가 있다.
⚠️ 세라믹 뚜껑은 Shopify 어디에도 언급이 없다 → 프리미엄 요소인데 누락 중.

## ⚪ 확인 필요 (원장의 pending 항목)

- Bushman·Shaman 캔들 향 노트 전문
- 캔들 3종(Bushman·Shaman·Valley of Roses) 동봉 씨앗 종류
- 조향사가 6종 전부 Christophe Laudamiel인지
- Myrrh Bar의 sweet almond(견과류) 알레르기 고지 필요 여부

## 🟡 제품 명칭 불일치 — soap on a rope

로프 달린 바 솝의 명칭이 제품마다 다르게 쓰여 있다.

| 제품 | 현재 표기 |
|---|---|
| Bamboo Forest Charcoal Detox Bar | `handmade luxury soap-on-a-rope` ✅ |
| Bushman Candle Myrrh Protection Bar | `hanging linen-blend rope for simple display` ❌ |
| Charcoal Bar (Good to Know) | `Hanging-linen composition natural rope` ❌ |

→ 전부 `soap on a rope`로 통일. 로프 소재는 뒤에 덧붙여 설명.
→ 규칙: `brand/brand-core.md` §3-1


---

# 2026-09-15 수정 반영분

## 중량 오류 정정

| 제품 | 전 | 후 |
|---|---|---|
| **Bushman Candle Myrrh Protection Bar** | `0.2 lb` (약 91 g) | **`0.6 lb`** (약 272 g) |

0.2 lb 는 실제 제품(250 g + 로프·포장)의 1/3 수준으로 명백한 오류였다.
같은 규격인 차콜 디톡스 바가 `0.6 lb` 이므로 동일하게 맞췄다.
→ 배송비 계산이 실제보다 낮게 잡히던 문제가 해소된다.

## 중량 검증 결과 — 나머지는 이상 없음

| 제품 | 등록 중량 | 판정 |
|---|---|---|
| 캔들 4종 | 2.3 lb (약 1,043 g) | ✅ 4종 모두 동일. 일관됨 |
| 차콜 디톡스 바 | 0.6 lb (약 272 g) | ✅ 250 g + 포장. 타당 |
| 바 솝 듀오 3종 | 1.2 lb | ✅ 0.6 × 2. 계산 맞음 |
| 미니 리추얼 세트 | 0.8 lb | ✅ 바 0.6 + 미니 틴 0.2. 타당 |
| 트래블 리추얼 틴 | 0.1 lb | 🟡 1.56 oz(44 g) 제품. 포장 포함이면 다소 낮아 보임 → `확인 필요` |

## SEO 비어 있던 5개 제품 채움

아래 제품은 SEO 제목·설명이 **둘 다 null** 이었다. 검색 결과에 본문이 잘려 노출되던 상태다.

| 제품 | 새 SEO 제목 |
|---|---|
| Bushman Candle Myrrh Protection Bar | Myrrh Protection Bar \| Namibian Wild Myrrh Soap - leverden |
| Charcoal Detox Bar Duo Set | Charcoal Detox Bar Duo Set \| Two Bars - leverden |
| Myrrh Protection Bar Duo Set | Myrrh Protection Bar Duo Set \| Two Bars - leverden |
| Ritual Cleansing Bar Duo | Ritual Cleansing Bar Duo \| Charcoal + Myrrh - leverden |
| Bamboo Forest Mini Ritual Set | Bamboo Forest Mini Ritual Set \| Tin Candle + Bar - leverden |

설명문에는 확정된 사실만 넣었다: 250 g, 손 장인 제작, 한 달 건조,
`Commiphora wildii`, 힘바 커뮤니티 수급, 파라핀 무첨가, 스위트아몬드(견과류) 고지.
**효능 주장은 쓰지 않았다.**

## 🟡 남은 항목

- **트래블 리추얼 틴** 중량 0.1 lb 확인
- 듀오 세트 본문에 `detoxify` · `purification` · `deeply purifies` 표현이 남아 있다.
  비누 세정 맥락이라 캔들의 `Purifies the environment` 보다는 약하지만
  기능성 미신고 제품에 쓰기엔 재검토 여지가 있다 → 소영님 판단 필요
- 듀오 세트 본문에 `Hand-poured` 표현이 있다. **비누는 붓는 것이 아니다.**
  `Handcrafted` 로 바꾸는 것이 정확하다 → 소영님 확인 후 수정

---

## 2026-09-15 추가 — 효능 표현 정리 (`소영` 승인)

### 원칙

| 쓸 수 있는 말 | 쓸 수 없는 말 |
|---|---|
| `cleanse` · `wash` — 비누가 실제로 하는 일 | `detoxify` (해독) · `purify` (정화) — **신체 기능 주장** |
| `nourish` · `moisturize` · `hydrate` — 화장품 일반 표현 | 기능성 미신고 제품에 쓰면 표시광고 위반 소지 |

한국 화장품법상 비누는 **인체세정용 제품류**다. 세정 외의 작용을 단언할 수 없다.
미국에서도 `detox` 는 FTC 가 주시하는 표현이다.

### 실제 수정 (4곳)

| 제품 | 전 | 후 |
|---|---|---|
| 차콜 듀오 세트 | deeply cleanses, **detoxifies**, and nourishes | deeply cleanses and nourishes |
| 리추얼 클렌징 듀오 | the perfect balance of **purification** | the perfect balance of **cleansing** |
| 리추얼 클렌징 듀오 | designed to **detoxify**, replenish, elevate | designed to **cleanse**, replenish, elevate |
| 미니 리추얼 세트 | it **deeply purifies** | it **cleanses thoroughly** |

문장 구조는 그대로 두고 동사만 교체했다. `nourish` · `replenish` · `soft` · `refreshed` 는 유지.

### `Hand-poured` → `Handcrafted` (2곳)

미르 프로텍션 바 본품 · 듀오 세트. **비누는 붓는 것이 아니다.**
캔들 문구가 복사되면서 넘어온 것으로 보인다.
캔들의 `Hand-poured in California` 는 정확한 표현이므로 그대로 둔다.
미니 리추얼 세트의 `hand-poured` 는 **틴 캔들**을 가리키므로 유지.

### 같이 넣은 확정 사실

| 항목 | 반영 |
|---|---|
| 중량 250 g | 바 솝 관련 6개 제품 전부 |
| 한 달 건조 | 바 솝 관련 제품 전부 |
| **스위트아몬드(견과류) 고지** | 미르 바 본품 · 듀오 · 리추얼 클렌징 듀오 |

🔴 **견과류 고지는 원래 영문 페이지에 아예 없었다.** 한국 페이지에는 있었다.
   알레르기 고지 누락은 실질적 위험이므로 이번에 추가했다.

### 제품명은 바꾸지 않는다 (`소영` 결정, 2026-09-15)

`Bamboo Forest Charcoal Detox Bar` 의 `Detox` 는 **제품명으로 유지**한다.
이름은 브랜드 식별자이며 문장형 효능 주장보다 약하다.
이름을 바꾸면 6종 체계 · 라벨 · 바코드 매핑 · KR 페이지가 연쇄로 걸린다.

### 🟡 남은 것

- 트래블 리추얼 틴 중량 `0.1 lb` (약 45 g) — 내용물 1.56 oz(44 g) 대비 포장 포함이면 낮아 보임
- E-gift card · 트래블 리추얼 틴 SEO 비어 있음 (실물 제품 아니거나 우선순위 낮음)

## 2026-09-15 — 트래블 리추얼 틴 중량 확정

| 항목 | 값 |
|---|---|
| 왁스(내용물) | 1.56 oz = 약 44 g |
| **등록 중량(완제품)** | **65 g** (`소영` 확정) |
| 이전 등록값 | 0.1 lb = 45.4 g — 왁스만 세고 틴·파우치를 누락 |

변형 4개 전부 반영. 단위도 POUNDS → GRAMS 로 바꿔 소수점 오차를 없앴다.

🟡 **이 제품은 곧 사이트에서 내릴 예정** (`소영`, 2026-09-15).
   내릴 때는 **ARCHIVED** 로 돌린다. 삭제하면 과거 주문 이력이 끊긴다.
   SKU·UPC 가 없는데, 내릴 제품이므로 새로 발급하지 않는다.

## 3.5 oz 미니 틴 4종 — 마스터 시트에서 삭제

`소영` 지시로 `data/SKU_UPC_List.xlsx` 에서 4줄 삭제했다.
발급된 UPC 는 `core-facts/바코드-UPC.md` 의 **단종 — 번호 재사용 금지** 항목에 옮겨 적었다.
번호가 이미 소진된 상태이므로 다른 제품에 재배정하면 안 된다.
