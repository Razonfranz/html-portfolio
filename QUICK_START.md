# 🚀 Quick Start Guide

Get your portfolio live in under 10 minutes!

## ⚡ Fast Track to Deployment

### Step 1: Customize Your Info (5 minutes)

Open `index.html` and replace:

```html
<!-- Line 27: Your name -->
<h1 class="hero-title">Hi, I'm YOUR NAME</h1>

<!-- Line 28: Your title -->
<p class="hero-subtitle">Your Professional Title</p>

<!-- Lines 37-39: Your bio -->
<p>Write your own biography here...</p>

<!-- Line 97: Your email in form -->
<a href="mailto:YOUR_EMAIL@example.com">
```

### Step 2: Update Links (2 minutes)

Replace these links in `index.html`:

```html
<!-- Line 93: GitHub link -->
<a href="https://github.com/YOUR_USERNAME">

<!-- Line 101: LinkedIn link -->
<a href="https://linkedin.com/in/YOUR_PROFILE">

<!-- Line 109: Email -->
<a href="mailto:YOUR_EMAIL@example.com">
```

### Step 3: Deploy to GitHub (3 minutes)

Open PowerShell in your project folder:

```powershell
# Initialize and commit
git init
git add .
git commit -m "My professional portfolio"

# Push to GitHub (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/html-portfolio.git
git branch -M main
git push -u origin main
```

### Step 4: Enable GitHub Pages (1 minute)

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Source: **main** branch, **/ (root)** folder
4. Click **Save**

### Step 5: View Your Live Site! 🎉

After 2-3 minutes, visit:
```
https://YOUR_USERNAME.github.io/html-portfolio/
```

---

## 🎨 Optional Customization

### Change Colors (30 seconds)

Edit `css/styles.css` line 3:

```css
--primary-color: #2563eb;  /* Change this hex code */
```

**Quick color options:**
- Purple: `#7c3aed`
- Green: `#10b981`
- Red: `#ef4444`
- Orange: `#f59e0b`

### Add Your Projects (2 minutes each)

Edit `index.html` starting at line 75, update:
- Project title
- Description
- GitHub link
- Live demo link

### Setup Contact Form (2 minutes)

1. Go to [formspree.io](https://formspree.io/) → Sign up (free)
2. Create new form
3. Copy form ID
4. Update `index.html` line 84:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

---

## 📸 Add Real Images Later

Replace these placeholder files in `assets/` folder:
- `myprofile.png` - Your profile photo (300x300px)
- `project1.jpg` - First project screenshot (800x500px)
- `project2.jpg` - Second project screenshot
- `project3.jpg` - Third project screenshot

Then commit and push:
```powershell
git add assets/
git commit -m "Added real images"
git push
```

---

## 🆘 Troubleshooting

**Site not showing?**
- Wait 3-5 minutes after enabling Pages
- Check repository is **Public**
- Verify `index.html` is in root folder

**Images not loading?**
- Check file names match exactly (case-sensitive)
- Verify images are in `assets/` folder
- Make sure you pushed the files to GitHub

**Form not working?**
- Sign up at Formspree.io
- Get your unique form ID
- Update the form action URL

---

## 📚 Full Documentation

For detailed guides, see:
- **README.md** - Complete documentation
- **DEPLOYMENT.md** - Detailed deployment steps
- **CUSTOMIZATION.md** - Full customization guide
- **PROJECT_SUMMARY.md** - Feature list and checklist

---

## ✅ Pre-Deployment Checklist

Before going live, make sure:
- [ ] Updated name in hero section
- [ ] Updated bio in about section
- [ ] Changed GitHub username in links
- [ ] Updated email address
- [ ] Committed all changes
- [ ] Pushed to GitHub
- [ ] Enabled GitHub Pages

---

**Need help?** Check the full documentation files or open an issue on GitHub.

**Ready to go?** Follow the 5 steps above and you're live! 🚀
