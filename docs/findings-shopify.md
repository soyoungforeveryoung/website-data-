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
| 바 솝 중량 | Charcoal 0.6 lb vs Myrrh 0.2 lb (3배 차이) | **Myrrh Bar가 오류.** 순중량 250g 확정 → Charcoal 0.6 lb만 타당 |

## 🟡 오타

| 위치 | 현재 | 정정 |
|---|---|---|
| 캔들 4종 `advantages_heading_3` | Consicientious | Conscientious |
| Valley of Roses SEO | Morocccan | Moroccan |
| Charcoal Bar 성분 | bermot | bergamot |
| Myrrh Bar 성분 | Prunus armgd­alus (보이지 않는 soft hyphen 포함) | Prunus amygdalus |
| 조향사 소개 본문 | Laudimiel | Laudamiel |

## 🟡 사양 변경 미반영

- 캔들 용량이 **250g**으로 변경되었으나 사이트에 반영 안 됨.
- 기존 표기 `Burning time: 60 hours`는 이전 용량 기준 → **재산정 필요**.
- 기존 표기 `Dimensions: 11 5/8 * 4 inches`는 약 29cm로 비현실적 → 실측 필요.

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
