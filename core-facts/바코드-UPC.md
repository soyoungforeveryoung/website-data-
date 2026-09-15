# 바코드 · SKU · UPC 원본

- 출처: **SKU/UPC 마스터 시트** (`소영`, 2026-09-15 제공)
- 원본 파일: **`data/SKU_UPC_List.xlsx`** — 이 저장소에 보관됨
- Drive 바코드 이미지 폴더: [UPC](https://drive.google.com/drive/folders/1s2LBpZa3BFtkAIsutCeBdokOWrWTW88H)
- 원칙: **추측한 값은 넣지 않는다.**

## 표기 규칙 🔴

- **12자리 UPC-A 로 통일한다.** `850034664200` 형식.
- ~~`00850034664200`~~ 처럼 앞에 0 을 붙인 14자리 표기는 **쓰지 않는다.**
  Drive 의 구 이미지 파일명에는 14자리로 적혀 있으나 숫자는 같다.

---

# 1. 코어 6종 — 라벨 인쇄용

라벨을 새로 만들 때 아래 값을 그대로 쓴다.

| 제품 | SKU | **UPC** | 바코드 이미지 |
|---|---|---|---|
| Bamboo Forest Charcoal Bar Soap | `111BFBS10` | **`850034664200`** | [PNG](https://drive.google.com/file/d/1vCRt7gukEyDvGU_KW6oXW7k5ahVYbpyc/view) |
| Bamboo Forest Special Body set | `111BFBS10` | **`850034664262`** | `없음` |
| Bamboo Forest Scented Candle | `777BFCD10` | **`850034664026`** | `없음` |
| Bushman Candle Scented Candle | `777BCCD10` | **`850034664163`** | [PNG](https://drive.google.com/file/d/1r2PNrWqB4Gaq5zhhgMCD9X7ObIwHD-nq/view) |
| Shaman Scented Candle | `777SMCD10` | **`850034664170`** | [PNG](https://drive.google.com/file/d/1H51ZCRgVkU7dJU_HwsSEoP0jTVkAXYyQ/view) |
| Valley of Roses Scented Candle | `777TVRCD10` | **`850034664217`** | [PNG](https://drive.google.com/file/d/1LCxrrPdvxUAAjw1EGpbtO0x9TKO0jABA/view) |
| Bushman Candle Myrrh Protection Bar | `111BCBS10` | **`850034664378`** | 실물 바코드 확인 |

✅ **미르 프로텍션 바 해결됨 (2026-09-15).** 소영님이 실제 바코드 이미지를 확인해 주셨고
   `8 50034 66437 8` = `850034664378` 로 Shopify 등록값과 일치했다.
   마스터 시트에 행이 없던 것을 **`data/SKU_UPC_List.xlsx` 17행에 추가**했다
   (Bath & Wellness, 차콜 바 · 스페셜 바디세트 다음).

## 복사용

```
Bamboo Forest Scented Candle      777BFCD10    850034664026
Bushman Candle Scented Candle     777BCCD10    850034664163
Shaman Scented Candle             777SMCD10    850034664170
Valley of Roses Scented Candle    777TVRCD10   850034664217
Bamboo Forest Charcoal Bar Soap   111BFBS10    850034664200
Myrrh Protection Bar              111BCBS10    850034664378
```

---

# 2. 🔴 주의 — 라벨 만들기 전에 확인할 것

## (1) 차콜 바 구번호 폐기됨

| 번호 | 상태 |
|---|---|
| **`850034664200`** | ✅ **현행.** 이걸 쓴다 |
| ~~`00850034664101`~~ | ❌ 예전에 잘못 만든 번호 (`소영` 확인, 2026-09-15). Shopify 에서 제거함 |

## (2) `111BFBS10` SKU 가 중복 사용되고 있다

| SKU | 제품 | UPC |
|---|---|---|
| `111BFBS10` | Bamboo Forest Charcoal Bar Soap | `850034664200` |
| `111BFBS10` | Bamboo Forest Special Body set | `850034664262` |

UPC 는 다르므로 **유통에는 문제가 없다.** 다만 SKU 로 재고를 관리하면 섞인다.
→ 세트 쪽 SKU 를 분리하는 것을 권함 (예: `111BFSBS10`).
   실제로 Drive 의 세트 바코드 파일명은 `111bfsbs10` 으로 되어 있어,
   **어딘가에서는 이미 분리해서 쓰고 있었던 것으로 보인다.**

## (3) `111BFBS10` 셀에 탭 문자가 들어 있다

마스터 시트 16행 `Bamboo Forest Special Body set` 의 SKU 값이 `\t111BFBS10` 으로
**앞에 탭 문자**가 붙어 있다. 눈으로는 안 보이지만 시스템 간 대조 시 불일치가 난다.
→ 시트에서 해당 셀을 다시 입력할 것.

## (4) Special Body set 번호가 두 곳에서 다르다

| 출처 | 번호 |
|---|---|
| 마스터 시트 | `850034664262` |
| Drive 이미지 파일명 | `00850034664224` |

🔴 **서로 다르다.** 코어 6종은 아니지만 세트 라벨을 만들 때 확인이 필요하다. → `확인 필요`

---

# 🔴 단종 — 번호 재사용 금지

아래 제품은 마스터 시트에서 **삭제**했다 (`소영`, 2026-09-15).
단 **UPC 번호는 이미 발급·사용된 것이므로 다른 제품에 재배정하면 안 된다.**
시트에서 지워도 번호는 소진된 상태로 남으므로 여기에 기록해 둔다.

## 3.5 oz 미니 틴 캔들 4종 (시트에서 삭제 완료)

| SKU | 제품 | UPC |
|---|---|---|
| `777BFTCD20` | Bamboo Forest Mini Tin Candle - 3.5oz + 1 Palo Santo Stick | `850034664156` |
| `777BCTCD20` | Bushman Mini Tin Candle - 3.5oz + 1 Palo Santo Stick | `850034664194` |
| `777SMTCD20` | Shaman Mini Tin Candle - 3.5oz + 1 Palo Santo Stick | `850034664187` |
| `777VRTCD20` | Valley of Roses - 3.5oz + 1 Palo Santo Stick | `850034664293` |

Drive 의 바코드 이미지 파일도 이 4종 것이 남아 있으니 **라벨 재인쇄 시 쓰지 말 것.**

## Travel Ritual Tin 1.5 oz — 🟡 사이트에서 삭제 예정

`소영` (2026-09-15): **곧 leverden.co 에서 내릴 예정.**

| 항목 | 값 |
|---|---|
| 현재 상태 | ACTIVE (변형 4개) |
| 중량 | **65 g** (2026-09-15 확정) |
| SKU | **없음** |
| UPC | **없음** |

→ 내릴 제품이므로 SKU·UPC 를 새로 발급하지 않는다.
→ 중량 65 g 은 내리기 전까지 나갈 주문의 배송비 계산을 위해 넣어 둔 값이다.
⚠️ 내릴 때 **ARCHIVED 로 돌리고 삭제하지 말 것.** 과거 주문 이력이 끊긴다.

---

# 3. 전체 목록 (마스터 시트 그대로)

| 분류 | SKU | 제품 | UPC |
|---|---|---|---|
| Bath & Wellness Products | `111BFLO10` | Bamboo Forest Hand & Body Lotion | `850034664002` |
| Bath & Wellness Products | `111BFMNLO10` | Bamboo Forest Mini Hand & Body Lotion | — |
| Bath & Wellness Products | `111BFBW10` | Bamboo Forest Hand & Body Wash | `850034664019` |
| Bath & Wellness Products | `111BFMNWA10` | Bamboo Forest Mini Hand & Body Wash | — |
| Bath & Wellness Products | `111WHSS10` | Wellness Home Spa Set | `850034664231` |
| Bath & Wellness Products | `333BFBS10` | BAMBOO FOREST - Amethyst Ki BathSoak - 1Kg | `850034664033` |
| Bath & Wellness Products | `333BFBS100G` | BathSoak - Amethyst Ki Mini Bamboo Salt | `850034664149` |
| Bath & Wellness Products | `111BFBS10` | Bamboo Forest Charcoal Bar Soap | `850034664200` |
| Bath & Wellness Products | `111BFBS10` | Bamboo Forest Special Body set | `850034664262` |
| Candles | `777BFCD10` | Bamboo Forest Scented Candle | `850034664026` |
| Candles |  | Old Bamboo Forest Scented Candle | — |
| Candles | `777BCCD10` | Bushman Candle Scented Candle | `850034664163` |
| Candles | `777SMCD10` | Shaman Scented Candle | `850034664170` |
| Candles | `777TVRCD10` | Valley of Roses Scented Candle | `850034664217` |
| Mini Tin Candles | `777BFTCD20` | Bamboo Forest Mini Tin Candle - 3.5oz + 1 Palo Santo Stick | `850034664156` |
| Mini Tin Candles | `777BCTCD20` | Bushman Mini Tin Candle - 3.5oz + 1 Palo Santo Stick | `850034664194` |
| Mini Tin Candles | `777SMTCD20` | Shaman Mini Tin Candle - 3.5oz + 1 Palo Santo Stick | `850034664187` |
| Mini Tin Candles | `777VRTCD20` | Valley of Roses - 3.5oz + 1 Palo Santo Stick | `850034664293` |
| Mini Tin Candles | `777KCTCD20` | Kama Collection - Travel Ritual Tin Set | `850034664354` |
| Mini Tin Candles | `777JTTCD20` | Joshua Tree - Travel Ritual Tin Set | `850034664361` |
| Mini Tin Candles |  | No Name - Burn Instruction Candles | — |
| Home Fragrance Diffuser | `888BFDF10` | Bamboo Forest Home Fragrance Diffuser | `850034664279` |
| Home Fragrance Diffuser | `888BCDF10` | Bushman candle Home Fragrance Diffuser | `850034664248` |
| Home Fragrance Diffuser | `888SMDF10` | Shaman Home Fragrance Diffuser | `850034664255` |
| Home Fragrance Diffuser | `888VRDF10` | Valley of Roses Home Fragrance Diffuser | `850034664286` |
| Home Fragrance Diffuser | `999DL10` | Metal Diffuser lid | `850034664309` |
| Home Fragrance Diffuser |  | Diffuser Gift Box | — |
| Home Fragrance Diffuser |  | Reed Sticks | — |
| Diffuser Refill Oil 162ml | `DR-BF01` | Bamboo Forest Diffuser Refill Oil Bottle | `850034664316` |
| Diffuser Refill Oil 162ml | `DR-BC01` | Bushman Candle Diffuser Refill Oil Bottle | `850034664323` |
| Diffuser Refill Oil 162ml | `DR-SM01` | Shaman Diffuser Refill Oil Bottle | `850034664330` |
| Diffuser Refill Oil 162ml | `DR-VR01` | Valley of Roses Diffuser Refill  Oil Bottle | `850034664347` |
| Diffuser Refill Oil 162ml | `999DL10` | Diffuser Lid | `850034664309` |
| Diffuser Refill Oil 162ml | `222BFBS10` | Luxury Gift bag | `850034664071` |
| Diffuser Refill Oil 162ml | `333BFCA10` | Bathsoak Canvas Bag | — |
| Diffuser Refill Oil 162ml |  | Brand Book | — |
| Package Box |  | Bushman Package Box | — |
| Package Box |  | Shaman Package Box | — |
| Package Box |  | Valley of Roses Package Box | — |
| Package Box | `111INI10` | Leverden Newsletters | — |
| Shipping Box | `222BSSS10` | Small Shipping Box | — |
| Shipping Box | `222BSMS10` | Medium Shipping Box | — |
| Shipping Box | `222BSLR10` | Large Shipping Box | — |
| Shipping Box | `222BSLB10` | Large Empty Box | — |
| Shipping Box | `222BFSP10` | Old leVerden logo seed packets | — |
| Lid |  | White Empty Lid Box | — |
| Lid |  | Black Wooden Lid | — |
| Lid |  | Pink Wooden Lid | — |
| Lid |  | Orange Wooden Lid | — |
| Lid |  | Blue Wooden Lid | — |
| Vessel |  | Pink Vessel | — |
| Vessel |  | Orange Vessel | — |
| Vessel |  | Navy Vessel w/black plate | — |
| Vessel | `222BFCB10` | Bamboo candle box labels (Bamboo print, candle box waring in labels) | — |
| Vessel |  | White Tissue Paper | — |
| Vessel | `111ABLS10` | Amethyst ki bathsoak label stickers | — |
| Vessel | `111BSWR10` | White round stickers (candle vessel wrapping) | — |
| Vessel | `111BRST10` | Black Round Sticker | — |
| Vessel | `111CWPC10` | Candle Wax Protection Card | — |

📌 UPC 가 `—` 인 항목은 마스터 시트에 번호가 비어 있는 것이다. 미발급인지
   단순 누락인지는 확인하지 않았다. → `확인 필요`
