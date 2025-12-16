# Desheng Hu - Personal Website

Personal website for my research and professional profile.

## Sections

- Education
- Work Experience
- Publications
- Skills
- Awards & Honors
- Contact Information

## Technologies

- HTML/CSS/JavaScript
- Google Fonts (Inter)

## Setup Instructions

### 1. Create GitHub Repository

Since you want to host this on GitHub Pages, you need to create a repository named `whocheers.github.io` (or `USERNAME.github.io` format for your GitHub username).

**Option A: Using GitHub Website**
1. Go to [https://github.com/new](https://github.com/new)
2. Repository name: `whocheers.github.io` (or your-username.github.io)
3. Make it Public
4. Don't initialize with README (we already have files)
5. Click "Create repository"

**Option B: Using GitHub CLI (if you install it)**
```bash
gh repo create whocheers.github.io --public --source=. --remote=origin --push
```

### 2. Push Your Code to GitHub

After creating the repository on GitHub, run these commands from the project directory:

```bash
cd /Users/deshenghu/Desktop/PhD_thesis_related/job_seeking_related/personal_website

# Add the remote repository (replace whocheers with your username if different)
git remote add origin https://github.com/whocheers/whocheers.github.io.git

# Push the code to GitHub
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/whocheers/whocheers.github.io`
2. Click on "Settings" tab
3. Scroll down to "Pages" section in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Your website will be live at: `https://whocheers.github.io`

**Note:** It may take a few minutes for the site to become available after enabling GitHub Pages.

### 4. Update Google Scholar Link

Before pushing to GitHub, you should update the Google Scholar link in `index.html`:

1. Find `YOUR_ID` in the HTML file (appears twice)
2. Replace it with your actual Google Scholar user ID from your profile URL
3. Commit and push the change:
   ```bash
   git add index.html
   git commit -m "Update Google Scholar link"
   git push
   ```

## Customization

### Updating Content

- **Personal Information**: Edit `index.html` sections
- **Styling**: Modify `styles.css` for colors, fonts, spacing
- **Interactions**: Update `script.js` for behavior changes

### Color Scheme

To change colors, edit the CSS variables in `styles.css`:
```css
:root {
    --primary-color: #2563eb;
    --secondary-color: #1e40af;
    --accent-color: #3b82f6;
    /* ... other colors */
}
```

## File Structure

```
personal_website/
├── index.html      # Main HTML file
├── styles.css      # CSS styling
├── script.js       # JavaScript functionality
└── README.md       # This file
```

## Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Local Development

To test locally, simply open `index.html` in your browser. For a better development experience with live reload:

```bash
# Using Python's built-in server
python3 -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## Maintenance

### Adding New Publications

Edit the `publications` section in `index.html`:

```html
<div class="publication-item">
    <h4>Your Paper Title</h4>
    <p class="authors"><strong>Your Name</strong>, et al.</p>
    <p class="venue">Conference Name YEAR</p>
</div>
```

### Adding New Skills

Add tags to the relevant skill category in `index.html`:

```html
<span class="tag">New Skill</span>
```

## License

Copyright © 2025 Desheng Hu. All rights reserved.

## Contact

- Email: hudeshengnpu@gmail.com
- Phone: (+41) 767115225
- Location: University of Zurich, Switzerland
