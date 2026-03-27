# Omar's Learning Center

Interactive study tool for 3rd grade at Cedar Hill Prep.

## Deploy to GitHub Pages

### Option 1: New repo (recommended)
```bash
# Create repo
gh repo create omars-learning-center --public
git clone https://github.com/YOUR_USERNAME/omars-learning-center.git
cd omars-learning-center

# Add the file
cp ~/Downloads/index.html .
git add index.html
git commit -m "Omar's Learning Center v1"
git push origin main

# Enable GitHub Pages
gh api repos/YOUR_USERNAME/omars-learning-center/pages -X POST -f source.branch=main -f source.path=/
```

### Option 2: Quick terminal one-liner
```bash
cd omars-learning-center && cp ~/Downloads/index.html . && git add -A && git commit -m "update learning center" && git push
```

## Add to Omar's iPad
1. Open Safari on the iPad
2. Go to: `https://YOUR_USERNAME.github.io/omars-learning-center/`
3. Tap Share → Add to Home Screen
4. Name it "Learning Center"

It will appear as an app icon on his home screen.

## How to update content
1. Send study guide photo to Claude
2. Claude updates the code
3. Download new `index.html`
4. Push to GitHub (one-liner above)
