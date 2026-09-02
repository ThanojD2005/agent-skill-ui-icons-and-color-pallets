name: select-modern-color-pallets
description: When have requirment to add/use color pallets in the project, use the below options to add the colors in the project

Body:

### Overview
Whenever a project requires color selection, styling, or theme tokens, always choose one of the curated **Modern Color Palettes** below. These options are derived from verified modern design palettes on [Coolors.co](./refferences/color.md).

---

### Critical Restrictions & Guidelines

1. **PROHIBITED: Common / Generic AI Zinc Palette**
   Do **NOT** use the overused, generic AI-template color scheme:
   - `Canvas Background: Obsidian Zinc (#09090B)`
   - `Card / Surface: Elevated Dark Slate (#121215)`
   - `Hairline Border: Subtle Zinc Border (#27272A)`
   - `AI Magic Accent: Electric Indigo / Violet (#6366F1 / #8B5CF6)`
   - `Active Highlight: Cyber Cyan (#06B6D4)`
   - `Primary Text: Ghost White (#F4F4F5)`
   - `Muted Text: Ash Gray (#71717A)`
   *Always select from the curated modern alternatives below instead.*

2. **Gradient Rule: Simple & Modern Look Only**
   - **No heavy, chaotic, or multi-stop rainbow gradients.**
   - Use only **subtle, 2-stop tonal linear transitions** (e.g., matching hue shifted by 5-10% lightness) or **low-opacity ambient glows (5% to 12% opacity)**.
   - Keep surfaces flat or gently frosted with glassmorphism rather than loud gradient fills.

---

### Step-by-Step Instructions

#### 1. Select the Best-Fit Palette for the Project
Choose the palette that matches the product's industry and mood:

* **Option 1: Modern Organic & Warm Minimalist** (Lifestyle, Eco, Wellness, Portfolios, Slow Living)
* **Option 2: Contemporary Coastal & Warm Sunset** (Modern Web Apps, Creative Studios, Consumer Platforms)
* **Option 3: Business Authority & Slate Steel** (FinTech, SaaS Dashboards, Enterprise Data)
* **Option 4: Minimalist Forest Slate** (Developer Tooling, Architecture, Engineering Portfolios)
* **Option 5: Midnight Luxury & Amber Gold** (Dark-Mode Products, Premium Brands, Media)
* **Option 6: Neutral Cashmere & Editorial** (Fashion, Publishing, Modern Clean Showcases)

---

### Approved Modern Color Options

#### Option 1: Modern Organic & Warm Minimalist (Bohemian Earth)
A calming, grounded aesthetic featuring warm creams, muted sage, and rich caramel.

* **Swatches**:
  - `Canvas Background`: `#FEFAE0` (Warm Alabaster)
  - `Card / Surface`: `#FFFFFF` (Crisp White)
  - `Sub-surface / Fills`: `#FAEDCD` (Papaya Cream)
  - `Hairline Border`: `#E9EDC9` (Matcha Tint)
  - `Subtle Accent / Tags`: `#CCD5AE` (Sage Green)
  - `Primary Action / CTA`: `#D4A373` (Oat Caramel)
  - `Primary Text`: `#2B2D42` (Deep Slate Indigo)
  - `Muted Text`: `#725D68` (Taupe Gray)

* **Simple Modern Gradients**:
  ```css
  /* Subtle page background transition */
  --gradient-bg-subtle: linear-gradient(180deg, #FEFAE0 0%, #F5F1D3 100%);
  /* Gentle 2-stop button gradient */
  --gradient-btn-action: linear-gradient(135deg, #D4A373 0%, #C39260 100%);
  ```

---

#### Option 2: Contemporary Coastal & Warm Sunset (Sunny Beach Day)
A warm, balanced palette pairing deep maritime charcoal with sunset terracotta.

* **Swatches**:
  - `Canvas Background`: `#264653` (Charcoal Blue)
  - `Card / Surface`: `#1D353F` (Elevated Marine Slate)
  - `Hairline Border`: `rgba(42, 157, 143, 0.25)` (Muted Verdigris Line)
  - `Secondary Accent`: `#2A9D8F` (Verdigris Teal)
  - `Highlight Accent`: `#E9C46A` (Golden Sand)
  - `Secondary Warm Accent`: `#F4A261` (Sandy Coral)
  - `Primary Action / CTA`: `#E76F51` (Burnt Sienna)
  - `Primary Text`: `#F8FAFC` (Pure Slate White)
  - `Muted Text`: `#94A3B8` (Cool Slate Silver)

* **Simple Modern Gradients**:
  ```css
  /* Subtle dark surface depth */
  --gradient-card-surface: linear-gradient(135deg, #1D353F 0%, #172B33 100%);
  /* Warm 2-stop CTA glow */
  --gradient-btn-action: linear-gradient(135deg, #E76F51 0%, #D65A3C 100%);
  ```

---

#### Option 3: Business Authority & Slate Steel
Sharp, high-contrast, and professional without feeling sterile.

* **Swatches**:
  - `Canvas Background`: `#EDF2F4` (Anti-Flash White)
  - `Card / Surface`: `#FFFFFF` (Pure Surface White)
  - `Hairline Border`: `rgba(141, 153, 174, 0.28)` (Subtle Steel Border)
  - `Structural Steel`: `#8D99AE` (Slate Steel)
  - `Primary Text / Brand`: `#2B2D42` (Dark Space Indigo)
  - `Primary Action / CTA`: `#EF233C` (Imperial Red)
  - `Hover / Active State`: `#D90429` (Crimson Flag)
  - `Muted Text`: `#5D687A` (Deep Muted Slate)

