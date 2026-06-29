# THIÊN QUANG SMARTTOOLS — Design Spec

Mobile-only catalog app · 390×844px (iPhone safe area) · Internal B2B tool

## 1. Color Palette

| Token | Hex | Usage |
| --- | --- | --- |
| brand-green | `#145C4E` | Primary, CTA, active nav, icons |
| brand-green-dark | `#103D34` | Page title headings |
| brand-green-mid | `#165A4D` | Back arrow, secondary links |
| brand-red | `#D94232` | SMARTTOOLS tagline |
| price-red | `#E64A33` | Price text (S02) |
| price-red-s3 | `#E31B23` | Price text (S03), delete button |
| cta-zalo | `#E31B23` | "Gửi báo giá qua Zalo" button |
| accent-yellow | `#FFCB2F` | Banner "sản phẩm" highlight |
| zalo-blue | `#0068FF` | Zalo nav item + badge |
| bg-screen | `#FCFCFA` | Screen background |
| bg-card | `#FFFFFF` | Card background |
| bg-image-zone | `#F4F6F2` | Product image outer zone (tinted sage) |
| bg-category-icon | `#F5F7F3` | Category icon outer zone |
| border-card | `#ECEFE8` | Card border (1px) |
| border-light | `#E7ECE8` | Quote row border |
| text-primary | `#171D19 / #1E2520 / #202220` | Main headings |
| text-secondary | `#67716A / #6E756F` | Sub-labels, counts |
| text-muted | `#909991` | Inactive nav items |
| text-dark | `#2A322C` | Qty stepper numbers |
| nav-active | `#145C4E` | Active nav label + icon |
| nav-inactive | `#909991` | Inactive nav |
| badge-red | `#EF2D2D` | Nav badge dot |
| btn-added-bg | `#F3FBF6` | "✓ Thêm" added state bg |
| phone-btn-bg | `#FFF1F1` | Header phone button bg |
| divider-qty | `#E6EAE3` | Qty stepper divider lines |

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
| Product code | 14px | 400 | `#69736C` | "Mã SP: BXD-X01" (S02) |
| Product code (S03) | 11px | 400 | `#6E756F` | "Mã SP: BXD-X01" (S03) |
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
| "+ Thêm" btn | 13px | 700/600 | `#145C4E` | Add button text |
| Qty number | 14px | 700 | `#2A322C` | Stepper quantity |
| Qty +/- | 15px | 600 | `#2A322C` | Stepper buttons |
| CTA button | 14px | 700 | `#FFFFFF` | Zalo send button |
| "×" delete | 19px | 500 | `#202220` | Row delete |
| Back arrow "←" | 26px | 500 | `#165A4D` | Back navigation |

## 3. Screen Layout

### Screen 01 — Home (Trang chủ)

`390×844px · bg #FCFCFA · border-radius 34 · border #E8EBE4 1px`

- Status bar (9:41 / signal): `y=16`
- Header (`y=56`)
  - Logo circle `40×40` at `x=20`
  - `THIÊN QUANG` centered on 390px, `x=132`, `y=58`
  - `SMARTTOOLS` centered, `x=153`, `y=82`
  - Phone button `42×42` circle, bg `#FFF1F1`, border `#F4BDBD`, `x=328`
- Banner `350×184`, radius `20`, `y=110`, `x=20`, image fill

### Screen 02 — Product List

`390×844px · scrollable content`

- Header (`y=56–92`)
  - `←` Back at `x=20`, 26px, `#165A4D`
  - Page title `20px/700`, `#103D34`
  - Subtitle `16px/400`, `#647068`
  - Filter icon `42×42` circle, `x=327`, 3-line SVG, `#145C4E`, stroke 2px
- Product grid
  - 2 columns, gap `8px`
  - Card `169×242`, radius `14`, white bg, border `#ECEFE8`

### Screen 03 — Quote List

`390×844px · scrollable content`

- Header: `←` Back, `Danh sách báo giá` `20px/700`, `4 sản phẩm` `16px/400`
- Product rows start at `y=118`
  - Row `350×116`, radius `16`, white bg, border `#E7ECE8`
  - Image zone `96×96`, `x=12`, `y=10`, radius `9`, bg `#F4F6F2`, image fill
  - Name `x=122`, `y=12`, `15px/600`, `#202220`
  - Code `x=122`, `y=38`, `11px/400`, `#6E756F`
  - Price `x=122`, `y=58`, `15px/700`, `#E31B23`

## 4. Component Specs

### Product Card — Grid (S02)

- Size: `169×242`, radius `14`
- Image zone: `129×129`, `x=20`, `y=12`, radius `9`, bg `#F4F6F2`
- Name: `x=14`, `y=144`, `17px 600`, `#1F2621`
- Code: `x=14`, `y=170`, `14px 400`, `#69736C`
- Price: `x=14`, `y=202`, `16px 700`, `#E64A33`
- Add button: `x=86`, `y=193`, `72×30`, radius `7`, border `1.4px #145C4E`

### Quote Row — List (S03)

