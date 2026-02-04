# Anujan Ithayarajan - Portfolio Website

A modern, tech-focused portfolio website for an Electronics and Embedded Systems Engineer. Built with HTML5, CSS3, and vanilla JavaScript.

## Features

✨ **Modern Design**
- Dark theme with blue (#00d4ff) and purple (#7c3aed) accent colors
- Responsive and mobile-friendly layout
- Smooth animations and transitions
- Professional typography and spacing

🎯 **Key Sections**
- **Home/Hero**: Eye-catching introduction with profile image and CTA buttons
- **About**: Personal bio, education, and core competencies with skill bars
- **Experience**: Timeline view of work experience
- **Projects**: Showcase of featured engineering projects with descriptions and technologies
- **Services**: Highlight offered services and expertise areas
- **Technical Skills**: Categorized skills and tools
- **Contact**: Contact information and message form
- **Footer**: Quick links and social profiles

⚡ **Functionality**
- Smooth scrolling navigation
- Mobile hamburger menu
- Active navigation link highlighting on scroll
- Responsive contact form with email integration
- Interactive animations on scroll
- Hover effects on cards and buttons
- Skill bar animations
- Social media integration

📱 **Responsive Design**
- Desktop optimized
- Tablet friendly
- Mobile responsive (480px+)
- Touch-friendly navigation

## File Structure

```
Portfolio/
├── index.html          # Main HTML file
├── styles.css          # Complete styling and animations
├── script.js           # JavaScript functionality and interactions
└── README.md           # This file
```

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No server or dependencies required

### Installation

1. **Clone or download the portfolio files**
   ```bash
   git clone <repository-url>
   cd Portfolio
   ```

2. **Open in browser**
   - Simply open `index.html` in your web browser
   - Or use a local development server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

3. **Access the website**
   - Open http://localhost:8000 in your browser

## Customization

### Update Personal Information

#### In `index.html`:
1. **Name and Title**
   - Update the hero section title and subtitle
   - Update navbar brand name

2. **Contact Information**
   - Update email address (search for `anujaithayarajan@gmail.com`)
   - Update phone number (search for `+94754918695`)
   - Update LinkedIn profile URL
   - Update GitHub profile URL

3. **About Section**
   - Modify personal bio and background
   - Update education details and graduation year
   - Adjust core competencies and skill names

4. **Experience**
   - Update work experience entries
   - Modify internship dates and descriptions
   - Update company names and locations

5. **Projects**
   - Edit project titles and descriptions
   - Update technologies and tech tags
   - Modify project features and GitHub links

6. **Services**
   - Customize service offerings
   - Modify service descriptions
   - Update service features

7. **Skills**
   - Update skill categories
   - Add or remove skills
   - Modify skill proficiency percentages

#### Profile Picture
Replace the placeholder image URL in the hero section:
```html
<img src="https://via.placeholder.com/300?text=Anujan" alt="Anujan Ithayarajan">
```
Change to your actual image URL:
```html
<img src="path/to/your/image.jpg" alt="Anujan Ithayarajan">
```

### Customize Colors

In `styles.css`, modify the CSS variables in the `:root` selector:
```css
:root {
    --primary-color: #00d4ff;      /* Cyan/Blue */
    --secondary-color: #7c3aed;    /* Purple */
    --accent-color: #a855f7;       /* Light Purple */
    --dark-bg: #0a0e27;            /* Very Dark Blue */
    --darker-bg: #050810;          /* Even Darker */
    --card-bg: #1a1f3a;            /* Card Background */
    --text-primary: #e0e6ff;       /* Light Text */
    --text-secondary: #a0aec0;     /* Secondary Text */
    --border-color: #2d3748;       /* Border Color */
    --success-color: #10b981;      /* Success Color */
}
```

### Adjust Layout

- **Container width**: Change `max-width` in `.container` (default: 1200px)
- **Section padding**: Modify `padding` in `section` CSS rule
- **Grid columns**: Update `grid-template-columns` values for different responsive breakpoints

### Modify Animations

All animations are defined at the bottom of `styles.css`. Key animations:
- `slideInLeft`, `slideInRight`, `slideInUp` - Entrance animations
- `float` - Floating background shapes
- `fillProgress` - Skill bar fills

## Contact Form Setup

The contact form currently uses `mailto:` links. For production deployment, you have several options:

### Option 1: Email Service (Recommended)
Use a service like:
- [Formspree](https://formspree.io/)
- [Basin](https://www.basinapp.com/)
- [Web3Forms](https://web3forms.com/)

### Option 2: Backend Integration
Set up a backend service to handle form submissions (Node.js, Python Flask, etc.)

### Option 3: Static Hosting
Use services like:
- [Netlify Forms](https://www.netlify.com/products/forms/)
- [Vercel](https://vercel.com/)

## Deployment Options

### Static Hosting (Recommended)
- **Netlify**: Drag and drop deployment
- **Vercel**: Git-based deployment
- **GitHub Pages**: Free hosting for GitHub users
- **Surge**: Simple static hosting

### Traditional Hosting
- Upload all files to your web hosting provider via FTP
- Ensure all files are in the root directory

### Steps for GitHub Pages
1. Create a GitHub repository
2. Push files to the repository
3. Go to Settings > Pages
4. Select main branch as source
5. Your site will be live at `username.github.io/portfolio`

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Optimization

- Uses vanilla JavaScript (no external dependencies)
- CSS is minified and optimized
- Images use placeholder service (replace with optimized images for production)
- Lazy loading ready (can be added for images)

## Accessibility

- Semantic HTML5 structure
- Proper heading hierarchy
- Alt text for images
- Keyboard navigation support
- Color contrast meeting WCAG standards

## SEO Optimization

- Proper meta tags in HTML head
- Semantic HTML structure
- Clean URLs with anchor navigation
- Mobile-responsive design
- Fast loading times

## Troubleshooting

### Mobile menu not closing
- Check if JavaScript is enabled
- Verify `script.js` is loaded correctly

### Animations not working
- Ensure CSS is fully loaded
- Check browser support for CSS animations
- Verify no CSS conflicts

### Contact form not working
- Check if email client is installed
- Verify email links are correctly formatted

### Images not showing
- Update image paths to correct URLs
- Ensure images are accessible

## Future Enhancements

- Add blog section
- Integrate real contact form backend
- Add project showcase with modal details
- Add dark/light theme toggle
- Add multi-language support
- Add resume/CV download
- Add testimonials section
- Add newsletter subscription
- Add search functionality

## Credits

- Font Awesome Icons: https://fontawesome.com/
- Google Fonts for typography
- Custom CSS animations and effects

## License

This portfolio template is free to use and modify for personal use.

## Support

For issues or questions:
1. Check the troubleshooting section
2. Review the customization guide
3. Ensure all files are properly linked
4. Verify file paths are correct

---

**Last Updated**: January 31, 2026

**Version**: 1.0.0

**Author**: Portfolio Template

For more information, visit the website or contact via email.
