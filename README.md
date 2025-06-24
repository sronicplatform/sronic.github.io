# Sronic - Company Website

A modern, responsive static website for Sronic, showcasing the company's innovative technology solutions and applications.

## 🌟 Features

### Core Pages
- **Intro Page** (`index.html`) - Company introduction and overview
- **Apps Page** (`apps.html`) - Showcase of available applications with dropdown structure
- **About Page** (`about.html`) - Company story, mission, vision, and team information

### App-Specific Pages
Each app has its own dedicated section with:
- Individual app introduction pages
- Terms of Service pages
- Privacy Policy pages

### Design Features
- **Responsive Design** - Works perfectly on desktop, tablet, and mobile devices
- **Modern UI/UX** - Clean, professional design with smooth animations
- **Interactive Elements** - Hover effects, smooth scrolling, and mobile navigation
- **Accessibility** - Semantic HTML and keyboard navigation support

## 📁 File Structure

```
Sronic/
├── index.html                 # Homepage (Intro)
├── apps.html                  # Apps overview page
├── about.html                 # About company page
├── terms.html                 # Main Terms of Service
├── privacy.html               # Main Privacy Policy
├── styles.css                 # Main stylesheet
├── script.js                  # JavaScript functionality
├── README.md                  # This file
└── apps/                      # Apps directory
    ├── taskmaster/            # TaskMaster Pro app
    │   ├── terms.html         # App-specific Terms
    │   └── privacy.html       # App-specific Privacy Policy
    ├── dataviz/               # DataViz Analytics app
    ├── securechat/            # SecureChat app
    ├── cloudsync/             # CloudSync app
    ├── timetracker/           # TimeTracker app
    ├── codeflow/              # CodeFlow app
    └── taskmaster.html        # TaskMaster Pro intro page
```

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A local web server (optional, for development)

### Installation
1. Clone or download the project files
2. Open `index.html` in your web browser
3. Navigate through the website to explore all features

### Local Development Server (Optional)
For the best development experience, you can run a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## 🎨 Customization

### Colors and Branding
The website uses a modern color scheme that can be easily customized in `styles.css`:

```css
/* Primary Colors */
--primary-color: #2563eb;
--secondary-color: #fbbf24;
--accent-color: #667eea;

/* Background Colors */
--bg-primary: #ffffff;
--bg-secondary: #f8fafc;
--bg-dark: #1f2937;
```

### Adding New Apps
To add a new app to the website:

1. Create a new directory in the `apps/` folder
2. Add the app to the grid in `apps.html`
3. Create individual app pages (intro, terms, privacy)
4. Update navigation links as needed

### Content Updates
- Update company information in the respective HTML files
- Modify contact information in footer sections
- Update legal content in Terms and Privacy pages

## 📱 Responsive Design

The website is fully responsive and optimized for:
- **Desktop** (1200px+)
- **Tablet** (768px - 1199px)
- **Mobile** (320px - 767px)

## 🔧 Technical Details

### Technologies Used
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with Flexbox and Grid
- **JavaScript** - Interactive functionality
- **Font Awesome** - Icons
- **Google Fonts** - Typography (Inter font family)

### Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

### Performance Features
- Optimized images and assets
- Minified CSS and JavaScript (for production)
- Efficient loading with lazy loading support
- Smooth animations and transitions

## 📄 Legal Pages

### Main Legal Pages
- `terms.html` - General Terms of Service for the website
- `privacy.html` - General Privacy Policy for the website

### App-Specific Legal Pages
Each app has its own legal pages following the structure:
- `apps/[appname]/terms.html`
- `apps/[appname]/privacy.html`

## 🚀 Deployment

### Static Hosting
This website can be deployed to any static hosting service:

- **Netlify** - Drag and drop deployment
- **Vercel** - Git-based deployment
- **GitHub Pages** - Free hosting for public repositories
- **AWS S3** - Scalable static hosting
- **Firebase Hosting** - Google's hosting solution

### Custom Domain
Configure your custom domain in your hosting provider's settings and update any hardcoded URLs in the HTML files.

## 📞 Contact Information

Update the contact information in the following files:
- Footer sections in all HTML files
- Legal pages contact details
- About page company information

## 🔄 Future Enhancements

### Planned Features
- Contact Us page with form functionality
- Blog/News section
- User authentication system
- Multi-language support
- Advanced analytics integration
- Newsletter subscription
- Social media integration

### Adding Contact Page
When ready to add a contact page:
1. Create `contact.html`
2. Add contact form with validation
3. Update navigation in all pages
4. Add form handling backend (PHP, Node.js, etc.)

## 📝 License

This project is created for Sronic. All rights reserved.

## 🤝 Contributing

For internal development:
1. Create a feature branch
2. Make your changes
3. Test thoroughly across devices
4. Submit a pull request

## 📊 Analytics and SEO

### SEO Optimization
- Semantic HTML structure
- Meta tags and descriptions
- Open Graph tags for social sharing
- Structured data markup (can be added)

### Analytics Integration
Add your analytics code to the `<head>` section of HTML files:
- Google Analytics
- Google Tag Manager
- Facebook Pixel
- Other tracking tools

---

**Built with ❤️ for Sronic**

For questions or support, contact the development team. 