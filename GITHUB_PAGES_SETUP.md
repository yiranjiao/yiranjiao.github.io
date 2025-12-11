# GitHub Pages Deployment Guide

Follow these steps to host your academic homepage on GitHub Pages.

## Step 1: Create a GitHub Account (if you don't have one)

1. Go to https://github.com
2. Click "Sign up"
3. Follow the registration process

## Step 2: Create a New Repository

1. Log in to GitHub
2. Click the **"+"** icon in the top-right corner
3. Select **"New repository"**
4. **Repository name**: Enter `your-username.github.io`
   - Replace `your-username` with your actual GitHub username
   - Example: If your username is `yiranjiao`, name it `yiranjiao.github.io`
   - ⚠️ **Important**: The repository name MUST be exactly `your-username.github.io`
5. Set to **Public** (required for free GitHub Pages)
6. Do NOT check "Initialize with README"
7. Click **"Create repository"**

## Step 3: Upload Your Files to GitHub

You have three options:

### Option A: Using GitHub Web Interface (Easiest)

1. In your new repository, click **"uploading an existing file"**
2. Drag and drop ALL files from the `yiran-homepage` folder:
   ```
   - _config.yml
   - index.md
   - Gemfile
   - .gitignore
   - README.md
   - DEPLOYMENT_GUIDE.md
   - assets/ (entire folder with all contents)
   ```
3. Scroll down and click **"Commit changes"**

### Option B: Using GitHub Desktop (Recommended)

1. Download GitHub Desktop: https://desktop.github.com
2. Install and sign in with your GitHub account
3. Click **File → Add Local Repository**
4. Browse to your `yiran-homepage` folder
5. If prompted to create a repository, click **"Create"**
6. Click **"Publish repository"**
7. Make sure the name is `your-username.github.io`
8. Uncheck "Keep this code private"
9. Click **"Publish repository"**

### Option C: Using Git Command Line

1. Open Terminal (Mac/Linux) or Command Prompt (Windows)
2. Navigate to your `yiran-homepage` folder:
   ```bash
   cd path/to/yiran-homepage
   ```
3. Run these commands (replace `your-username` with your GitHub username):
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Academic homepage"
   git branch -M main
   git remote add origin https://github.com/your-username/your-username.github.io.git
   git push -u origin main
   ```

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Click **"Pages"** (left sidebar)
4. Under **"Source"**:
   - Select **"Deploy from a branch"**
   - Choose **"main"** branch
   - Choose **"/ (root)"** folder
   - Click **"Save"**

## Step 5: Wait for Deployment

1. GitHub will start building your site (takes 1-5 minutes)
2. Refresh the Settings → Pages page
3. You'll see a green checkmark and your site URL when ready:
   ```
   Your site is live at https://your-username.github.io
   ```

## Step 6: Visit Your Site!

Open your browser and go to:
```
https://your-username.github.io
```

🎉 Your academic homepage is now live!

## Troubleshooting

### Site Not Showing Up?
- Wait 5-10 minutes after initial setup
- Check Settings → Pages for any error messages
- Make sure repository name is exactly `your-username.github.io`
- Verify files are in the root directory (not in a subfolder)

### Images Not Loading?
- Make sure the `assets` folder was uploaded with all files
- Check that `profile.jpg` and `header-bg.jpg` are in `assets/`
- Try clearing your browser cache

### CSS Not Working?
- Verify `assets/css/style.scss` was uploaded
- Make sure the file starts with `---` on line 1
- Wait a few minutes and refresh

### 404 Error?
- Repository name must be `your-username.github.io`
- Make sure branch is set to `main` in Settings → Pages
- Verify `index.md` is in the root directory

## Updating Your Site

Whenever you want to make changes:

### Using GitHub Web Interface:
1. Go to your repository
2. Click on the file you want to edit
3. Click the pencil icon (Edit)
4. Make your changes
5. Scroll down and click "Commit changes"
6. Wait 1-2 minutes, then refresh your site

### Using GitHub Desktop:
1. Edit files on your computer
2. Open GitHub Desktop
3. You'll see your changes listed
4. Add a commit message (e.g., "Updated experience section")
5. Click "Commit to main"
6. Click "Push origin"
7. Wait 1-2 minutes, then refresh your site

### Using Git Command Line:
```bash
# After editing files
git add .
git commit -m "Description of changes"
git push
```

## Customizing Your Site

### Update Your Personal Information
Edit `_config.yml`:
```yaml
title: Your Name
email: your.email@example.com
github_username: your-username
```

### Update Content
Edit `index.md` to change:
- About Me section
- Education details
- Work experience
- Research projects
- Skills

### Change Colors
Edit `assets/css/style.scss` to customize:
- Navigation bar colors
- Section colors
- Link colors
- Background colors

### Replace Background Image
Replace `assets/header-bg.jpg` with your own image

### Update CV
Replace `assets/Yiran_CV.pdf` with your latest CV

## Custom Domain (Optional)

If you want to use your own domain (e.g., `www.yourname.com`):

1. Buy a domain from a registrar (Namecheap, Google Domains, etc.)
2. In your repository, create a file named `CNAME` (no extension)
3. Add your domain to the file: `www.yourname.com`
4. Configure DNS settings at your domain registrar:
   - Add A records pointing to GitHub's IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Or add a CNAME record pointing to `your-username.github.io`
5. Wait 24-48 hours for DNS to propagate

## Need Help?

- GitHub Pages Documentation: https://docs.github.com/en/pages
- Jekyll Documentation: https://jekyllrb.com/docs/
- GitHub Community: https://github.community

## Quick Reference

**Your repository**: `https://github.com/your-username/your-username.github.io`  
**Your website**: `https://your-username.github.io`  
**Settings**: Repository → Settings → Pages

---

Good luck with your academic homepage! 🚀
