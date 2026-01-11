# Brighter Realities Website

Minimal Jekyll site for GitHub Pages.

## Setup

### 1. Download Fraunces font

Download the Fraunces variable font files from [Google Fonts](https://fonts.google.com/specimen/Fraunces):

1. Go to https://fonts.google.com/specimen/Fraunces
2. Click "Download family"
3. Extract and copy these files to `assets/fonts/`:
   - `Fraunces-VariableFont_SOFT,WONK,opsz,wght.ttf` → rename to `Fraunces-Variable.ttf`
   - `Fraunces-Italic-VariableFont_SOFT,WONK,opsz,wght.ttf` → rename to `Fraunces-Italic-Variable.ttf`

### 2. Update App Store link

In `index.md`, replace the `#` placeholder in the Wristrax App Store link with your actual App Store URL.

### 3. Deploy to GitHub Pages

1. Create a new repo on GitHub
2. Push this code
3. Go to Settings → Pages → Source: Deploy from branch (main)
4. Add your custom domain in Settings → Pages → Custom domain

### 4. DNS setup

Point your domain to GitHub Pages:
- A record: `185.199.108.153`
- A record: `185.199.109.153`
- A record: `185.199.110.153`
- A record: `185.199.111.153`

Or use a CNAME if using a subdomain.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Then visit http://localhost:4000

## Structure

```
├── _config.yml          # Jekyll config
├── _layouts/
│   └── default.html     # Main template
├── assets/
│   ├── css/
│   │   └── style.css    # All styles
│   └── fonts/           # Self-hosted fonts (add manually)
├── index.md             # Homepage content
└── README.md
```

## Editing content

All content is in `index.md`. Just edit the markdown/HTML there.
