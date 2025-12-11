# Portfolio Customization Guide

Quick reference for customizing your portfolio website.

## 🎨 Change Colors

Edit `css/styles.css` (lines 2-11):

```css
:root {
  --primary-color: #2563eb;        /* Main blue - buttons, links */
  --primary-dark: #1d4ed8;         /* Darker blue - hover states */
  --text-color: #1f2937;           /* Main text color */
  --text-light: #6b7280;           /* Secondary text */
  --background-color: #ffffff;     /* Page background */
  --surface-color: #f9fafb;        /* Card backgrounds */
  --border-color: #e5e7eb;         /* Borders */
  --focus-color: #3b82f6;          /* Focus indicator */
}
```

### Popular Color Schemes

**Purple Theme:**
```css
--primary-color: #7c3aed;
--primary-dark: #6d28d9;
```

**Green Theme:**
```css
--primary-color: #10b981;
--primary-dark: #059669;
```

**Orange Theme:**
```css
--primary-color: #f59e0b;
--primary-dark: #d97706;
```

## 👤 Update Personal Information

### Hero Section (index.html, line 24)
```html
<h1 class="hero-title">Hi, I'm YOUR NAME</h1>
<p class="hero-subtitle">Your Title/Role</p>
<p class="hero-description">Your tagline or brief description</p>
```

### About Section (index.html, line 34)
Replace with your biography and update the profile image:
```html
<img src="assets/myprofile.png" alt="Your Name">
```

### Contact Information (index.html, line 90)
Update social media links:
```html
<a href="https://github.com/YOUR_USERNAME">
<a href="https://linkedin.com/in/YOUR_PROFILE">
<a href="mailto:your.email@example.com">
```

## 🛠️ Update Skills

Edit `index.html` (lines 45-70). Change skill names and proficiency levels:

```html
<article class="skill-card">
  <div class="skill-icon">🌐</div>
  <h3 class="skill-name">YOUR SKILL</h3>
  <div class="skill-bar">
    <div class="skill-progress" style="width: 90%;"></div>
  </div>
  <p class="skill-level">Advanced</p>
</article>
```

**Skill Icons (Emoji):**
- 🌐 HTML5
- 🎨 CSS3
- ⚡ JavaScript
- 📱 Responsive Design
- ♿ Accessibility
- 🐍 Python
- ⚛️ React
- 🎯 TypeScript
- 🔧 Git
- 🗄️ Database

Find more at [Emojipedia](https://emojipedia.org/)

## 📁 Update Projects

Edit `index.html` (lines 75-120):

```html
<article class="project-card">
  <div class="project-image-wrapper">
    <img src="assets/YOUR_PROJECT_IMAGE.jpg" alt="Project description">
  </div>
  <div class="project-content">
    <h3 class="project-title">Project Title</h3>
    <p class="project-description">Project description...</p>
    <div class="project-tags">
      <span class="tag">HTML5</span>
      <span class="tag">CSS3</span>
    </div>
    <div class="project-links">
      <a href="YOUR_GITHUB_LINK">View Code</a>
      <a href="YOUR_LIVE_DEMO_LINK">Live Demo</a>
    </div>
  </div>
</article>
```

### Adding More Projects

Simply copy the entire `<article class="project-card">` block and paste it before the closing `</div>` of `projects-grid`.

### Project Images

1. Take screenshots of your projects (recommended: 800x500px)
2. Save them in the `assets/` folder
3. Update the image path in your HTML

## 📧 Setup Contact Form

1. Go to [Formspree.io](https://formspree.io/)
2. Sign up for a free account
3. Create a new form
4. Copy your form endpoint
5. Update `index.html` (line 84):

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

## 🎯 Customize Hero Gradient

Edit `css/styles.css` (line 110):

```css
.hero {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

**Gradient Generator:** [CSSGradient.io](https://cssgradient.io/)

## 📱 Adjust Responsive Breakpoints

Edit `css/styles.css` (lines 380-450):

Current breakpoints:
- Mobile: < 768px
- Tablet: 768px - 1023px
- Desktop: ≥ 1024px

## 🔤 Change Fonts

### Using Google Fonts

1. Visit [Google Fonts](https://fonts.google.com/)
2. Select a font
3. Add to `index.html` `<head>`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
```

4. Update `css/styles.css`:

```css
:root {
  --font-family: 'Inter', sans-serif;
}
```

## 🖼️ Replace Placeholder Images

Current placeholder images:
- `assets/myprofile.png` - Your profile photo (300x300px recommended)
- `assets/project1.jpg` - Project screenshot
- `assets/project2.jpg` - Project screenshot
- `assets/project3.jpg` - Project screenshot

### Image Optimization Tips:
- Use `.jpg` for photos
- Use `.png` for logos/graphics with transparency
- Optimize images with [TinyPNG](https://tinypng.com/)
- Recommended max width: 1200px

## 🔧 Add/Remove Sections

### To Add a New Section:

1. Add navigation link in header:
```html
<li><a href="#new-section" class="nav-link">New Section</a></li>
```

2. Add section in main:
```html
<section id="new-section" class="section">
  <h2 class="section-title">New Section</h2>
  <!-- Your content here -->
</section>
```

3. Add styles in `css/styles.css`

### To Remove a Section:

1. Delete the navigation link
2. Delete the entire `<section>` block
3. Remove related CSS if needed

## 📊 Add Analytics (Optional)

To track visitors with Google Analytics:

1. Create account at [Google Analytics](https://analytics.google.com/)
2. Get your tracking ID
3. Add before `</head>` in `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_TRACKING_ID');
</script>
```

## 🚀 Performance Tips

1. **Optimize Images:** Use [Squoosh](https://squoosh.app/)
2. **Minify CSS:** Use [CSSMinifier](https://cssminifier.com/)
3. **Lazy Loading:** Images already have `loading="lazy"`
4. **Preload Critical CSS:** Already implemented

## ✅ Validation Tools

- **HTML:** [W3C HTML Validator](https://validator.w3.org/)
- **CSS:** [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- **Accessibility:** [WAVE](https://wave.webaim.org/)
- **Mobile-Friendly:** [Google Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)

## 🆘 Need Help?

- Review the main README.md
- Check DEPLOYMENT.md for deployment issues
- Search on [Stack Overflow](https://stackoverflow.com/)
- Ask on [GitHub Discussions](https://github.com/orgs/community/discussions)

---

Happy customizing! 🎨
