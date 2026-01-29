# 🚀 Deployment Guide: GitHub + Vercel

## Step-by-Step Instructions

### Prerequisites
✅ GitHub account (create at https://github.com)
✅ Vercel account (create at https://vercel.com - use GitHub to sign up)
✅ Git installed on your computer (download from https://git-scm.com)

---

## Part 1: Upload to GitHub

### Step 1: Create GitHub Repository

1. Go to https://github.com
2. Click the **"+"** icon (top right) → **"New repository"**
3. Fill in:
   - **Repository name**: `jollof-pot-receipt`
   - **Description**: "Receipt generator for Jollof Pot Restaurant"
   - **Visibility**: Public ✅
   - **DO NOT** check "Add a README file" (we have one)
4. Click **"Create repository"**

### Step 2: Upload Files to GitHub

You have downloaded a ZIP file with these files:
```
jollof-pot-vercel/
├── index.html
├── vercel.json
├── .gitignore
├── README.md
└── DEPLOYMENT_GUIDE.md
```

**Option A: Using GitHub Web Interface (Easiest)**

1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop ALL files from the extracted folder
3. Scroll down, type commit message: "Initial commit"
4. Click **"Commit changes"**

**Option B: Using Git Command Line**

Open terminal/command prompt in the folder and run:

```bash
# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Jollof Pot Receipt Generator"

# Add your repository (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/jollof-pot-receipt.git

# Push to GitHub
git branch -M main
git push -u origin main
```

✅ Your code is now on GitHub!

---

## Part 2: Deploy to Vercel

### Step 1: Connect Vercel to GitHub

1. Go to https://vercel.com
2. Click **"Sign Up"**
3. Choose **"Continue with GitHub"**
4. Authorize Vercel to access your GitHub account

### Step 2: Import Project

1. On Vercel dashboard, click **"Add New..."** → **"Project"**
2. Find your repository: `jollof-pot-receipt`
3. Click **"Import"**

### Step 3: Configure Project

1. **Framework Preset**: Select "Other" (it's a static site)
2. **Root Directory**: Leave as `./`
3. **Build Settings**: Leave everything default (no build needed!)
4. Click **"Deploy"**

### Step 4: Wait for Deployment

- Vercel will deploy your site (takes 30-60 seconds)
- You'll see a progress screen
- When done, you'll get a URL like: `https://jollof-pot-receipt.vercel.app`

### Step 5: Test Your Live Site

1. Click **"Visit"** or go to your Vercel URL
2. Test the receipt generator:
   - Add items
   - Generate receipt
   - Download PDF
3. Share your URL with others!

✅ Your site is now LIVE!

---

## Part 3: Custom Domain (Optional)

### Add Your Own Domain

If you own a domain (e.g., jollofpot.com):

1. In Vercel project, go to **"Settings"** → **"Domains"**
2. Click **"Add"**
3. Enter your domain name
4. Follow DNS configuration instructions
5. Wait 24-48 hours for DNS propagation

---

## 🔄 Making Updates

### To Update Your Site:

**Option A: GitHub Web**
1. Go to your repository on GitHub
2. Click on `index.html`
3. Click the pencil icon (Edit)
4. Make changes
5. Click "Commit changes"
6. Vercel auto-deploys in 30 seconds!

**Option B: Git Command Line**
```bash
# Make your changes to index.html
# Then:
git add .
git commit -m "Updated menu prices"
git push
```

Vercel automatically detects changes and redeploys!

---

## 📊 Your Vercel Dashboard

After deployment, you can:
- ✅ View live site
- ✅ See deployment history
- ✅ Check visitor analytics
- ✅ Add custom domains
- ✅ Enable HTTPS (automatic)
- ✅ Set up environment variables

---

## 🐛 Troubleshooting

### Issue: "Build Failed"
**Solution**: This shouldn't happen with static HTML. Check that `vercel.json` was uploaded correctly.

### Issue: "PDF Download Not Working"
**Solution**: 
- Clear browser cache
- Try different browser
- Check browser console for errors (F12)

### Issue: "Page Shows 404"
**Solution**: 
- Ensure `index.html` is in root directory
- Check `vercel.json` is present
- Redeploy from Vercel dashboard

### Issue: "Fonts Not Loading"
**Solution**: 
- Google Fonts requires internet connection
- Fonts are loaded from CDN, so they should work automatically

---

## 🎉 Success Checklist

After following this guide, you should have:

✅ Repository on GitHub
✅ Live site on Vercel
✅ Custom Vercel URL (e.g., jollof-pot-receipt.vercel.app)
✅ Auto-deployment when you push changes
✅ Free HTTPS certificate
✅ Global CDN for fast loading

---

## 📞 Need Help?

- **GitHub Issues**: Report bugs on your repository
- **Vercel Docs**: https://vercel.com/docs
- **GitHub Docs**: https://docs.github.com

---

## 🎯 Next Steps

1. Share your URL with customers
2. Test on mobile devices
3. Add to your restaurant website
4. Print QR code linking to the generator
5. Train staff on using it

**Your URL**: https://YOUR-PROJECT-NAME.vercel.app

---

Made with ❤️ | Deployment made easy!
