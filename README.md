# Cafe Bar - Independent HTML Website

A standalone HTML version of the Cafe Bar website, completely independent of any framework or build system.

## Features

- 🌐 Pure HTML/CSS/JavaScript - no build tools required
- 📱 Fully responsive design using Tailwind CSS (CDN)
- ☕ Complete coffee shop website with all pages
- 🖼️ Image gallery with lightbox functionality
- 📝 Working contact form with validation
- 🎨 Modern design with animations and transitions
- ♿ Accessible markup and semantic HTML5

## Pages

- **Home** (`index.html`) - Hero section, features, call-to-action
- **Menu** (`menu.html`) - Interactive menu with filtering by category
- **About** (`about.html`) - Our story, team information
- **Gallery** (`gallery.html`) - Photo gallery with lightbox
- **Contact** (`contact.html`) - Contact form and location info

## Getting Started

### Local Development

1. Clone or download the files
2. Navigate to the project directory
3. Start a local server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Or open index.html directly in your browser
```

4. Open `http://localhost:8000` in your browser

### Deployment

Since this is a static website, you can deploy it to any static hosting service:

- Netlify (drag and drop the folder)
- Vercel (drag and drop the folder)
- GitHub Pages
- Any traditional web server

## File Structure

```
cofee/
├── index.html          # Homepage
├── menu.html           # Menu page
├── about.html          # About page
├── gallery.html        # Gallery page
├── contact.html        # Contact page
├── public/             # Assets folder
│   ├── favicon.svg
│   ├── logo.svg
│   ├── logo-horizontal.svg
│   ├── logo-icon.svg
│   └── images/         # All website images
│       ├── hero/
│       ├── menu/
│       ├── gallery/
│       ├── about/
│       └── ...
└── README.md           # This file
```

## Customization

### Colors
The site uses an amber/orange color scheme. To change colors, modify the CSS variables or Tailwind classes:

- Primary: `amber-600` (rgb(217 119 6))
- Secondary: `amber-700` (rgb(180 83 9))

### Content
All content is hardcoded in the HTML files. To update:
- Edit text directly in the respective HTML files
- Update images by replacing files in the `public/images/` folder
- Modify contact information in the contact page

### Adding New Menu Items
Edit the `menuItems` array in `menu.html`:

```javascript
{
  id: 13,
  name: 'New Item',
  description: 'Description of the new item',
  price: 4.50,
  category: 'coffee',
  available: true,
  image: '/public/images/menu/new-item.jpg'
}
```

## Browser Support

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS framework (CDN)
- **Vanilla JavaScript** - Interactive functionality
- **SVG Icons** - Scalable graphics

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

For questions or support:
- Email: hello@cafebar.com
- Phone: (555) 123-4567