# Basic Personal Portfolio

A clean, minimalist single-page portfolio website built with pure HTML and CSS. Perfect for students, freelancers, and job seekers who want a professional online presence without the complexity of frameworks or build tools.

## ✨ Features

- **Modern & Responsive Design**: Looks great on all devices (mobile, tablet, desktop)
- **Single-Page Layout**: Smooth scrolling navigation between sections
- **Clean Sections**:
  - Hero/Header with name, tagline, and call-to-action
  - About section with profile image and personal details
  - Skills showcase with progress bars and icons
  - Portfolio with 3 project cards
  - Contact section with email and social links
  - Footer with copyright and back-to-top link
- **Accessible**: Semantic HTML, ARIA labels, keyboard navigation, focus styles
- **SEO Optimized**: Meta tags, Open Graph support, proper heading hierarchy
- **No Dependencies**: Pure HTML/CSS, no JavaScript frameworks or build steps
- **GitHub Pages Ready**: Deploy instantly without configuration

## 📁 Folder Structure

```
basic-personal-portfolio/
├── index.html          # Main HTML file with all sections
├── style.css           # Complete stylesheet with CSS variables
├── assets/             # Images and icons folder
│   ├── profile.jpg     # Profile photo placeholder
│   ├── project-1.jpg   # Project screenshot placeholder
│   ├── project-2.jpg   # Project screenshot placeholder
│   ├── project-3.jpg   # Project screenshot placeholder
│   ├── og-image.jpg    # Open Graph image for social sharing
│   ├── favicon.png     # Website favicon
│   ├── html-icon.svg   # HTML5 skill icon
│   ├── css-icon.svg    # CSS3 skill icon
│   ├── js-icon.svg     # JavaScript skill icon
│   ├── react-icon.svg  # React skill icon
│   ├── nodejs-icon.svg # Node.js skill icon
│   └── git-icon.svg    # Git skill icon
├── README.md           # This file
└── LICENSE             # MIT License

```

## 🎨 Customization Guide

### Update Personal Information

1. **Open `index.html`** and replace placeholder text:
   - Line 10: Update `<meta name="author">` with your name
   - Line 14-16: Update Open Graph meta tags
   - Line 18: Update page title
   - Line 33: Replace "Your Name" in nav brand
   - Line 48: Replace hero name and tagline
   - Lines 67-92: Update About section with your bio and details
   - Lines 207-210: Update contact email
   - Line 212-231: Update social media links
   - Line 241: Update footer copyright name

2. **Update `style.css`** to change colors and fonts:
   ```css
   /* Around line 8-16, modify color variables */
   --color-primary: #6366f1;        /* Main accent color */
   --color-primary-dark: #4f46e5;   /* Darker shade for hovers */
   --color-text: #1f2937;           /* Main text color */
   --color-background: #ffffff;      /* Background color */
   
   /* Around line 28, change font family */
   --font-family: 'Poppins', sans-serif;  /* Replace with your preferred font */
   ```

3. **Replace Images** in the `assets/` folder:
   - `profile.jpg`: Your professional photo (400x400px recommended)
   - `project-1.jpg`, `project-2.jpg`, `project-3.jpg`: Your project screenshots (800x600px)
   - `og-image.jpg`: Social sharing image (1200x630px)
   - `favicon.png`: Your custom favicon (32x32px)

### Customize Skills

In `index.html` (lines 96-168), modify the skills section:
- Replace skill names and icons
- Adjust progress bar widths (style="width: XX%")
- Add or remove skill items by copying the `.skill-item` div structure

### Update Portfolio Projects

In `index.html` (lines 176-224):
- Replace project images, titles, and descriptions
- Update project links (replace `#` with actual URLs)
- Add more projects by duplicating `.project-card` article elements

### Change Color Scheme

Edit CSS variables in `style.css` (lines 8-16):
```css
/* Blue/Purple theme (default) */
--color-primary: #6366f1;

/* Alternative themes */
/* Green theme: #10b981 */
/* Orange theme: #f97316 */
/* Pink theme: #ec4899 */
/* Teal theme: #14b8a6 */
```

