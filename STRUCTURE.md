# HTML Structure Guide

Quick reference for editing the Casa Bruja website structure.

## 📄 File Structure

The website is a single-page application with all sections in one HTML file:

```
index.html
├── <head>
│   ├── Meta tags & title
│   ├── Google Fonts
│   └── <style> (All CSS here)
└── <body>
    ├── Video Intro
    ├── Navigation
    ├── Hero Section
    ├── About Section
    ├── Products Section
    ├── Shop Section
    ├── Events Section
    ├── Contact Section
    ├── Footer
    └── <script> (All JavaScript here)
```

## 🎯 Section IDs for Navigation

```html
#home      → Hero section
#about     → About section
#products  → Product collection
#shop      → Shop options
#events    → Events & Instagram
#contact   → Contact form
```

## 📝 Key Sections to Edit

### 1. Logo (Line ~550)
```html
<div class="logo-container">
    <img src="data:image/jpeg;base64,..." alt="Casa Bruja Logo">
</div>
```
**To change:** Replace the base64 data with `src="images/logo.jpg"`

### 2. Hero Text (Line ~560)
```html
<h1>CASA BRUJA</h1>
<p class="hero-description">
    A mystical sanctuary on wheels...
</p>
```

### 3. About Section (Line ~600)
```html
<section id="about">
    <h2>Our Story</h2>
    <div class="about-content">
        <div class="about-text">...</div>
        <div class="about-image"></div>
    </div>
</section>
```

### 4. Product Cards (Line ~650)
Each product follows this structure:
```html
<div class="product-card product-card-1">
    <div class="product-image">
        <img src="data:image/jpeg;base64,..." alt="Product Name">
    </div>
    <div class="product-content">
        <h3>Product Name</h3>
        <p>Product description...</p>
    </div>
</div>
```

### 5. Contact Info (Line ~850)
```html
<div class="contact-info">
    <p>✦ Based in San Antonio, Texas</p>
    <p>✉ <a href="mailto:jeanny@casabrujasa.com">jeanny@casabrujasa.com</a></p>
</div>
```

## 🎨 CSS Variables (Line ~50)

Change site-wide colors by editing these:
```css
:root {
    --purple: #7B3FE4;
    --bright-purple: #9B5FFF;
    --gold: #E8D78F;
    --candle-glow: #FFD99A;
    --dark: #0D0D1F;
    --navy: #1A1A3E;
    --cream: #F5F0E8;
    --forest: #2C3E2E;
    --mist: #E8E4DC;
    --terracotta: #C17C5A;
}
```

## 🎬 Video Settings (Line ~520)

```html
<iframe 
    src="https://www.youtube.com/embed/Xr5wbI6Dyf4?autoplay=1&mute=1..."
</iframe>
```
**To change video:** Replace `Xr5wbI6Dyf4` with new YouTube video ID

**To change duration:** Modify line in JavaScript:
```javascript
setTimeout(endIntro, 9000); // 9 seconds
```

## 📱 Responsive Breakpoints (Line ~480)

```css
@media (max-width: 768px) {
    /* Mobile styles */
}
```

## ⚡ JavaScript Functions (Line ~900)

### Video Intro Control
```javascript
function endIntro() {
    videoIntro.classList.add('fade-out');
}
```

### Hero Slideshow
```javascript
function nextSlide() {
    // Cycles through background images
}
setInterval(nextSlide, 5000); // Change every 5 seconds
```

### Navbar Scroll Effect
```javascript
window.addEventListener('scroll', () => {
    // Shows navbar after scrolling past 80% of viewport
});
```

## 🔧 Common Edits

### Change Navigation Links
```html
<nav id="navbar">
    <ul>
        <li><a href="#home">Home</a></li>
        <!-- Add/remove/modify links -->
    </ul>
</nav>
```

### Update Product Information
Find the product card and edit:
```html
<h3>Product Name</h3>
<p>New description here...</p>
```

### Change Social Links
```html
<div class="social-links">
    <a href="https://www.instagram.com/casabrujasa/" ...>◈</a>
    <a href="mailto:jeanny@casabrujasa.com" ...>✉</a>
</div>
```

### Modify Footer
```html
<footer>
    <p>© 2025 Casa Bruja · House Witch Boutique · San Antonio, Texas</p>
</footer>
```

## 💡 Tips for VS Code

### Install Helpful Extensions:
- **Live Server** - Preview changes in real-time
- **HTML CSS Support** - Better autocomplete
- **Prettier** - Code formatting
- **Color Highlight** - See colors in code

### Useful VS Code Shortcuts:
- `Ctrl/Cmd + /` - Comment/uncomment
- `Alt + Up/Down` - Move line up/down
- `Ctrl/Cmd + D` - Select next occurrence
- `Ctrl/Cmd + F` - Find
- `Ctrl/Cmd + H` - Find and replace

---

**Need help?** Check README.md for general project info or COLORS.md for color palette details.