- Size: `350×116`, radius `16`
- Image zone: `96×96`, `x=12`, `y=10`, radius `9`, bg `#F4F6F2`
- Name: `x=122`, `y=12`, `15px 600`, `#202220`
- Code: `x=122`, `y=38`, `11px 400`, `#6E756F`
- Price: `x=122`, `y=58`, `15px 700`, `#E31B23`
- Stepper: `x=122`, `y=80`, `82×25`, radius `8`, border `#E6EAE3`
- Row total: `x=258`, `y=58`, `16px 700`, `#E31B23`
- Delete: `x=322`, `y=7`, `19px 500`, `#202220`

### Qty Stepper

- Size: `82×25`, radius `8`, border `#E6EAE3`
- Layout: horizontal, padding `L=6 R=6`, gap `8`
- Structure: `[−] | divider | N | divider | [+]`
- Number: `14px/700`
- Plus/minus: `15px/600`
- Text color: `#2A322C`
- Divider color: `#E6EAE3`

### Add Button

- Height: `30`
- Radius: `7`
- Border: `1.4px #145C4E`
- Padding: `L=11 R=11 T=7 B=7`
- Gap: `5`
- Default: bg `#FFFFFF`, `+` and `Thêm` in `#145C4E`
- Added: bg `#F3FBF6`, `✓` and `Thêm` in `#145C4E`

### Category Card (S01)

- Inner card: `72–94px` wide, `122px` tall, radius `12`, white bg
- Active border: `1.6px #145C4E`
- Inactive border: `1px #ECEFE8`
- Icon zone: `52×52`, radius `10`, bg `#F5F7F3`, image fill
- Name at `y=74`: `14px/500 #242A25`
- Count at `y=97`: `14px/700 #2C332E`
- Active bar: `36×4`, radius `2`, bg `#145C4E`

### Bottom Nav

- Size: `390×82`
- Bg: white
- Top border: `1px #ECEFE8`
- Active: `#145C4E`
- Inactive: `#909991`
- Zalo: `#0068FF`
- Badge: `18×18`, red `#EF2D2D`, text `3` in `10px/700` white
- Nav label: `12px/500`

## 5. Features & Interactions

| Action | Trigger | Result |
| --- | --- | --- |
| Add product | Tap `+ Thêm` | Button becomes `✓ Thêm`, bg `#F3FBF6`, badge +1 |
| Increase qty | Tap `+` in stepper | Qty +1, row total updates |
| Decrease qty | Tap `−` in stepper | Qty -1, min 1 |
| Remove item | Tap `×` | Row removed, badge -1, total updates |
| Send quote | Tap Zalo button | Opens Zalo with pre-filled quote message |
| Back to shop | Tap `Tiếp tục` | Navigate to product list |
| Filter | Tap filter icon | Open filter/sort panel |
| Category | Tap category card | Navigate to product list for that category |

## 6. Data Models

```json
{
  "id": "BXD-X01",
  "name": "Bay inox 20cm",
  "code": "BXD-X01",
  "price": 89000,
  "category": "bay-xay-dung",
  "image": "url_to_1x1_white_bg_jpg"
}
```

## 7. Sample Data

Categories:

- Xây tô (`300+`)
- Ốp lát (`250+`)
- Sơn nước (`180+`)
- Thạch cao (`150+`)

Products — Bay xây dựng:

| Code | Name | Price |
| --- | --- | --- |
| BXD-X01 | Bay inox 20cm | 89.000đ |
| BXD-X02 | Bay inox 22cm | 99.000đ |
| BXD-X03 | Bay inox 20cm | 89.000đ |
| BXD-X04 | Bay inox 22cm | 99.000đ |
| BXD-X05 | Bay inox 20cm | 89.000đ |
| BXD-X06 | Bay inox 22cm | 99.000đ |

Quote List (Screen 03):

| Code | Name | Price | Qty | Total |
| --- | --- | --- | --- | --- |
| BXD-X01 | Bay inox 20cm | 89.000đ | 2 | 178.000đ |
| BXD-T01 | Bay thép 20cm | 79.000đ | 3 | 237.000đ |
| KCB-01 | Ke cân bằng | 45.000đ | 5 | 225.000đ |
| BKH-60 | Bàn kéo hồ 60cm | 199.000đ | 1 | 199.000đ |
| TOTAL |  |  | 4 items | 839.000đ |

## 8. Assets Required

| Asset | Format | Size |
| --- | --- | --- |
| Logo Thiên Quang | PNG transparent | 80×80px |
| Banner homepage | JPG | 700×368px @2x |
| Category icons (4) | PNG white bg | 104×104px @2x |
| Product photos | JPG white bg | 258×258px @2x, 1:1 |
| Filter icon | SVG | 3 lines, stroke `#145C4E` 2px rounded |

## 9. Figma Reference

- File: `https://figma.com/design/yh4mZrtJwlXKQ7mBgSf4U6`
- Screen 01 — Home: node `17:11`
- Screen 02 — Product List: node `17:12`
- Screen 03 — Quote List: node `17:13`
