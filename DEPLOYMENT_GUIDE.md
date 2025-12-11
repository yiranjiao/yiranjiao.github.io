# Quick Deployment Guide for GitHub Pages

## Step 1: Create GitHub Repository

1. Go to https://github.com and sign in
2. Click the "+" icon in the top right corner and select "New repository"
3. Name your repository: `your-username.github.io` 
   - **Important**: Replace `your-username` with your actual GitHub username
   - Example: If your username is "yiranjiao", name it "yiranjiao.github.io"
4. Set it to "Public"
5. Do NOT initialize with README (we already have one)
6. Click "Create repository"

## Step 2: Upload Files to GitHub

### Option A: Using Git Command Line

1. Open Terminal/Command Prompt
2. Navigate to the folder containing these files
3. Run these commands:

```bash
git init
git add .
git commit -m "Initial commit: Academic homepage"
git branch -M main
git remote add origin https://github.com/your-username/your-username.github.io.git
git push -u origin main
```

### Option B: Using GitHub Desktop

1. Download and install GitHub Desktop
2. File → Add Local Repository → Choose this folder
3. Commit changes with message "Initial commit: Academic homepage"
4. Publish repository to GitHub
5. Make sure the repository name is `your-username.github.io`

### Option C: Using GitHub Web Interface

1. In your new repository on GitHub, click "uploading an existing file"
2. Drag and drop all files from this folder
3. Commit the files

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Source":
   - Select "Deploy from a branch"
   - Choose "main" branch
   - Choose "/ (root)" folder
   - Click "Save"

## Step 4: Wait and Access

- GitHub will build your site (takes 1-5 minutes)
- Your site will be live at: `https://your-username.github.io`
- You'll see a green checkmark when it's ready

## Customization

### Before Deploying:

1. Edit `_config.yml`:
   - Replace `your-github-username` with your actual username

2. Edit `index.md`:
   - Review all content for accuracy
   - Update any information as needed

### After Deploying:

- Any changes you push to the repository will automatically update your site
- Changes typically appear within 1-2 minutes

## Troubleshooting

**Site not showing up?**
- Wait 5 minutes after initial setup
- Check Settings → Pages to see if there are any errors
- Make sure repository name is exactly `your-username.github.io`

**CSS not loading?**
- Make sure `assets/css/style.scss` is in your repository
- Check that file starts with two lines of three dashes `---`

**Need help?**
- GitHub Pages Documentation: https://docs.github.com/en/pages
- Jekyll Documentation: https://jekyllrb.com/docs/

## Local Testing (Optional)

If you want to preview changes before pushing:

1. Install Ruby (https://www.ruby-lang.org/en/downloads/)
2. Install Bundler: `gem install bundler`
3. In this folder, run: `bundle install`
4. Run: `bundle exec jekyll serve`
5. Open browser to: `http://localhost:4000`

## Updating Your Site

1. Edit the files locally
2. Commit changes: `git add . && git commit -m "Update content"`
3. Push to GitHub: `git push`
4. Changes will appear on your site in 1-2 minutes
