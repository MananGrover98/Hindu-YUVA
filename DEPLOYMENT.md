# 🚀 Deployment Guide - Hindu YUVA Website

This guide will walk you through deploying your Hindu YUVA website to GitHub and Vercel.

## 📋 Prerequisites

Before starting, make sure you have:
- [Git](https://git-scm.com/) installed on your computer
- A [GitHub](https://github.com/) account
- A [Vercel](https://vercel.com/) account (free)

## 🔧 Step 1: Prepare Your Local Files

1. **Create a new folder** for your project (if you haven't already)
2. **Copy all your website files** into this folder:
   - `home.html`
   - `aboutus.html`
   - `events.html`
   - `gallery.html`
   - `resources.html`
   - `temple.html`
   - `academic.html`
   - `career.html`
   - `styles.css`
   - `script.js`
   - `favicon.png`
   - `README.md`
   - `vercel.json`
   - `.gitignore`
   - `LICENSE`

## 🌐 Step 2: Create GitHub Repository

### Option A: Using GitHub Web Interface (Recommended)

1. **Go to GitHub.com** and sign in
2. **Click the "+" icon** in the top right corner
3. **Select "New repository"**
4. **Fill in the details:**
   - Repository name: `hindu-yuva-umb`
   - Description: `Official website for Hindu YUVA at UMass Boston`
   - Make it **Public**
   - **Don't** initialize with README (we already have one)
5. **Click "Create repository"**

### Option B: Using Git Commands

```bash
# Navigate to your project folder
cd path/to/your/hindu-yuva-folder

# Initialize Git repository
git init

# Add all files
git add .

# Make initial commit
git commit -m "Initial commit: Hindu YUVA website"

# Add GitHub remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/hindu-yuva-umb.git

# Push to GitHub
git push -u origin main
```

## 📤 Step 3: Push Code to GitHub

If you used Option A (GitHub Web Interface), follow these steps:

```bash
# Navigate to your project folder
cd path/to/your/hindu-yuva-folder

# Initialize Git repository
git init

# Add all files
git add .

# Make initial commit
git commit -m "Initial commit: Hindu YUVA website"

# Add GitHub remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/hindu-yuva-umb.git

# Push to GitHub
git push -u origin main
```

## 🚀 Step 4: Deploy to Vercel

1. **Go to [vercel.com](https://vercel.com)**
2. **Sign up/Login** with your GitHub account
3. **Click "New Project"**
4. **Import your GitHub repository:**
   - Find `hindu-yuva-umb` in the list
   - Click "Import"
5. **Configure project settings:**
   - Project Name: `hindu-yuva-umb` (or leave default)
   - Framework Preset: **Other** (or leave as is)
   - Root Directory: `./` (leave as is)
6. **Click "Deploy"**

## ✅ Step 5: Verify Deployment

1. **Wait for deployment** (usually takes 1-2 minutes)
2. **Click on your project** in the Vercel dashboard
3. **Visit your live website** using the provided URL
4. **Test all pages** to make sure everything works:
   - Home page
   - About Us
   - Events
   - Gallery
   - Resources
   - Temple directory
   - Academic advising
   - Career advising

## 🔗 Step 6: Custom Domain (Optional)

### Add Custom Domain

1. **In Vercel dashboard**, go to your project
2. **Click "Settings"** tab
3. **Click "Domains"** in the left sidebar
4. **Add your domain** (e.g., `hinduyuva.umb.edu`)
5. **Follow DNS instructions** provided by Vercel

### DNS Configuration

You'll need to add these DNS records to your domain provider:

```
Type: CNAME
Name: @
Value: cname.vercel-dns.com
```

## 🔄 Step 7: Future Updates

### Making Changes

1. **Edit files locally**
2. **Commit and push to GitHub:**
   ```bash
   git add .
   git commit -m "Update: description of changes"
   git push origin main
   ```
3. **Vercel will automatically redeploy** your website

### Adding New Content

- **New events**: Edit `events.html`
- **New gallery images**: Edit `gallery.html`
- **Content updates**: Edit respective HTML files
- **Style changes**: Edit `styles.css`
- **Functionality**: Edit `script.js`

## 🛠️ Troubleshooting

### Common Issues

1. **Build fails on Vercel:**
   - Check that all file paths are correct
   - Ensure all files are committed to GitHub
   - Check the build logs in Vercel dashboard

2. **Images not loading:**
   - Make sure image files are in the repository
   - Check image paths in HTML files
   - Use relative paths (e.g., `./images/photo.jpg`)

3. **Styles not applying:**
   - Check that `styles.css` is properly linked
   - Verify CSS syntax is correct
   - Clear browser cache

4. **Navigation not working:**
   - Check that all HTML files exist
   - Verify file names match links
   - Test all internal links

### Getting Help

- **Vercel Documentation**: [vercel.com/docs](https://vercel.com/docs)
- **GitHub Help**: [help.github.com](https://help.github.com)
- **Contact Support**: Check the README.md for contact information

## 📱 Performance Tips

1. **Optimize images** before uploading
2. **Minimize CSS and JavaScript** for production
3. **Use WebP format** for images when possible
4. **Enable compression** in Vercel settings

## 🔒 Security

- **HTTPS is automatically enabled** by Vercel
- **Security headers** are configured in `vercel.json`
- **Regular updates** are recommended

## 📊 Analytics (Optional)

### Add Google Analytics

1. **Create Google Analytics account**
2. **Get tracking code**
3. **Add to your HTML files** before `</head>`:
   ```html
   <!-- Google Analytics -->
   <script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
   <script>
     window.dataLayer = window.dataLayer || [];
     function gtag(){dataLayer.push(arguments);}
     gtag('js', new Date());
     gtag('config', 'GA_MEASUREMENT_ID');
   </script>
   ```

---

## 🎉 Congratulations!

Your Hindu YUVA website is now live and ready for the community! 

**Next steps:**
- Share the website URL with your community
- Update content regularly
- Consider adding a CMS for easier content management
- Monitor website performance and user feedback

**Need help?** Check the README.md file or contact the development team.
