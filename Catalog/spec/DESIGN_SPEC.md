# THIÊN QUANG SMARTTOOLS — Design Spec v2

Mobile-only catalog app · 390×844px (iPhone safe area) · Internal B2B tool

4 screens: Home · Product List · Product List (Filter Open) · Quote List

## 1. Color Palette

| Token | Hex | Usage |
| --- | --- | --- |
| brand-green | `#145C4E` | Primary, CTA, active nav, icons, radio selected |
| brand-green-dark | `#103D34` | Page title headings |
| brand-green-mid | `#165A4D` | Back arrow, secondary links |
| brand-red | `#D94232` | SMARTTOOLS tagline |
| price-red | `#E64A33` | Price text (S02) |
| price-red-s3 | `#E31B23` | Price text (S03), CTA delete |
| cta-zalo | `#E31B23` | "Gửi báo giá qua Zalo" button |
| accent-yellow | `#FFCB2F` | Banner "sản phẩm" highlight |
| zalo-blue | `#0068FF` | Zalo nav item + badge |
| bg-screen | `#FCFCFA` | Screen background |
| bg-card | `#FFFFFF` | Card / sheet background |
| bg-image-zone | `#F4F6F2` | Product image outer zone (tinted sage) |
| bg-category-icon | `#F5F7F3` | Category icon outer zone |
| border-card | `#ECEFE8` | Card border (1px) |
| border-light | `#E7ECE8` | Quote row border |
| border-divider | `#ECEFE8` | Dividers inside sheet / cards |
| text-primary | `#171D19 / #1E2520 / #202220` | Main headings |
| text-secondary | `#67716A / #6E756F` | Sub-labels, counts |
| text-muted | `#909991` | Inactive nav, section labels |
| text-dark | `#2A322C` | Qty stepper numbers |
| nav-active | `#145C4E` | Active nav label + icon |
| nav-inactive | `#909991` | Inactive nav |
| badge-red | `#EF2D2D` | Nav badge dot |
| btn-added-bg | `#F3FBF6` | "✓ Thêm" added state background |
| phone-btn-bg | `#FFF1F1` | Header phone button background |
| divider-qty | `#E6EAE3` | Qty stepper divider lines |
| radio-off | `#D0D5D1` | Unselected radio border |
| overlay | `rgba(20,31,25,0.45)` | Filter backdrop overlay |

## 2. Typography

| Style | Size | Weight | Color | Usage |
| --- | --- | --- | --- | --- |
| Brand name | 18px | 700 | `#145C4E` | THIÊN QUANG header |
| Brand tag | 12px | 700 | `#D94232` | SMARTTOOLS |
| Status bar | 16px | 600 | `#121212` | 9:41 time |
| Page title | 20px | 700 | `#103D34` | Screen 02/03 header title |
| Page subtitle | 16px | 400 | `#647068` | "42 sản phẩm" count |
| Section title | 20px | 600 | `#171D19` | "Danh mục sản phẩm" etc. |
| "Xem tất cả" link | 14px | 600 | `#5B655E` | Section action link |
| Product name (S02) | 17px | 600 | `#1F2621` | Grid card name |
| Product name (S03) | 15px | 600 | `#202220` | List row name |
| Product group name | 18px | 600 | `#1E2520` | Home group card name |
| Product code (S02) | 14px | 400 | `#69736C` | "Mã SP: BXD-X01" |
| Product code (S03) | 11px | 400 | `#6E756F` | "Mã SP: BXD-X01" |
| Price (S02) | 16px | 700 | `#E64A33` | Product price |
| Price (S03) | 15px | 700 | `#E31B23` | Quote row price |
| Total price | 18px | 700 | `#E31B23` | Grand total |
| Subtotal label | 12px | 400 | `#6E756F` | "Tạm tính (tham khảo)" |
| "Thành tiền" label | 10px | 400 | `#6E756F` | Per-row total label |
| Per-row total | 16px | 700 | `#E31B23` | Per-row total value |
| Category name | 14px | 500 | `#242A25` | Category card label |
| Category count | 14px | 700 | `#2C332E` | "300+" count |
| Nav label | 12px | 500 | varies | Bottom nav text |
| Banner hero number | 28px | 700 | `#FFFFFF` | "2.000+" |
| Banner hero text | 28px | 700 | `#FFCB2F` | "sản phẩm" |
| Banner bullet | 15px | 500 | `#FFFFFF` | Bullet points |
| Add btn text | 13px | 700/600 | `#145C4E` | "+ Thêm" / "✓ Thêm" |
| Qty number | 14px | 700 | `#2A322C` | Stepper quantity |
| Qty +/- | 15px | 600 | `#2A322C` | Stepper +/- |
| CTA button | 14px | 700 | `#FFFFFF` | Zalo / Apply buttons |
| "×" delete | 19px | 500 | `#202220` | Row delete |
| Back arrow "←" | 26px | 500 | `#165A4D` | Back navigation |
| Filter sheet title | 18px | 700 | `#103D34` | "Bộ lọc sản phẩm" |
| Filter close "✕" | 18px | 500 | `#909991` | Sheet close button |
| Filter section label | 12px | 600 | `#909991` | "Loại bay" section |
| Filter option default | 15px | 400 | `#202220` | Unselected option |
| Filter option selected | 15px | 600 | `#145C4E` | Selected option |
| Filter reset btn | 15px | 600 | `#145C4E` | "Đặt lại" button |
| Filter apply btn | 15px | 700 | `#FFFFFF` | "Áp dụng" button |