* **Simple Modern Gradients**:
  ```css
  /* Clean linear backdrop */
  --gradient-bg-subtle: linear-gradient(180deg, #EDF2F4 0%, #E2E8EB 100%);
  /* Sleek red action gradient */
  --gradient-btn-action: linear-gradient(135deg, #EF233C 0%, #D90429 100%);
  ```

---

#### Option 4: Minimalist Forest Slate
A muted, biophilic slate scheme for technical and architectural products.

* **Swatches**:
  - `Canvas Background`: `#2F3E46` (Deep Forest Slate)
  - `Card / Surface`: `#253339` (Elevated Shadow Slate)
  - `Hairline Border`: `#354F52` (Dark Slate Gray)
  - `Muted Fill / Badges`: `#52796F` (Hooker's Green)
  - `Primary Action / Accent`: `#84A98C` (Cambridge Sage)
  - `Light Highlight / Contrast`: `#CAD2C5` (Ash Green Light)
  - `Primary Text`: `#F1F5F3` (Crisp Off-White)
  - `Muted Text`: `#9EADA7` (Muted Sage Gray)

* **Simple Modern Gradients**:
  ```css
  /* Ambient dark angle gradient */
  --gradient-card-surface: linear-gradient(135deg, #2F3E46 0%, #243137 100%);
  /* Soft sage button gradient */
  --gradient-btn-action: linear-gradient(135deg, #84A98C 0%, #72977A 100%);
  ```

---

#### Option 5: Midnight Luxury & Amber Gold
High-end dark mode balancing rich prussian navy depth with striking amber accents.

* **Swatches**:
  - `Canvas Background`: `#000000` (Obsidian Base)
  - `Card / Surface`: `#14213D` (Prussian Dark Navy)
  - `Hairline Border`: `rgba(255, 255, 255, 0.12)` (Translucent Hairline)
  - `Primary Action / CTA`: `#FCA311` (Vibrant Amber Gold)
  - `Action Hover`: `#E59208` (Deep Amber)
  - `Primary Text`: `#E5E5E5` (Platinum Silver)
  - `High-Contrast Accent`: `#FFFFFF` (Pure White)
  - `Muted Text`: `#8E9AA8` (Muted Navy Gray)

* **Simple Modern Gradients**:
  ```css
  /* Low-key luxurious card gradient */
  --gradient-card-surface: linear-gradient(135deg, #14213D 0%, #0E172B 100%);
  /* Warm gold accent gradient */
  --gradient-btn-action: linear-gradient(135deg, #FCA311 0%, #E59208 100%);
  ```

---

#### Option 6: Neutral Cashmere & Editorial
A clean, editorial aesthetic replacing sterile white with warm parchment and subtle blush.

* **Swatches**:
  - `Canvas Background`: `#F4F3EE` (Isabelline Pearl)
  - `Card / Surface`: `#FFFFFF` (Elevated White)
  - `Hairline Border`: `#BCB8B1` (French Gray)
  - `Soft Accent / Pills`: `#E0AFA0` (Dusty Powder Rose)
  - `Muted Label / Secondary`: `#8A817C` (Grey Olive)
  - `Primary Text / Headlines`: `#463F3A` (Espresso Taupe)
  - `Muted Text`: `#6D6661` (Warm Slate Gray)

* **Simple Modern Gradients**:
  ```css
  /* Soft editorial canvas fade */
  --gradient-bg-subtle: linear-gradient(180deg, #F4F3EE 0%, #EAE9E3 100%);
  /* Delicate warm blush button */
  --gradient-btn-action: linear-gradient(135deg, #E0AFA0 0%, #CF9E8F 100%);
  ```

---

### Standard CSS Variable Template
When initializing colors in a stylesheet (`styles.css` or `globals.css`), always use clear semantic design tokens:

```css
:root {
  /* Surface & Background */
  --color-bg-base: #FEFAE0;
  --color-bg-surface: #FFFFFF;
  --color-border: #E9EDC9;

  /* Typography */
  --color-text-primary: #2B2D42;
  --color-text-secondary: #725D68;

  /* Brand & Actions */
  --color-accent-primary: #D4A373;
  --color-accent-hover: #C39260;
  --color-accent-subtle: rgba(212, 163, 115, 0.12);

  /* Simple Modern Gradients (2-Stop Only) */
  --gradient-bg: linear-gradient(180deg, #FEFAE0 0%, #F5F1D3 100%);
  --gradient-cta: linear-gradient(135deg, #D4A373 0%, #C39260 100%);
}
```

---

### Quality Checklist Before Deployment
- [ ] Ensure the generic Zinc/Obsidian/Electric Indigo combination was **not** used.
- [ ] Gradients are **2-stop simple tonal shifts** and not multi-colored rainbow ramps.
- [ ] Text-to-background contrast satisfies WCAG 2.1 AA (minimum 4.5:1 ratio for normal text).
- [ ] All colors are mapped to CSS custom properties (`var(--color-...)`) rather than raw hardcoded hex codes in component styles.