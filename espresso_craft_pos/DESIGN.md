---
name: Espresso Craft POS
colors:
  surface: '#fcf9f3'
  surface-dim: '#dcdad4'
  surface-bright: '#fcf9f3'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3ed'
  surface-container: '#f0eee8'
  surface-container-high: '#ebe8e2'
  surface-container-highest: '#e5e2dc'
  on-surface: '#1c1c18'
  on-surface-variant: '#504440'
  inverse-surface: '#31312d'
  inverse-on-surface: '#f3f0ea'
  outline: '#827470'
  outline-variant: '#d3c3be'
  surface-tint: '#74584e'
  primary: '#090100'
  on-primary: '#ffffff'
  primary-container: '#2c1810'
  on-primary-container: '#9e7e73'
  inverse-primary: '#e3bfb2'
  secondary: '#84531a'
  on-secondary: '#ffffff'
  secondary-container: '#febc79'
  on-secondary-container: '#784910'
  tertiary: '#000301'
  on-tertiary: '#ffffff'
  tertiary-container: '#002215'
  on-tertiary-container: '#09976a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbce'
  primary-fixed-dim: '#e3bfb2'
  on-primary-fixed: '#2a170f'
  on-primary-fixed-variant: '#5a4137'
  secondary-fixed: '#ffdcbd'
  secondary-fixed-dim: '#fbb977'
  on-secondary-fixed: '#2c1600'
  on-secondary-fixed-variant: '#683c02'
  tertiary-fixed: '#85f8c4'
  tertiary-fixed-dim: '#68dba9'
  on-tertiary-fixed: '#002114'
  on-tertiary-fixed-variant: '#005137'
  background: '#fcf9f3'
  on-background: '#1c1c18'
  surface-variant: '#e5e2dc'
typography:
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 22px
    fontWeight: '700'
    lineHeight: 28px
  headline-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '700'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '600'
    lineHeight: 16px
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
  numeric-total:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '800'
    lineHeight: 32px
  numeric-card:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '700'
    lineHeight: 18px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-compact: 0.75rem
  margin: 1.25rem
  margin-mobile: 0.75rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.875rem
  space-lg: 1.25rem
  space-xl: 2rem
---

## Brand & Style

This design system is engineered for modern specialty coffee shops, roasteries, and beachside café concepts in Da Nang. It bridges artisanal coffee culture with high-velocity hospitality operations. The visual atmosphere balances the tactile richness of dark roasted specialty coffee with the crisp efficiency of contemporary touch-first enterprise software.

### Tone & Personality
- **Artisanal & Grounded:** Rooted in deep, rich espresso tones and warm caramelized undertones that mirror single-origin brews and roasted beans.
- **Ergonomic & Touch-First:** Designed specifically for counter tablets and point-of-sale displays. Buttons, modifiers, and numerical readouts prioritize tap accuracy and zero-latency operational speed during peak morning rushes.
- **Ultra-Legible & Functional:** Clean information architecture with aggressive visual hierarchy, allowing baristas and cashiers to process complex ticket queues and modifications effortlessly under ambient coastal daylight or dim café interior lighting.

### Visual Style
A tailored mix of **Minimalism** and **Tactile Modern Utility**:
- Sharp planar separation with subtle surface tinting rather than heavy drop shadows.
- Generous, tap-optimized hit targets (minimum 48px to 56px) with distinct physical feedback states (depressed active states, high-contrast borders).
- Segmented workstation ergonomics: Left navigation (Categories/Floors), Central grid (Item Cards with large imagery and pricing), and Right panel (Real-time Order Slip & VietQR/Cash Checkout).

## Colors

The palette is tuned specifically for coffeehouse point-of-sale operations, combining heavy contrast for quick recognition with natural, warm earth tones:

- **Primary (`#2C1810` - Deep Espresso):** Represents strong structure and authority. Used for primary interactive actions (Charge, Send to Kitchen), top-level active category selections, critical header bars, and primary dark text readouts.
- **Secondary (`#C78C4E` - Caramel Warmth):** Used for item modifiers (extra shot, oat milk, sugar levels), secondary triggers, discount badges, and highlighted selections within order items.
- **Tertiary (`#059669` - Fresh Mint Emerald):** Dedicated to operational success signals, active table availability, completed transactions, and the real-time "Online" status indicator. Paired with a soft mint background (`#ECFDF5`) for high legibility.
- **Neutral Canvas (`#F9F6F0` - Warm Milk Foam):** Replaces harsh stark whites with a comforting, low-glare cream foundation that reduces cashier eye strain during long shifts.

### Functional States & System Colors
- **VietQR Accent (`#005BAA`):** Dedicated national banking standard blue, reserved exclusively for the instant VietQR dynamic payment toggle.
- **Alert / Void / Busy Table (`#DC2626` / `#B91C1C`):** Used for voiding items, cancelling orders, offline status alerts, and occupied tables.
- **Surface Elevation Levels:**
  - Base Screen Canvas: `#F4EFEA`
  - Card & Module Surfaces: `#FFFFFF`
  - Subtle Border Strokes: `#E6DCD2`
  - Cart Panel Background: `#FFFFFF`
  - Active Selection Fill: `#F3E8DF`

## Typography

The type system blends the organic, friendly structure of **Plus Jakarta Sans** for product branding, drink titles, and menu categories with the ultra-precise tabular clarity of **Inter** for currency amounts, quantities, order numbers, and operational labels.

