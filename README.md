# Parth Panchal - Portfolio Website

A professional portfolio website for Parth Panchal, a Senior Big Data Engineer with 4.5+ years of experience in AWS, Spark, and data engineering solutions.

## Features

- **Responsive Design**: Built with Bootstrap 5.3.0 for mobile-first responsive layout
- **Interactive Animations**: AOS (Animate On Scroll) library for smooth scroll animations
- **Professional Sections**: Hero, About, Skills, Experience, Projects, and Contact sections
- **Skill Progress Bars**: Animated progress bars showing technical expertise
- **Timeline Layout**: Professional experience displayed in an attractive timeline format
- **Modern UI/UX**: Clean, professional design with gradient backgrounds and hover effects

## Technologies Used

### Backend
- **Flask** - Python web framework
- **Python 3.11** - Programming language
- **Gunicorn** - WSGI HTTP Server

### Frontend
- **HTML5** - Markup language
- **CSS3** - Styling with custom variables and animations
- **Bootstrap 5.3.0** - CSS framework for responsive design
- **JavaScript** - Interactive functionality
- **AOS Library** - Animate On Scroll effects
- **Font Awesome** - Professional icons

## Installation & Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd parth_portfolio_website
   ```

2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
   Or if using uv:
   ```bash
   uv sync
   ```

3. **Set environment variables**
   ```bash
   export SESSION_SECRET="your-secret-key-here"
   ```

4. **Run the application**
   ```bash
   python app.py
   ```
   
   Or using Gunicorn:
   ```bash
   gunicorn --bind 0.0.0.0:5000 --reuse-port --reload main:app
   ```

5. **Access the website**
   Open your browser and navigate to `http://localhost:5000`

## Project Structure

```
parth_portfolio_website/
├── app.py                 # Main Flask application
├── main.py               # Application entry point
├── pyproject.toml        # Python dependencies
├── uv.lock              # Dependency lock file
├── replit.md            # Project documentation
├── templates/
│   └── index.html       # Main HTML template
├── static/
│   ├── css/
│   │   └── style.css    # Custom CSS styles
│   ├── js/
│   │   └── script.js    # JavaScript functionality
│   └── assets/
│       └── resume.pdf   # Downloadable resume
└── README.md            # This file
```

## Features Breakdown

### Hero Section
- Professional introduction with animated elements
- Call-to-action buttons for navigation and resume download
- Responsive profile image with floating animation

### About Section
- Career highlights and professional summary
- Statistics counter animation
- Professional imagery

### Skills Section
- Technical skills organized by categories
- Animated progress bars showing proficiency levels
- Intersection Observer for smooth animations

### Experience Timeline
- Chronological work history
- Detailed job descriptions and achievements
- Responsive timeline layout

### Projects Showcase
- Key project accomplishments
- Technology stack highlights
- Interactive hover effects

### Contact Information
- Professional contact details
- Social media links
- Interactive contact cards

## Customization

### Updating Content
1. Edit `templates/index.html` to modify the content
2. Update `static/css/style.css` for styling changes
3. Modify `static/js/script.js` for functionality updates

### Adding New Sections
1. Add HTML structure in `templates/index.html`
2. Add corresponding CSS styles in `static/css/style.css`
3. Add JavaScript functionality if needed in `static/js/script.js`

### Replacing Resume
Replace `static/assets/resume.pdf` with your updated resume file.

## Performance Optimizations

- **AOS Library**: Configured with `once: true` to prevent repeated animations
- **Intersection Observer**: Used for efficient scroll-based animations
- **Smooth Scrolling**: Implemented via CSS `scroll-behavior` with JavaScript fallback
- **Responsive Images**: Bootstrap classes ensure proper image scaling
- **CDN Dependencies**: External libraries loaded from CDNs for better performance

## Browser Compatibility

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile responsive design
- Progressive enhancement approach

## Deployment

This application is ready for deployment on:
- **Replit**: Already configured with `.replit` file
- **Heroku**: Add `Procfile` with `web: gunicorn main:app`
- **Railway**: Configure with `railway.toml`
- **Vercel**: Add `vercel.json` configuration

## Contact

**Parth Panchal**
- Email: parthpanchal1098@gmail.com
- LinkedIn: [https://www.linkedin.com/in/parth-panchal-b431a1197/](https://www.linkedin.com/in/parth-panchal-b431a1197/)
- Blog: [https://awspcube.blogspot.com/](https://awspcube.blogspot.com/)
- Location: Kavisha Amara, Shela, Ahmedabad 380058
- Phone: +91 98247 31421

---

*This portfolio website showcases 4.5+ years of experience in Big Data Engineering, AWS services, and modern web development practices.*