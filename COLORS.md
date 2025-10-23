# Casa Bruja Color Palette

Colors inspired by the Casa Bruja logo and mystical intro video aesthetic.

## 🎨 Primary Colors

### Dark Navy
- **Variable:** `--dark`
- **Hex:** `#0D0D1F`
- **RGB:** `rgb(13, 13, 31)`
- **Usage:** Main dark backgrounds, hero overlay

### Deep Purple
- **Variable:** `--purple`
- **Hex:** `#7B3FE4`
- **RGB:** `rgb(123, 63, 228)`
- **Usage:** Primary accent color, headings, logo text, buttons

### Bright Purple
- **Variable:** `--bright-purple`
- **Hex:** `#9B5FFF`
- **RGB:** `rgb(155, 95, 255)`
- **Usage:** Lighter purple accents, glows, hover states

## 🌟 Accent Colors

### Warm Gold
- **Variable:** `--gold`
- **Hex:** `#E8D78F`
- **RGB:** `rgb(232, 215, 143)`
- **Usage:** Navigation hover, dividers, mystical accents

### Candle Glow
- **Variable:** `--candle-glow`
- **Hex:** `#FFD99A`
- **RGB:** `rgb(255, 217, 154)`
- **Usage:** Warm glows, button borders, magical highlights

## 🤍 Neutral Colors

### Cream
- **Variable:** `--cream`
- **Hex:** `#F5F0E8`
- **RGB:** `rgb(245, 240, 232)`
- **Usage:** Light backgrounds, product cards, main text on dark

### Mist
- **Variable:** `--mist`
- **Hex:** `#E8E4DC`
- **RGB:** `rgb(232, 228, 220)`
- **Usage:** Secondary text, soft backgrounds

### Navy (Secondary Dark)
- **Variable:** `--navy`
- **Hex:** `#1A1A3E`
- **RGB:** `rgb(26, 26, 62)`
- **Usage:** Navigation background, section backgrounds

### Forest Green
- **Variable:** `--forest`
- **Hex:** `#2C3E2E`
- **RGB:** `rgb(44, 62, 46)`
- **Usage:** Text on light backgrounds, product descriptions

### Terracotta
- **Variable:** `--terracotta`
- **Hex:** `#C17C5A`
- **RGB:** `rgb(193, 124, 90)`
- **Usage:** Warm earthy accents (optional use)

## 🎭 Color Combinations

### Hero Section
- Background: `--dark` with gradient overlay
- Title: `--bright-purple` with glow effect
- Subtitle: `--gold`
- Description: `--mist`
- CTA Button: `--purple` to `--bright-purple` gradient, `--candle-glow` border

### Product Cards
- Background: `--cream`
- Title: `--purple`
- Description: `--forest`
- Hover: Lift effect with purple shadow

### Navigation
- Background: `--navy` (semi-transparent)
- Links: `--cream`
- Hover: `--gold`

### Contact Section
- Background: `--purple` gradient with transparency
- Text: `--mist`
- Links: `--gold` → `--purple` on hover

## 💫 Shadow & Glow Effects

### Text Shadows
```css
/* Purple glow for main title */
text-shadow: 0 0 30px rgba(123, 63, 228, 0.9), 
             0 0 60px rgba(155, 95, 255, 0.5);

/* Gold glow for accents */
text-shadow: 0 0 20px rgba(232, 215, 143, 0.6);
```

### Box Shadows
```css
/* Purple glow for buttons */
box-shadow: 0 5px 20px rgba(123, 63, 228, 0.4);

/* Hover state */
box-shadow: 0 8px 30px rgba(155, 95, 255, 0.6);
```

## 🌈 Gradient Formulas

### Purple Gradient (Buttons)
```css
background: linear-gradient(135deg, #7B3FE4, #9B5FFF);
```

### Dark Overlay (Hero)
```css
background: linear-gradient(180deg, 
    rgba(10, 10, 21, 0.5) 0%, 
    rgba(26, 26, 46, 0.3) 50%, 
    rgba(42, 42, 62, 0.6) 100%);
```

### Section Backgrounds
```css
background: linear-gradient(180deg, #0D0D1F, #2C3E2E);
```

---

**Color Inspiration:**
- Logo: Deep navy, vibrant purple, warm gold
- Video: Mystical nighttime ambiance, candlelight, purple glow
- Anthropologie: Natural, earthy, bohemian elegance
