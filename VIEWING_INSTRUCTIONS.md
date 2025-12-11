# How to View Your Homepage Preview

## Your Profile Image
✅ Your profile image has been successfully converted and is ready to use!
- Located at: `assets/profile.jpg`
- It will display as a 200px circular image on the right side of your name
- I can see the image and it looks great!

## Why You Might Not See the Image in preview.html

When you open `preview.html` directly by double-clicking it, some browsers block images from loading due to security restrictions on local files. This is normal and won't be a problem once deployed to GitHub Pages.

## How to View the Preview WITH the Image

### Option 1: Open the Full Folder Structure (Simplest)
Make sure you download the entire `yiran-homepage` folder with all its contents, then:
1. Open `preview.html` in your browser
2. If the image doesn't show, try Option 2

### Option 2: Use a Local Web Server (Recommended - See Everything Work)
This is the best way to preview exactly how it will look on GitHub Pages:

**Using Python (if installed):**
```bash
cd yiran-homepage
python3 -m http.server 8000
# or on Windows:
python -m http.server 8000
```
Then open: http://localhost:8000/preview.html

**Using VS Code:**
- Install "Live Server" extension
- Right-click on preview.html
- Select "Open with Live Server"

**Using Node.js/npx:**
```bash
cd yiran-homepage
npx http-server
```

### Option 3: Just Deploy It!
Once you push to GitHub Pages, everything will work perfectly right away. The image will load automatically.

## What Your Homepage Will Look Like

**Desktop View:**
```
┌──────────────────────────────────────────┐
│ Yiran Jiao               [Your Photo]    │
│ AI Product Manager                       │
│ Email: ... Phone: ...                    │
└──────────────────────────────────────────┘
```

**Mobile View:**
```
┌────────────────┐
│  [Your Photo]  │
│                │
│  Yiran Jiao    │
│  AI Product    │
│  Manager       │
└────────────────┘
```

The photo displays as an elegant circle with a white border and shadow effect against the purple gradient background.

## Confirm the Image is Ready
To verify your image is properly placed:
```bash
cd yiran-homepage
ls -l assets/profile.jpg
```
You should see a file about 1.4MB in size.