## 3. Screen Layout

### Screen 01 — Home

`390×844px · bg #FCFCFA · radius 34 · border 1px #E8EBE4`

- Status bar (`9:41`): `y=16`
- Header (`y=56–97`)
  - Logo circle `40×40`, `x=20`
  - `THIÊN QUANG` centered `x=132`, `y=58`, `18px/700 #145C4E`
  - `SMARTTOOLS` centered `x=153`, `y=82`, `12px/700 #D94232`
  - Phone button `42×42` circle `x=328`, bg `#FFF1F1`, border `#F4BDBD`
- Banner `350×184`, `x=20`, `y=110`, radius `20`, image fill

### Screen 02 — Product List (Default)

`390×844px · scrollable`

- Header
  - `←` Back `x=20`, `26px/500 #165A4D`
  - Title `x=58`, `y=60`, `20px/700 #103D34`
  - Subtitle `x=58`, `y=92`, `16px/400 #647068`
  - Filter button `42×42` circle `x=327`, `y=56`
    - bg white, border `1px #E2E8E0`, radius `21`
    - 3-line SVG `18×14`, stroke `#145C4E` 2px round

### Screen 02B — Product List (Filter Open)

Base = Screen 02 +

- Overlay: `390×844 rgba(20,31,25,0.45)` full screen
- Filter Bottom Sheet: `390×590`, `y=254`
  - bg white
  - `topLeftRadius=24`
  - `topRightRadius=24`
  - Handle `36×4` radius `2`, `x=177`, `y=12`, color `#ECEFE8`
  - Title `Bộ lọc sản phẩm`: `x=20`, `y=30`, `18px/700 #103D34`
  - Close `✕`: `x=352`, `y=30`, `18px/500 #909991`

### Screen 03 — Quote List

`390×844px · scrollable`

- Header: `←` Back · `Danh sách báo giá` `20px/700` · `4 sản phẩm` `16px/400`
- Rows start `y=118`, each `350×116`, radius `16`, border `#E7ECE8`
  - Image `96×96`, `x=12`, `y=10`, radius `9`, bg `#F4F6F2`
  - Name `x=122`, `y=12`, `15px/600 #202220`
  - Code `x=122`, `y=38`, `11px/400 #6E756F`
  - Price `x=122`, `y=58`, `15px/700 #E31B23`
  - Stepper `x=122`, `y=80`, `82×25`, radius `8`, border `#E6EAE3`

## 4. Component Specs

### Product Card (S02)

- Size: `169×242`, radius `14`
- Image: `129×129`, `x=20`, `y=12`, radius `9`, bg `#F4F6F2`
- Name: `x=14`, `y=144`, `17px/600`, `#1F2621`
- Code: `x=14`, `y=170`, `14px/400`, `#69736C`
- Price: `x=14`, `y=202`, `16px/700`, `#E64A33`
- Button: `x=86`, `y=193`, `72×30`, radius `7`, border `1.4px #145C4E`
  - Default: bg white · `+ Thêm` `13px/700+600 #145C4E`
  - Added: bg `#F3FBF6` · `✓ Thêm` `13px/700+600 #145C4E`
  - Padding `L=11 R=11 T=7 B=7`, gap `5`

