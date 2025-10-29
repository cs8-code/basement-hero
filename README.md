# Static Website - Garagen & Keller Entrümpelung

This folder contains a pure HTML/CSS/JavaScript version of the website that can be used independently on any web server.

## Files

- `index.html` - Main HTML file with all content
- `styles.css` - All styling and animations
- `script.js` - Interactive functionality (smooth scroll, form handling, animations)

## Usage

### Option 1: Direct Upload
Simply upload these three files to any web hosting service:
- Traditional web hosting (via FTP)
- Netlify (drag & drop)
- GitHub Pages
- Vercel
- Any other static hosting service

### Option 2: Local Testing
Open `index.html` directly in your web browser to test locally.

## Important Notes

### Hero Image
The CSS references the hero image at `../../src/assets/hero-garage.jpg`. 

**To use this standalone:**
1. Copy the image from `src/assets/hero-garage.jpg` 
2. Place it in the same folder as your HTML file
3. Update line 56 in `styles.css` to:
   ```css
   background-image: url('hero-garage.jpg');
   ```

### Contact Form
The contact form currently only shows a success message but doesn't actually send emails. 

**To make it functional, you can:**
1. Use a form service like [Formspree](https://formspree.io/) or [Netlify Forms](https://www.netlify.com/products/forms/)
2. Add a backend API endpoint
3. Use mailto: action (not recommended for production)

**Example with Formspree:**
Change the form tag in `index.html` to:
```html
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Customization
- **Colors**: Edit CSS variables in `styles.css` (lines 15-23)
- **Content**: Edit text directly in `index.html`
- **Phone/Email**: Update in both HTML and the href attributes
- **Add Logo**: Replace "Entrümpelung Mülheim" text with an `<img>` tag

## Browser Support
Works in all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## No Build Process Required
These files work directly without any compilation or build steps. Just upload and go!
