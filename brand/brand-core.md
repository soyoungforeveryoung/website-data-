# 브랜드 코어 규칙

이 문서의 규칙은 **모든 채널·모든 언어·모든 자료에 예외 없이 적용**된다.
상충하는 기존 표기는 전부 이 규칙에 맞춰 수정한다.

## 1. 브랜드명 표기

**`leverden`** — 전부 소문자, 한 단어, 띄어쓰기 없음.

| 상태 | 표기 |
|---|---|
| ✅ 정 | `leverden` |
| ❌ 오 | `leVerden` · `LeVerden` · `Leverden` · `LEVERDEN` · `le Verden` |

- **사유**: 상표권(trademark) 이슈로 `leVerden` → `leverden` 변경됨. 대문자 `V` 표기는 더 이상 사용하지 않는다.
- **적용 범위**: 제품명, 벤더명, SEO 타이틀/설명, 본문 카피, 이메일, 인쇄물, 소셜, 패키지, 도메인 표기 등 전부.
- **예외**: 문장 첫 글자여도 대문자로 올리지 않는다. 로고 아트워크 등 이미 인쇄·제작된 자산은 별도 교체 계획으로 관리한다.

### 점검 방법
```
grep -rniE 'le[[:space:]]*[Vv]erden' . | grep -v 'leverden'
```

## 2. 제품명 표기

- 영문 제품명은 Title Case, 콜렉션명 + 제품 타입 순서.
  예) `Bamboo Forest Scented Candle`, `Bushman Candle Myrrh Protection Bar`
- 연속 공백 금지 (현재 `Bushman candle  Scented Candle` 오류 있음).
- `Bushman Candle`은 **식물(원료) 이름**이다. 영문은 두 단어 모두 대문자,
  국문은 `부시맨 캔들`로 띄어 쓴다. 붙여 쓰지 않는다.
- 제품명은 **원료명 + 제품 종류** 구조를 지킨다.
  `부시맨 캔들 센티드 캔들` 처럼 '캔들'이 두 번 나와도 그대로 둔다.
  앞의 '캔들'은 식물 이름의 일부이고 뒤의 '캔들'은 제품 종류이므로 생략하면 뜻이 달라진다.
  영문도 동일: `Bushman Candle Scented Candle`

## 3. Product type 표기

| ✅ 정 | ❌ 오 |
|---|---|
| `Candle` | — |
| `Bar Soap` | `barsoap` · `Barsoap` · `BarSoap` |

`bar soap`은 영어에서 **두 단어**다. `barsoap`은 존재하지 않는 표기이므로 쓰지 않는다.
제품 타입·제품명 등 고유명사 위치에서는 `Bar Soap`, 문장 속 일반명사로 쓸 때는 `bar soap`.

### 3-1. Soap on a rope

로프가 달린 바 솝은 영어권 통용 명칭인 **`soap on a rope`** 로 통일한다.

| 위치 | 표기 | 예 |
|---|---|---|
| 문장 속 | `soap on a rope` | Our handmade soap on a rope lathers into a rich foam. |
| 명사 앞 수식어 | `soap-on-a-rope` (하이픈) | a luxury soap-on-a-rope ritual |

| ✅ 정 | ❌ 오 |
|---|---|
| `soap on a rope` | `hanging rope soap` · `rope bar soap` · `hanging bar soap` |

- 현재 Charcoal Bar 본문에만 `soap-on-a-rope`가 쓰여 있고, Myrrh Bar 등 나머지는
  `hanging linen-blend rope` 식으로 제각각이다. 전부 위 규칙으로 정렬한다.
- 로프 소재를 설명할 때는 `on a biodegradable linen-blend rope` 처럼 뒤에 덧붙인다.
  로프 소재가 명칭을 대체하지 않는다.

## 4. 제품 사양 표기

- 캔들 용량은 **250g** (순 왁스 중량)으로 통일한다. 배송중량과 혼동하지 않는다.
- 용량·중량은 g 단위를 우선 표기하고, 필요 시 oz를 괄호로 병기한다.
