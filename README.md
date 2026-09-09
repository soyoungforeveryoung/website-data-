# 웹사이트 모든 데이터 통합 수정

leverden 브랜드의 국가별 웹사이트에 흩어진 제품 데이터를 **하나의 원장(Single Source of Truth)** 으로 통합하는 저장소.

## 배경

| 채널 | 플랫폼 | 도메인 | 지역 |
|---|---|---|---|
| 글로벌 | Shopify | leverden.co | US · EU |
| 한국 | Cafe24 | leverden.co.kr | KR |

같은 브랜드·같은 제품인데 **국가별로 불변 정보(성분, 용량, 향 노트, 원산지 등)가 다르게 저장**되어 있음.
2027년 리브랜딩을 앞두고, 먼저 코어팩트를 확정하고 두 사이트를 여기에 맞춰 정렬한다.

## 범위 (Phase 1)

2026년 말까지 한국·미국·유럽에서 판매하는 **6종**만 다룬다.

**캔들 4종**
- Bamboo Forest Scented Candle
- Bushman Candle Scented Candle
- Shaman Scented Candle
- Valley of Roses Scented Candle

**바 솝 2종**
- Bamboo Forest Charcoal Detox Bar
- Bushman Candle Myrrh Protection Bar

## 작업 순서

1. **코어팩트 원장 작성** ← 진행 중 (`core-facts/core-facts.yaml`)
2. 솔드아웃·단종 제품 shop list에서 정리 (`docs/soldout-cleanup.md`)
3. 두 사이트를 원장 기준으로 정렬
4. 상세페이지 및 마케팅 자료 제작

## 디렉터리

```
brand/          브랜드 표기 규칙 (최상위 원칙)
core-facts/     제품 코어팩트 원장 — 이 저장소의 핵심
docs/           불일치 조사 결과, 정리 계획
data/           각 채널에서 뽑은 원본 데이터 (수정 금지)
```
