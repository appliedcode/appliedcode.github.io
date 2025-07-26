# AI Training Hub Website

A comprehensive website for offering AI, Machine Learning, and Agentic AI courses and training programs. Built for deployment on GitHub Pages.

## 🚀 Features

- **Modern Design**: Clean, responsive design optimized for all devices
- **Course Catalog**: Comprehensive listing of AI training courses
- **Video Integration**: Embedded training videos and demos
- **Registration System**: Complete course registration functionality
- **Corporate Training**: Dedicated section for enterprise training programs
- **Student Testimonials**: Social proof from successful graduates
- **Mobile Responsive**: Perfect experience across all devices

## 📚 Course Offerings

1. **AI Fundamentals** (8 weeks) - Perfect for beginners
2. **Advanced Machine Learning** (10 weeks) - For intermediate learners
3. **Agentic AI Workflows** (12 weeks) - Advanced autonomous AI systems
4. **Natural Language Processing** (9 weeks) - LLMs and conversational AI
5. **Computer Vision** (10 weeks) - Image processing and recognition
6. **AI Ethics & Governance** (6 weeks) - Responsible AI development

## 🛠 Technical Stack

- **Frontend**: HTML5, CSS3, JavaScript
- **Styling**: Custom CSS with modern gradients and animations
- **Icons**: Font Awesome icons
- **Video**: YouTube/Vimeo integration ready
- **Forms**: Contact and registration forms
- **Deployment**: GitHub Pages compatible

## 📁 File Structure

```
/
├── index.html              # Main homepage
├── courses.html            # Course catalog page
├── register.html           # Course registration form
├── css/
│   ├── base.css           # Base styles
│   ├── vendor.css         # Third-party styles
│   ├── main.css           # Main theme styles
│   └── ai-training.css    # Custom AI training styles
├── js/
│   ├── main.js            # Main JavaScript
│   ├── plugins.js         # Plugin scripts
│   └── jquery-3.2.1.min.js
├── images/
│   ├── logo.svg           # Company logo
│   ├── hero-bg.jpg        # Hero background
│   └── ...                # Other images
└── fonts/                 # Custom fonts
```

## 🚀 Deployment on GitHub Pages

### Method 1: Direct Repository Deployment

1. **Fork or Clone** this repository
2. **Rename** the repository to `yourusername.github.io` (for user site) or keep any name (for project site)
3. **Go to Settings** → Pages
4. **Select Source**: Deploy from a branch
5. **Select Branch**: main/master
6. **Save** and wait for deployment

### Method 2: GitHub Actions (Recommended)

1. Create `.github/workflows/deploy.yml`:

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  deploy:
    runs-on: ubuntu-latest
    
    steps:
    - uses: actions/checkout@v3
    
    - name: Setup Node.js
      uses: actions/setup-node@v3
      with:
        node-version: '18'
    
    - name: Deploy to GitHub Pages
      uses: peaceiris/actions-gh-pages@v3
      if: github.ref == 'refs/heads/main'
      with:
        github_token: ${{ secrets.GITHUB_TOKEN }}
        publish_dir: ./
```

### Your Site Will Be Available At:
- User site: `https://yourusername.github.io`
- Project site: `https://yourusername.github.io/repository-name`

## 🎨 Customization Guide

### 1. Update Content
- Edit course descriptions in `index.html`
- Modify pricing in `courses.html`
- Update contact information throughout

### 2. Branding
- Replace `images/logo.svg` with your logo
- Update color scheme in `css/ai-training.css`
- Modify hero background image

### 3. Add Videos
- Replace YouTube embed URLs in video sections
- Add your training video content
- Update video descriptions

### 4. Forms Integration
Currently forms are client-side only. To make them functional:

**Option A: Netlify Forms**
```html
<form name="registration" method="POST" data-netlify="true">
```

**Option B: Formspree**
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option C: EmailJS**
Add EmailJS script and configuration for client-side email sending.

## 📱 Mobile Optimization

The site is fully responsive with:
- Mobile-first CSS approach
- Touch-friendly interface
- Optimized images and loading
- Responsive video embeds

## 🔧 Development Setup

1. Clone the repository
2. Open `index.html` in a browser
3. For live reload during development, use:
   ```bash
   npx live-server
   ```

## 📈 SEO Features

- Semantic HTML structure
- Meta tags for social sharing
- Fast loading times
- Mobile-friendly design
- Clean URL structure

## 🎯 Performance

- Optimized images
- Minified CSS/JS
- Fast loading animations
- Efficient font loading
- Optimized for Core Web Vitals

## 📞 Support

For questions about the website:
- Email: hello@appliedcode.in
- GitHub Issues: Create an issue in this repository

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

**Ready to launch your AI training business? Deploy this website and start accepting students today!** 🚀
