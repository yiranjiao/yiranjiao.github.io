# Yiran Jiao - Academic Homepage

This is the source code for my academic homepage, built with Jekyll and hosted on GitHub Pages.

## Setup Instructions

### Prerequisites
- Git
- Ruby (version 2.7 or higher)
- Bundler

### Local Development

1. Clone this repository:
```bash
git clone https://github.com/your-username/your-username.github.io.git
cd your-username.github.io
```

2. Install dependencies:
```bash
bundle install
```

3. Run the local server:
```bash
bundle exec jekyll serve
```

4. Open your browser and navigate to `http://localhost:4000`

### Deploying to GitHub Pages

1. Create a new repository named `your-username.github.io` (replace `your-username` with your actual GitHub username)

2. Push this code to your repository:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/your-username/your-username.github.io.git
git push -u origin main
```

3. Go to your repository settings on GitHub
   - Navigate to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Select "main" branch and "/ (root)" folder
   - Click "Save"

4. Your site will be published at `https://your-username.github.io` within a few minutes

## Customization

### Update Personal Information

Edit `_config.yml` to update:
- Your name
- Email address
- GitHub username
- Other personal information

### Update Content

Edit `index.md` to update:
- About section
- Education details
- Professional experience
- Research projects
- Skills

### Add Your CV

Place your CV PDF file in the `assets` directory and name it `Yiran_CV.pdf` (or update the link in `index.md`)

### Styling

Customize the appearance by editing `assets/css/style.scss`

## Structure

```
.
├── _config.yml          # Site configuration
├── index.md             # Main homepage content
├── assets/
│   ├── css/
│   │   └── style.scss   # Custom styles
│   └── Yiran_CV.pdf     # Your CV (add this file)
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## License

This template is available for personal and academic use.