### Change Fonts

1. Replace Google Fonts link in `index.html` (line 26)
2. Update `--font-family` in `style.css` (line 28)

Popular alternatives:
- `Roboto` - Modern and clean
- `Inter` - Excellent for UI
- `Montserrat` - Bold and striking
- `Open Sans` - Highly readable

## 🚀 Deployment to GitHub Pages

### Option 1: GitHub Web Interface

1. Create a new repository on GitHub
2. Upload all files (index.html, style.css, assets folder)
3. Go to repository Settings → Pages
4. Under "Source", select `main` branch and `/ (root)` folder
5. Click "Save"
6. Your site will be live at `https://yourusername.github.io/repository-name/`

### Option 2: Git Command Line

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit: Personal portfolio website"

# Add remote repository (replace with your repo URL)
git remote add origin https://github.com/yourusername/your-repo.git

# Push to GitHub
git push -u origin main

# Enable GitHub Pages
# Go to repository Settings → Pages → Select main branch → Save
```

### Custom Domain (Optional)

1. In repository Settings → Pages → Custom domain
2. Enter your domain name (e.g., `www.yourname.com`)
3. Configure DNS with your domain provider:
   - Add CNAME record pointing to `yourusername.github.io`

## 🛠️ Testing & Validation

### HTML Validation
Visit [W3C HTML Validator](https://validator.w3.org/) and paste your site URL

### CSS Validation
Visit [W3C CSS Validator](https://jigsaw.w3.org/css-validator/) and paste your site URL

### Accessibility Check
- Use [WAVE Web Accessibility Tool](https://wave.webaim.org/)
- Test keyboard navigation (Tab, Enter, Shift+Tab)
- Verify screen reader compatibility

### Responsive Testing
Test on different devices or use browser DevTools:
- Mobile: 375px, 414px
- Tablet: 768px, 1024px
- Desktop: 1280px, 1920px

### Browser Compatibility
Test on:
- Chrome/Edge (Chromium)
- Firefox
- Safari
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 Design System

### Spacing Scale (8px base)
```
--space-xs: 8px
--space-sm: 16px
--space-md: 24px
--space-lg: 32px
--space-xl: 48px
--space-2xl: 64px
--space-3xl: 96px
```

### Typography Scale
```
--font-size-xs: 0.875rem (14px)
--font-size-sm: 1rem (16px)
--font-size-md: 1.125rem (18px)
--font-size-lg: 1.5rem (24px)
--font-size-xl: 2rem (32px)
--font-size-2xl: 2.5rem (40px)
--font-size-3xl: 3rem (48px)
```

### Color Variables
All colors are defined as CSS variables in `:root` for easy customization.

## 🎯 Tips for Success

### Content Writing
- Keep bio concise (2-3 short paragraphs)
- Use action verbs in project descriptions
- Highlight measurable achievements
- Keep skill list focused (6-8 core skills)

### Images
- Use high-quality, professional photos
- Optimize images before upload (use tools like TinyPNG)
- Maintain consistent aspect ratios
- Use descriptive filenames

### SEO Best Practices
- Update meta description with your unique value proposition
- Use descriptive alt text for all images
- Create meaningful page title
- Add Open Graph image for social sharing

### Performance
- All images are already optimized
- CSS uses modern features (Grid, Flexbox)
- No external dependencies (except Google Fonts)
- Minimal CSS with efficient selectors

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Free to use for personal and commercial projects with attribution.

## 🙏 Credits

Created by [Hidden-Sect](https://github.com/Hidden-Sect) as part of the "Basic Package" - affordable, professional website templates.

## 📧 Support

For questions or issues:
- Open an issue on GitHub
- Check existing documentation
- Review the customization guide above

---

**Made with ❤️ by Hidden-Sect** | [More Templates](https://github.com/Hidden-Sect)
