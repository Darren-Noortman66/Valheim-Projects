# Valheim Projects Website

A premium, modern website template for Gerhard Noortman's high-end steel and wood craftsmanship business. This website is designed to showcase luxury projects and appeal to discerning clients.

## Features

### 🎨 Design Elements
- **Elegant Typography**: Uses Playfair Display (serif) for headings and Inter (sans-serif) for body text
- **Premium Color Scheme**: Black, white, and metallic gold (#D4AF37) inspired by the Valheim logo
- **Subtle Valheim Elements**: Viking helmet icon and metallic accents without being overly thematic
- **Modern Layout**: Clean, spacious design with excellent visual hierarchy

### 📱 Responsive Design
- Fully responsive across all devices
- Mobile-first approach with hamburger navigation
- Optimized for desktop, tablet, and mobile viewing

### ⚡ Interactive Features
- Smooth scrolling navigation
- Portfolio filtering system
- Contact form with validation
- Animated counters for statistics
- Parallax effects
- Loading animations
- Scroll progress indicator

### 🏗️ Sections
1. **Hero Section**: Eye-catching introduction with call-to-action buttons
2. **About Section**: Gerhard's story with impressive statistics
3. **Services Section**: Six key service offerings with icons
4. **Portfolio Section**: Filterable project showcase
5. **Contact Section**: Contact information and inquiry form
6. **Footer**: Logo, links, and social media

## File Structure

```
valheim-projects-website/
├── index.html          # Main HTML structure
├── styles.css          # All CSS styling
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Customization Guide

### 🎨 Colors
The website uses a sophisticated color palette:
- **Primary Gold**: `#D4AF37` (metallic gold from logo)
- **Secondary Gold**: `#B8860B` (darker gold for gradients)
- **Black**: `#000` (for backgrounds and text)
- **White**: `#fff` (for contrast)
- **Gray**: `#666`, `#ccc` (for secondary text)

### 📝 Content Updates

#### Logo
The logo uses Font Awesome's `fa-helmet-battle` icon. You can:
- Replace with your actual logo image
- Change the icon to a different Font Awesome icon
- Use a custom SVG or image

#### Contact Information
Update in `index.html`:
```html
<!-- Phone -->
<p>+1 (555) 123-4567</p>

<!-- Email -->
<p>gerhard@valheimprojects.com</p>

<!-- Address -->
<p>123 Craftsmanship Lane<br>Artisan District, CA 90210</p>
```

#### Services
Modify the services in the services section:
```html
<div class="service-card">
    <div class="service-icon">
        <i class="fas fa-sculpture"></i>
    </div>
    <h3>Custom Sculptures</h3>
    <p>Your service description here...</p>
</div>
```

#### Portfolio Items
Add new portfolio items:
```html
<div class="portfolio-item" data-category="sculptures">
    <div class="portfolio-placeholder">
        <i class="fas fa-sculpture"></i>
        <span>Project Name</span>
    </div>
    <div class="portfolio-overlay">
        <h3>Project Title</h3>
        <p>Project description</p>
    </div>
</div>
```

### 🖼️ Adding Images

#### Hero Image
Replace the placeholder in the hero section:
```html
<div class="hero-visual">
    <img src="path/to/your/hero-image.jpg" alt="Valheim Projects Hero" class="hero-image">
</div>
```

#### About Image
Replace the about placeholder:
```html
<div class="about-image">
    <img src="path/to/gerhard-portrait.jpg" alt="Gerhard Noortman" class="about-image">
</div>
```

#### Portfolio Images
Replace portfolio placeholders:
```html
<div class="portfolio-item" data-category="sculptures">
    <img src="path/to/project-image.jpg" alt="Project Name" class="portfolio-image">
    <div class="portfolio-overlay">
        <h3>Project Title</h3>
        <p>Project description</p>
    </div>
</div>
```

### 📧 Form Handling
The contact form currently shows a success message. To make it functional:

1. **Email Service**: Use services like Formspree, Netlify Forms, or your own backend
2. **Update the form action**:
```html
<form id="contactForm" action="https://formspree.io/your-email@domain.com" method="POST">
```

3. **Or use JavaScript to send to your server**:
```javascript
// In script.js, replace the form submission with:
fetch('/api/contact', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
});
```

### 🔧 Advanced Customization

#### Fonts
Change fonts in `styles.css`:
```css
/* Update Google Fonts import in index.html */
<link href="https://fonts.googleapis.com/css2?family=Your+Font:wght@400;600;700&display=swap" rel="stylesheet">

/* Update font-family in CSS */
body { font-family: 'Your Font', sans-serif; }
```

#### Animations
Modify animation speeds in `script.js`:
```javascript
// Typing speed
typeWriter(heroTitle, originalText, 80); // 80ms per character

// Counter animation duration
animateCounter(stat, target, 2000); // 2000ms = 2 seconds
```

#### Portfolio Categories
Add new categories by:
1. Adding filter buttons in HTML
2. Adding `data-category` attributes to portfolio items
3. The JavaScript will automatically handle the filtering

## Browser Compatibility
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Features
- Optimized CSS with efficient selectors
- Minimal JavaScript for fast loading
- Responsive images (when added)
- Smooth animations with hardware acceleration

## SEO Considerations
- Semantic HTML structure
- Meta descriptions and titles
- Proper heading hierarchy
- Alt text for images (when added)
- Fast loading times

## Deployment
1. Upload all files to your web hosting
2. Ensure all files are in the same directory
3. Test the contact form functionality
4. Add your actual images and content
5. Update meta tags for SEO

## Support
For customization help or questions about the template, refer to the code comments or modify the relevant sections as outlined above.

---

**Note**: This template is designed to be a starting point. Replace placeholder content with actual project images, Gerhard's real information, and customize the styling to match your exact brand requirements. 