### Quote Row (S03)

- Size: `350×116`, radius `16`
- Image: `96×96`, `x=12`, `y=10`, radius `9`, bg `#F4F6F2`
- Name: `x=122`, `y=12`, `15px/600`, `#202220`
- Code: `x=122`, `y=38`, `11px/400`, `#6E756F`
- Price: `x=122`, `y=58`, `15px/700`, `#E31B23`
- Qty: `x=122`, `y=80`, `82×25`, radius `8`
- Total: `x=258`, `y=58`, `16px/700`, `#E31B23`
- Delete: `x=322`, `y=7`, `19px/500`, `#202220`

### Qty Stepper

- Size: `82×25`, radius `8`, border `#E6EAE3`
- `[−] 15px/600 | divider 1×17 | N 14px/700 | divider 1×17 | [+] 15px/600`
- Padding `L=6 R=6`
- Gap `8`
- Text color `#2A322C`
- Divider `#E6EAE3`

### Filter Bottom Sheet

- Size: `390×590`
- Top left radius `24`
- Top right radius `24`
- Bg white
- 9 radio options
- Single-select
- `Tất cả` selected by default
- Buttons: `Đặt lại` + `Áp dụng`

### Bottom Nav

- Size: `390×82`
- Active `#145C4E`
- Inactive `#909991`
- Zalo always `#0068FF`
- Badge `18×18 #EF2D2D`, text `10px/700` white

## 5. Interactions & Filter Rules

### Filter Interaction Rules

```text
MODEL: Single-select radio (1 active at a time)
DEFAULT: "Tất cả" selected

Tap option   → deselect previous · select tapped
Tap "Đặt lại" → reset all · auto-select "Tất cả" · grid NOT yet filtered
Tap "Áp dụng" → close sheet (slide down) · fade overlay · filter grid
Tap "✕" / backdrop → close without applying · restore prev state
```

### All Interactions

| Action | Trigger | Result |
| --- | --- | --- |
| Add product | `+ Thêm` | `✓ Thêm`, bg `#F3FBF6`, badge +1 |
| Remove from cart | `✓ Thêm` | `+ Thêm`, bg white, badge -1 |
| Open filter | Filter icon | Sheet slides up, overlay appears |
| Close filter | `✕` or backdrop | Sheet slides down, no change |
| Reset filter | `Đặt lại` | All clear, `Tất cả` selected |
| Apply filter | `Áp dụng` | Close sheet, filter grid |
| Increase qty | `+` | qty+1, row total, grand total update |
| Decrease qty | `−` | qty-1 (min=1), totals update |
| Remove row | `×` | Row removed, badge -1, totals update |
| Send quote | Zalo CTA | Open Zalo with pre-filled message |

## 6. Data Models

```json
{
  "id": "BXD-X01",
  "name": "Bay inox 20cm",
  "code": "BXD-X01",
  "price": 89000,
  "category": "bay-xay-dung",
  "subtype": "can-go",
  "image": "url_to_1x1_white_bg_jpg"
}
```

## 7. Sample Data

### Quote List (S03)

| Code | Name | Price | Qty | Total |
| --- | --- | --- | --- | --- |
| BXD-X01 | Bay inox 20cm | 89.000đ | 2 | 178.000đ |
| BXD-T01 | Bay thép 20cm | 79.000đ | 3 | 237.000đ |
| KCB-01 | Ke cân bằng | 45.000đ | 5 | 225.000đ |
| BKH-60 | Bàn kéo hồ 60cm | 199.000đ | 1 | 199.000đ |
| TOTAL |  |  | 4 | 839.000đ |

## 8. Assets Required

| Asset | Format | Size |
| --- | --- | --- |
| Logo | PNG transparent | 80×80px |
| Banner | JPG | 700×368px @2x |
| Category icons (4) | PNG white bg | 104×104px @2x |
| Product photos | JPG white bg | 258×258px @2x · 1:1 mandatory |
| Filter icon | SVG | 3 decreasing lines · stroke `#145C4E` 2px round |

## 9. Figma Reference

- File: `https://figma.com/design/yh4mZrtJwlXKQ7mBgSf4U6`
- S01 Home: node `17:11`
- S02 Product List: node `17:12`
- S03 Quote List: node `17:13`
- S02B Filter Open: clone of S02 + overlay + bottom sheet
