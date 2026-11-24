# 🍔 Tappy Food — Midnight Neon Gourmet Delivery

> **Production-Grade Food Delivery Application & Interactive CSS Selectors Masterclass**  
> *Theme: Midnight Navy with Neon Magenta Glow & Warm Golden Amber Highlights*

---

## 📋 Table of Contents
1. [Project Overview](#-project-overview)
2. [Design Theme & Visual Philosophy](#-design-theme--visual-philosophy)
3. [Design Language & Token Specifications](#-design-language--token-specifications)
4. [Budget Amount & Pricing Structure](#-budget-amount--pricing-structure)
5. [Component Architecture & Anatomy](#-component-architecture--anatomy)
6. [CSS Selectors Master Showcase](#-css-selectors-master-showcase)
7. [Directory Structure & Quick Start](#-directory-structure--quick-start)

---

## 🌟 Project Overview

**Tappy Food** is a production-ready, mobile-responsive web application for a premier food delivery platform. It combines a high-conversion, consumer-facing user experience with an educational showcase of modern CSS selectors.

The project demonstrates:
- A luxury **Midnight Navy & Neon Glow** visual identity.
- Production-grade semantic HTML5 layout and accessibility.
- Authentic high-resolution photography sourced from Unsplash.
- Complete demonstration of **all 10 categories of CSS Selectors** without external CSS frameworks.

---

## 🎨 Design Theme & Visual Philosophy

The design is built around the **Midnight Neon & Amber Gourmet** aesthetic, inspired by modern night-mode delivery applications (like DoorDash Premium, Deliveroo Gold, and high-end Asian street-eats platforms):

- **Foundation:** Deep Midnight Navy (`#0A0E1A` / `#0D1224`) providing a rich, cinema-grade canvas with subtle atmospheric radial glow accents.
- **Surface Elevation:** Dark Indigo Slate (`#13182B`) cards with subtle borders (`1px solid rgba(255, 255, 255, 0.08)`) and deep drop shadows.
- **Focal Typography:** Warm Golden Amber (`#FFB020`) for appetizing food titles and rating stars, commanding immediate visual hierarchy.
- **The Interaction Driver:** Vibrant Neon Magenta to Purple gradient (`linear-gradient(135deg, #FF007A, #7928CA)`) reserved for primary action pill buttons (`ORDER NOW`).

---

## 📐 Design Language & Token Specifications

### 1. Color Palette Tokens

| Token Name | Hex / Gradient Value | Purpose & Application |
| :--- | :--- | :--- |
| `--bg-body` | `#0A0E1A` | Main page canvas foundation |
| `--bg-card` | `#13182B` | Elevated card & container surface |
| `--bg-card-hover`| `#171E36` | Card background on hover interaction |
| `--bg-glass` | `rgba(19, 24, 43, 0.82)` | Sticky glassmorphic navigation bar |
| `--color-white` | `#FFFFFF` | Primary headlines, current price, active text |
| `--color-amber` | `#FFB020` | Dish titles, rating stars, brand accent |
| `--color-text-body` | `#94A3B8` | Item descriptions and general body copy |
| `--color-text-muted`| `#8E98B0` | Metadata labels, prep time, cuisine tags |
| `--color-text-dim` | `#64748B` | Strikethrough original prices, copyright |
| `--btn-gradient` | `linear-gradient(135deg, #FF007A 0%, #7928CA 100%)` | Primary "ORDER NOW" CTA button |
| `--btn-glow` | `0 6px 22px rgba(255, 0, 122, 0.45)` | Luminous button drop-glow |

### 2. Typography System

The interface pairs two Google Fonts:

```html
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800;900&family=Plus+Jakarta+Sans:ital,wght@0,400;0,500;0,600;0,700;0,800;1,400;1,600&display=swap" rel="stylesheet">
```

- **Headings & Display (`Outfit`):**
  - Hero Display Title: `clamp(2.8rem, 6vw, 4.2rem)`, `font-weight: 800`, `letter-spacing: -0.02em`
  - Section Titles: `clamp(1.9rem, 4vw, 2.5rem)`, `font-weight: 800`
  - Item Titles: `1.35rem`, `font-weight: 700`, color `--color-amber`
  - Action Buttons: `0.88rem`, `font-weight: 800`, uppercase, letter-spacing `0.06em`
  - Prices: `1.25rem`, `font-weight: 800`

- **Body Copy & Metadata (`Plus Jakarta Sans`):**
  - Body Text: `1rem`, `line-height: 1.6`
  - Item Descriptions: `0.92rem`, `line-height: 1.55`, color `--color-text-body`
  - Meta Tags & Time: `0.85rem`, `font-weight: 500`, color `--color-text-muted`

### 3. Corner Radii & Elevation

- **Buttons:** `border-radius: 9999px` (Full Pill)
- **Cards & Figures:** `border-radius: 18px` (`--rounded-lg`)
- **Inputs & Micro-Cards:** `border-radius: 10px` (`--rounded-md`)
- **Card Shadow:** `0 12px 32px rgba(0, 0, 0, 0.5)`
- **Hover Card Lift:** `transform: translateY(-5px); box-shadow: 0 18px 45px rgba(0, 0, 0, 0.65), 0 0 25px rgba(255, 0, 122, 0.15)`

---

## 💰 Budget Amount & Pricing Structure

The application models a **Moderate to Premium Casual** food delivery platform with dynamic price benchmarking and discount structures:

### 1. Best Seller Menu Item Pricing

| Item Name | Current Price | Original Benchmark | Discount | Budget Tier |
| :--- | :--- | :--- | :--- | :--- |
| **Wood-Fired Margherita Pizza** | **$13.99** | <del>$16.50</del> | **15% OFF** | Value Casual |
| **Chicken Tikka Masala Bowl** | **$14.49** | <del>$18.99</del> | **24% OFF** | Best Seller Budget |
| **Double Truffle Smash Burger** | **$15.49** | <del>$18.99</del> | **18% OFF** | Gourmet Casual |
| **Rainbow Dragon Sushi Roll (8pcs)** | **$17.99** | <del>$21.50</del> | **16% OFF** | Premium Fresh Catch |

### 2. Dining Category Budget Tiers

- **Street Food & Comfort Bowls:** `$12.00 – $16.00` per person
- **Artisan Bistro & Trattoria Meals:** `$16.00 – $26.00` per person
- **Luxury Teahouse & Fine Dining:** `$28.00 – $55.00+` multi-course set

### 3. Delivery Fees & Customer Savings

- **Minimum Order Requirement:** `$10.00`
- **Standard Courier Drop Fee:** `$1.99` (flat rate)
- **Free Delivery Threshold:** Orders **$25.00 and above** qualify for zero delivery fee.
- **First-Time Diner Promo:** Use code `TAPPY20` for **20% off** your first five bookings.

---

## 🧩 Component Architecture & Anatomy

### 1. Card Anatomy (Replicating the Reference Model)
```
+-----------------------------------------------------------+
| [ High-Resolution Food Image with Bottom Gradient Mask ]   |
+-----------------------------------------------------------+
| Popular • ⏱ 30 min                                        |
| ★ 4.8 Indian                                             |
|                                                           |
| Chicken Tikka Masala                                      |  <-- Warm Amber (#FFB020)
| Tender chunks of grilled chicken enveloped in a rich,    |
| creamy, and mildly spiced tomato sauce...                 |
|                                                           |
| $14.49  $18.99                         [ ORDER NOW ]      |  <-- Glowing Magenta Pill
+-----------------------------------------------------------+
```

### 2. Sticky Glassmorphic Navbar
- Floating pill structure centered at the top of the viewport (`sticky; top: 16px`).
- Background blur filter (`backdrop-filter: blur(16px)`).
- Glowing hover transitions on navigation anchor items.

### 3. Contact & Inquiries Form
- Dark high-contrast inputs (`#0B0E1B`) with inset shadow.
- Glowing magenta focus ring (`border-color: #FF007A; box-shadow: 0 0 16px rgba(255, 0, 122, 0.35)`).

---

## 📚 CSS Selectors Master Showcase

The stylesheet (`styles.css`) is structured to demonstrate **all fundamental and advanced CSS selector patterns**:

### 1. Universal Selector (`*`)
```css
*, *::before, *::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

### 2. Element / Type Selectors
Targets HTML tags directly: `html`, `body`, `header`, `main`, `footer`, `article`, `figure`, `figcaption`, `h1`, `h2`, `h3`, `p`, `ul`, `li`, `a`, `form`, `fieldset`, `legend`, `label`, `input`, `button`, `del`.

### 3. Class Selectors
Custom class names: `.heading`, `.navbar`, `.navlist`, `.card`, `.card-image-wrap`, `.card-content`, `.item-title`, `.item-desc`, `.btn-order`, `.text-amber`, `.price-current`.

### 4. ID Selectors
Unique page anchors: `#home`, `#about`, `#bestsellers`, `#best-restaurants`, `#top-restaurants`, `#contact`.

### 5. Grouping Selectors
Comma-separated selectors sharing identical layout rules:
```css
#bestsellers, #best-restaurants, #top-restaurants {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 30px;
}
```

### 6. Combinator Selectors
- **Descendant Combinator (`ancestor descendant`):**
  ```css
  article img { width: 100%; height: 220px; object-fit: cover; }
  header p { color: var(--color-text-muted); }
  ```
- **Child Combinator (`parent > child`):**
  ```css
  section > p { text-align: center; max-width: 720px; }
  ```
- **Adjacent Sibling Combinator (`prev + next`):**
  ```css
  label + input { margin-top: 2px; }
  .section_title + p { margin-top: -6px; }
  ```

### 7. Attribute Selectors
Styles elements according to HTML attributes:
```css
input[type="text"], input[type="email"], input[type="tel"] {
  width: 100%;
  background-color: var(--bg-input);
}
button[type="submit"] { width: 100%; }
a[target="_blank"] { cursor: pointer; }
```

### 8. Pseudo-Classes
- **Dynamic States:** `:hover`, `:active`, `:focus`, `:focus-visible`
- **Structural Pseudo-classes:** `:first-child`, `:not()`
  ```css
  button[type="button"]:not(.btn-order) { ... }
  #about ul li:first-child { border-top-color: rgba(255, 176, 32, 0.5); }
  ```

### 9. Pseudo-Elements
Styles generated content and document fragments:
```css
input::placeholder { color: var(--color-text-dim); }
::selection { background-color: #FF007A; color: #FFFFFF; }
::-webkit-scrollbar { width: 10px; }
::-webkit-scrollbar-thumb { background: linear-gradient(180deg, #FF007A, #7928CA); }
.card-image-wrap::after { ... } /* Dark gradient vignette overlay */
```

### 10. Responsive Media Queries
Adapts grid layouts, typography clamp sizes, and padding for viewports under `900px` (tablets) and `600px` (smartphones).

---

## 📁 Directory Structure & Quick Start

```
CSS Selectors/
├── index.html       # Complete semantic markup with Unsplash food imagery
├── styles.css       # Midnight Neon CSS theme with full selector showcase
└── README.md        # Comprehensive documentation (Theme, Budget, Language)
```

### Quick Start: Previewing Locally

1. Open File Explorer to `D:\HTML_2026\CSS Selectors\`.
2. Double-click `index.html` to open it in Google Chrome, Microsoft Edge, or Mozilla Firefox.
3. No build tools, Node servers, or compilers required — standard vanilla HTML5 and CSS3.

---

*Authored for the Tappy Food 2026 Web Development & UI Showcase.*
