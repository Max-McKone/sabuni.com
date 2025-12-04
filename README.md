# Michael Sabuni Photography Portfolio

A minimal, image-focused photography portfolio website built with pure HTML and CSS.

## Project Structure

```
sabuni.com/
├── index.html          # Homepage with photo gallery
├── about.html          # About page with bio and contact info
├── css/
│   └── style.css       # All styles in one file
├── images/             # Place all photos here
│   ├── placeholder-1.jpg
│   ├── placeholder-2.jpg
│   └── portrait.jpg    # About page portrait
└── README.md
```

## Getting Started

1. **Add your images** to the `images/` folder
2. **Update image paths** in `index.html` and `about.html`
3. **Update the Shopify link** - replace `https://your-shopify-store.myshopify.com` with your actual shop URL
4. **Customize content** - update bio, contact info, and social links

## Customization

### Adding Photos to Gallery

In `index.html`, add gallery items using this template:

```html
<figure class="gallery-item">
    <img src="images/your-photo.jpg" alt="Description of photo" loading="lazy">
    <figcaption>Series Title, Year</figcaption>
</figure>
```

**Gallery item modifiers:**
- `gallery-item--wide` - spans 2 columns (for landscape/panoramic shots)
- `gallery-item--tall` - spans 2 rows (for portrait shots)

### Changing Colors

Edit the CSS custom properties in `css/style.css`:

```css
:root {
    --color-bg: #faf9f7;        /* Background */
    --color-text: #1a1a1a;       /* Main text */
    --color-accent: #8b7355;     /* Accent (shop link) */
}
```

### Changing Fonts

The site uses:
- **Cormorant Garamond** - for headings (elegant, editorial)
- **Instrument Sans** - for body text (clean, modern)

To change fonts, update the Google Fonts link in both HTML files and the CSS variables.

## Local Development

Simply open `index.html` in your browser. No build tools required!

For live reloading during development, you can use:
```bash
# Using Python
python -m http.server 8000

# Using Node.js (if you have it)
npx serve
```

## Deployment

This is a static site - deploy anywhere:
- **Netlify** - drag and drop the folder
- **Vercel** - connect your GitHub repo
- **GitHub Pages** - push to a `gh-pages` branch
- **Any web host** - upload via FTP

## Browser Support

Modern browsers (Chrome, Firefox, Safari, Edge). Uses:
- CSS Grid
- CSS Custom Properties
- Backdrop Filter (graceful fallback)

---

© 2024 Michael Sabuni


