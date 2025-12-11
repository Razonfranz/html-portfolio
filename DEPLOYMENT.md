# GitHub Pages Deployment Guide

This guide will help you deploy your portfolio website to GitHub Pages.

## Prerequisites
- GitHub account
- Git installed on your computer
- Your portfolio files ready

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com/) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository: `html-portfolio` (or any name you prefer)
5. Make sure it's set to **Public**
6. **Do NOT** initialize with README (we already have one)
7. Click "Create repository"

## Step 2: Push Your Code to GitHub

Open PowerShell in your project folder and run these commands:

```powershell
# Initialize git repository (if not already done)
git init

# Add all files
git add .

# Commit your files
git commit -m "Initial commit - Complete portfolio website"

# Add your GitHub repository as remote
# Replace YOUR_USERNAME with your GitHub username
git remote add origin https://github.com/YOUR_USERNAME/html-portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** section (left sidebar)
4. Under "Source", select **main** branch
5. Select **/ (root)** folder
6. Click **Save**

## Step 4: Access Your Live Website

After a few minutes, your site will be live at:
```
https://YOUR_USERNAME.github.io/html-portfolio/
```

For example: `https://bh69.github.io/html-portfolio/`

## Step 5: Update Your README

Once deployed, update the live demo link in your README.md file with your actual GitHub Pages URL.

## Troubleshooting

### Site not loading?
- Wait 2-5 minutes after enabling GitHub Pages
- Check that your repository is public
- Verify that `index.html` is in the root directory
- Check GitHub Actions tab for deployment status

### Images not showing?
- Ensure all image paths are relative (e.g., `assets/myprofile.png`)
- Check that image files are committed and pushed
- Verify file names match exactly (case-sensitive)

### Contact form not working?
1. Sign up at [Formspree.io](https://formspree.io/)
2. Create a new form
3. Copy your form endpoint
4. Update the form action in `index.html`:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

## Making Updates

After making changes to your website:

```powershell
# Add changes
git add .

# Commit changes
git commit -m "Description of your changes"

# Push to GitHub
git push
```

Your site will automatically update in a few minutes!

## Custom Domain (Optional)

To use a custom domain like `www.yourname.com`:

1. Buy a domain from a registrar (Namecheap, GoDaddy, etc.)
2. In repository Settings → Pages → Custom domain
3. Enter your domain name
4. Configure DNS records at your domain registrar
5. Enable "Enforce HTTPS"

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [Markdown Guide](https://www.markdownguide.org/)

## Need Help?

- Check [GitHub Pages Status](https://www.githubstatus.com/)
- Visit [GitHub Community](https://github.community/)
- Review deployment logs in your repository's Actions tab

---

Good luck with your deployment! 🚀