### Hierarchy Guidelines
- **Numeric Dominance (`numeric-total`, `numeric-card`):** Prices use tabular numbers (`tnum`) in Inter font to avoid horizontal shifting when item totals update. VND currency symbols (đ) are rendered consistently adjacent to the figure.
- **Product Titles:** Drink names (e.g., "Cà phê Muối Đà Nẵng", "Cold Brew Cam Vàng") use `headline-sm` with a tight line height to prevent two-line item cards from clipping prices.
- **Kitchen & Order Slip Notes:** Modifiers (e.g., "50% Đường, 70% Đá, Thêm Shot Espresso") utilize `body-sm` in caramel tone `#C78C4E` to ensure immediate distinction from the parent item.

## Layout & Spacing

The POS workspace follows an ergonomic 3-zone split architecture designed for landscape touch displays (typically 10.5" to 15.6" screens):

1. **Category Rail (Left, 96px - 140px fixed width):** Vertical icon + text category tabs (Cà Phê, Trà Sữa, Bánh Ngọt, v.v.) and table map switcher.
2. **Product Catalog Grid (Center, flexible fluid width):** 3 to 4 column responsive grid with square or 4:3 product cards optimized for rapid visual scanning.
3. **Receipt & Order Register (Right, 360px - 420px fixed width):** Full vertical height pinned register displaying line items, table assignment, payment methods, and total checkout buttons.

### Breakpoints & Adaptations
- **Desktop / Countertop POS (≥1024px Landscape):** 3-column concurrent layout with pinned right-hand cart and zero screen-switching needed for order placement.
- **Tablet Portrait (768px - 1023px):** Left category bar collapses to a horizontal scrollable chip bar above the product grid. Cart remains pinned on the right (320px).
- **Handheld Mobile / Barista Smartphone (<768px):** Single-column layout. Cart transforms into a persistent bottom sheet bar showing item count and total VND, expanding to a full-screen drawer upon tap.

## Elevation & Depth

To preserve peak rendering speed on POS hardware and prevent visual clutter under bright counter lamps, depth is conveyed through **tonal surface layering** combined with **subtle micro-borders**:

- **Surface 0 (Screen Background):** `#F4EFEA` (Warm stone cream).
- **Surface 1 (Modules & Product Cards):** `#FFFFFF` paired with an outline of `1px solid #E6DCD2`.
- **Surface 2 (Floating Popovers / Modifiers Modal):** `#FFFFFF` with an ambient shadow of `0 10px 25px -5px rgba(44, 24, 16, 0.12), 0 8px 10px -6px rgba(44, 24, 16, 0.08)`.
- **Order Panel Isolation:** The right-hand receipt drawer is defined by a vertical left boundary border (`1.5px solid #E2D7CD`) and an ultra-soft inner ambient gradient, ensuring clear functional separation from the product grid.
- **Interactive Depress State:** Touching an item card drops its scale (`scale(0.97)`) and shifts border color from `#E6DCD2` to `#C78C4E` for immediate optical verification.

## Shapes

The interface uses a consistent **Rounded (Level 2)** shape standard:
- **Product & Order Cards:** `rounded-lg` (`1rem` / 16px) creates approachable, modern tiles while maintaining optimal screen real estate.
- **Buttons & Touch Modifiers:** `rounded-md` (`0.5rem` / 8px) to `rounded-lg` (`1rem` / 16px) depending on size, offering clear affordance without visual harshness.
- **Category Badges & Status Pills:** Fully rounded pills (`9999px`) for network indicators (Online/Offline) and table occupancy tags.

## Components

### 1. Touch-First Product Card
- **Layout:** Image top (aspect 4:3 or 1:1), followed by item title in `headline-sm`, and bold price in `numeric-card` (`#2C1810`).
- **Quick Modifiers:** An inline "+" badge in caramel accent `#C78C4E` sits on the bottom right corner of each card for fast 1-tap addition of defaults.
- **Sold Out / Out of Stock:** Overlay with semi-transparent scrim (`rgba(244, 239, 234, 0.8)`), grayscale image, and centered badge "Hết hàng".

### 2. Category Selector
- Large vertical pill buttons on landscape setups.
- **Active State:** Deep Espresso background (`#2C1810`), white text, and secondary caramel active indicator bar.
- **Inactive State:** Transparent background, muted brown text (`#6E5D53`), with light hover/touch background `#EDE4DC`.

### 3. Order Cart & Slip (Right Panel)
- **Header:** Table number badge (e.g., "Bàn 12 - Tầng 1" or "Mang về") with time elapsed.
- **List Items:** Row contains Quantity adjuster (`-` `[count]` `+` touch buttons, minimum 36px hit-box), product name, modifiers indented below in caramel `#C78C4E`, and right-aligned subtotal.
- **Swipe-to-Remove:** Allows swift deletion with a single thumb drag to the left, revealing red delete action.

### 4. Fast Checkout Matrix (1-Click Actions)
- Located fixed at the bottom of the cart panel:
  - **Dynamic VietQR Button:** Blue-themed `#005BAA` with instant QR popover showing customer bill total, generating bank QR instantly.
  - **Cash Button ("Tiền mặt"):** `#2C1810` espresso fill with automatic suggested cash denomination chips (e.g., 50.000đ, 100.000đ, 200.000đ, 500.000đ) and calculated change output.
  - **Secondary Actions:** Split bill, Print Pro-forma receipt ("Tạm tính"), and Kitchen ticket dispatch ("Báo pha chế").

### 5. Network & System Indicator
- Fixed badge in the top bar:
  - **Online Mode:** Green pill (`#ECFDF5`), green dot with pulse animation, text "Hệ thống Online" (`#059669`).
  - **Offline / Local Cache Mode:** Amber/Red pill (`#FEF2F2`), warning icon, text "Offline - Lưu nội bộ" (`#DC2626`), alerting the cashier that orders are buffered locally in IndexedDB until reconnection.