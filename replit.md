# Parth Panchal - Portfolio Website

## Overview

This is a personal portfolio website for Parth Panchal, a Senior Big Data Engineer. The application is built using Flask (Python) as the backend framework and serves a single-page portfolio website with modern frontend design. The website showcases professional experience, skills, projects, and contact information.

## System Architecture

### Frontend Architecture
- **Single Page Application (SPA)**: The website uses a single HTML template with JavaScript for smooth navigation and animations
- **Responsive Design**: Bootstrap 5.3.0 framework for responsive layout and components
- **Animation Library**: AOS (Animate On Scroll) for smooth scroll animations
- **Icon Library**: Font Awesome 6.4.0 for professional icons
- **Custom Styling**: CSS3 with custom variables for consistent theming

### Backend Architecture
- **Framework**: Flask (Python) - lightweight web framework
- **Template Engine**: Jinja2 (Flask's default templating engine)
- **Static File Serving**: Flask's built-in static file handling
- **File Download**: Direct file serving for resume downloads

## Key Components

### Backend Components
- **`app.py`**: Main Flask application with route definitions
- **`main.py`**: Application entry point for production deployment
- **Route Handlers**:
  - `/` - Serves the main portfolio page
  - `/download-resume` - Handles resume PDF downloads

### Frontend Components
- **`templates/index.html`**: Main HTML template containing the portfolio structure
- **`static/css/style.css`**: Custom styling with CSS variables and responsive design
- **`static/js/script.js`**: JavaScript for animations, smooth scrolling, and interactive features

### Design Features
- **Navigation**: Fixed navigation bar with smooth scrolling
- **Hero Section**: Eye-catching introduction with gradient backgrounds
- **Sections**: About, Skills, Experience, Projects, and Contact sections
- **Skill Bars**: Animated progress bars for technical skills
- **Responsive Design**: Mobile-first approach with Bootstrap grid system

## Data Flow

1. **Static Content Delivery**: All content is static and embedded in the HTML template
2. **Resume Download**: 
   - User clicks download button
   - Flask serves PDF file from `static/assets/resume.pdf`
   - File is downloaded as attachment
3. **Client-side Interactions**:
   - JavaScript handles smooth scrolling navigation
   - AOS library manages scroll-based animations
   - Intersection Observer API triggers skill bar animations

## External Dependencies

### Python Dependencies
- **Flask**: Web framework for serving the application
- **Standard Library**: `os` module for environment variables

### Frontend Dependencies (CDN)
- **Bootstrap 5.3.0**: CSS framework for responsive design
- **Font Awesome 6.4.0**: Icon library for professional icons
- **AOS 2.3.1**: Animation library for scroll effects

### Browser APIs
- **Intersection Observer API**: For triggering animations when elements come into view
- **Smooth Scroll API**: For enhanced navigation experience

## Deployment Strategy

### Environment Configuration
- **Development Mode**: Flask debug mode enabled for local development
- **Session Secret**: Configurable via environment variable `SESSION_SECRET`
- **Host Configuration**: Configured to run on `0.0.0.0:5000` for broad accessibility

### Static Assets
- **Resume File**: Expected to be placed in `static/assets/resume.pdf`
- **CSS/JS Files**: Served directly by Flask from the `static` directory
- **External Dependencies**: Loaded from CDNs for better performance

### Deployment Considerations
- Application is configured for containerized deployment (0.0.0.0 host)
- Environment variables used for configuration
- Debug mode should be disabled in production
- Static files can be served by web server (nginx/Apache) for better performance

## Changelog

```
Changelog:
- July 07, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```

## Technical Notes

### Architecture Decisions
- **Flask Choice**: Lightweight framework chosen for simplicity since this is a static portfolio site
- **Single Template**: All content in one HTML file for better SEO and simpler maintenance
- **CDN Dependencies**: External libraries loaded from CDNs to reduce bundle size and leverage browser caching
- **CSS Variables**: Used for consistent theming and easy customization
- **Progressive Enhancement**: JavaScript enhances the experience but the site works without it

### Performance Optimizations
- **AOS Library**: Configured with `once: true` to prevent repeated animations
- **Intersection Observer**: Used for efficient scroll-based animations
- **Smooth Scrolling**: Implemented via CSS `scroll-behavior` with JavaScript fallback
- **Responsive Images**: Bootstrap classes ensure proper image scaling

### Security Considerations
- **Session Secret**: Configurable environment variable for production security
- **File Downloads**: Direct file serving with proper headers for resume downloads
- **Static Content**: No user input processing reduces security attack surface