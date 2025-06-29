# 🚀 Portfolio Deployment Guide

This guide will help you deploy your portfolio website to GitHub Pages for free hosting.

## Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository: `portfolio` or `my-portfolio`
5. Make it **Public** (required for free GitHub Pages)
6. Don't initialize with README (we already have one)
7. Click "Create repository"

## Step 2: Connect Local Repository to GitHub

Run these commands in your terminal:

```bash
# Add the remote repository (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# Push your code to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section (in the left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch
6. Select "/ (root)" folder
7. Click "Save"

## Step 4: Wait for Deployment

- GitHub will build and deploy your site
- This usually takes 2-5 minutes
- You'll see a green checkmark when it's ready
- Your site will be available at: `https://YOUR_USERNAME.github.io/portfolio`

## Alternative Deployment Options

### Option 1: Netlify (Recommended for Custom Domains)

1. Go to [netlify.com](https://netlify.com)
2. Sign up with GitHub
3. Click "New site from Git"
4. Choose your portfolio repository
5. Deploy settings:
   - Build command: (leave empty)
   - Publish directory: (leave empty)
6. Click "Deploy site"

### Option 2: Vercel

1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub
3. Click "New Project"
4. Import your portfolio repository
5. Click "Deploy"

### Option 3: Firebase Hosting

```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login to Firebase
firebase login

# Initialize project
firebase init hosting

# Deploy
firebase deploy
```

## Custom Domain Setup

### For GitHub Pages:
1. In repository Settings > Pages
2. Add your custom domain
3. Create a `CNAME` file in your repository with your domain
4. Update your DNS settings with your domain provider

### For Netlify:
1. Go to Site Settings > Domain management
2. Add custom domain
3. Update DNS settings

## Troubleshooting

### Common Issues:

1. **Site not loading**: Check if repository is public
2. **404 errors**: Ensure `index.html` is in the root directory
3. **Styling issues**: Check if CSS file paths are correct
4. **Images not loading**: Verify image paths and file names

### Performance Tips:

1. **Optimize images** before uploading
2. **Minify CSS/JS** for production
3. **Use CDN** for external libraries
4. **Enable Gzip** compression

## Post-Deployment Checklist

- [ ] Website loads correctly
- [ ] All links work properly
- [ ] Contact form functions (if backend is set up)
- [ ] Mobile responsiveness works
- [ ] Images load properly
- [ ] Social media links are updated
- [ ] SEO meta tags are in place
- [ ] Google Analytics is set up (optional)

## Updating Your Site

After making changes:

```bash
git add .
git commit -m "Update portfolio content"
git push origin main
```

GitHub Pages will automatically rebuild and deploy your changes.

## Support

If you encounter issues:
1. Check GitHub Pages documentation
2. Verify all file paths are correct
3. Ensure all files are committed and pushed
4. Check browser console for errors

---

**Your portfolio is now live! 🎉**

Share your URL: `https://YOUR_USERNAME.github.io/portfolio` 