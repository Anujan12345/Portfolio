# Code Customization Guide

Quick reference for common code modifications needed to personalize your portfolio.

---

## 1. Update Personal Information

### Change Name (Appears in multiple places)

**In index.html - Navbar Brand:**
```html
<!-- Find this: -->
<div class="nav-brand">Anujan</div>

<!-- Change to: -->
<div class="nav-brand">YourName</div>
```

**In index.html - Hero Title:**
```html
<!-- Find this: -->
<h1 class="hero-title">
    <span class="hi-text">Hi, I'm Anujan Ithayarajan</span>
</h1>

<!-- Change to: -->
<h1 class="hero-title">
    <span class="hi-text">Hi, I'm Your Name</span>
</h1>
```

**In index.html - Footer:**
```html
<!-- Find this: -->
<h3>Anujan Ithayarajan</h3>

<!-- Change to: -->
<h3>Your Name</h3>
```

### Update Contact Information

**Email Address:**
```html
<!-- Find all instances of: -->
anujaithayarajan@gmail.com

<!-- Replace with: -->
your.email@gmail.com
```

**Phone Number:**
```html
<!-- Find this: -->
<a href="tel:+94754918695">+94 75 491 8695</a>

<!-- Change to: -->
<a href="tel:+1234567890">+1 (234) 567-8900</a>
```

**LinkedIn Profile:**
```html
<!-- Find this: -->
<a href="https://www.linkedin.com/in/anujan-ithayarajan-bb7112210/" target="_blank">

<!-- Change to: -->
<a href="https://www.linkedin.com/in/your-profile-url/" target="_blank">
```

**GitHub Profile:**
```html
<!-- Find this: -->
<a href="https://github.com/Anujan12345" target="_blank">

<!-- Change to: -->
<a href="https://github.com/your-username" target="_blank">
```

---

## 2. Update Profile Picture

### Replace Placeholder Image

**Find this in index.html:**
```html
<img src="https://via.placeholder.com/300?text=Anujan" alt="Anujan Ithayarajan">
```

**Replace with your image URL:**
```html
<!-- Option 1: Local file in same directory -->
<img src="profile.jpg" alt="Your Name">

<!-- Option 2: External URL -->
<img src="https://example.com/path/to/your-image.jpg" alt="Your Name">

<!-- Option 3: Base64 encoded image -->
<img src="data:image/jpeg;base64,..." alt="Your Name">
```

---

## 3. Update About Section

### Education Information

```html
<!-- Find this: -->
<div class="info-item">
    <h3>Education</h3>
    <p><strong>Electrical and Information Engineering</strong><br>University of Ruhuna, Sri Lanka<br>Graduation: 2026</p>
</div>

<!-- Change to: -->
<div class="info-item">
    <h3>Education</h3>
    <p><strong>Your Degree Name</strong><br>Your University Name<br>Graduation: 20XX</p>
</div>
```

### Location

```html
<!-- Find this: -->
<div class="info-item">
    <h3>Location</h3>
    <p>Sri Lanka</p>
</div>

<!-- Change to: -->
<div class="info-item">
    <h3>Location</h3>
    <p>Your City, Country</p>
</div>
```

### Personal Bio

```html
<!-- Find this paragraph: -->
<p>
    I'm an Electrical and Information Engineering graduate from the University of Ruhuna, Sri Lanka, 
    with a strong passion for electronics and embedded systems...
</p>

<!-- Replace with your bio -->
```

---

## 4. Update Skills with Different Percentages

### Skill Items in About Section

```html
<!-- Find this: -->
<div class="skill-item">
    <span>Embedded Systems</span>
    <div class="skill-bar">
        <div class="skill-progress" style="width: 95%"></div>
    </div>
</div>

<!-- Change the percentage to match your skill level: -->
<div class="skill-item">
    <span>Your Skill Name</span>
    <div class="skill-bar">
        <div class="skill-progress" style="width: 80%"></div>
    </div>
</div>
```

---

## 5. Update Work Experience

### Add New Experience Entry

**Find the experience timeline section and add:**
```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
        <h3>Your Job Title</h3>
        <p class="company">Company Name, Location</p>
        <p class="duration">Start Month YYYY – End Month YYYY</p>
        <ul class="responsibilities">
            <li>Responsibility or achievement 1</li>
            <li>Responsibility or achievement 2</li>
            <li>Responsibility or achievement 3</li>
        </ul>
    </div>
</div>
```

---

## 6. Update Projects

### Modify Existing Project

```html
<!-- Find a project card: -->
<div class="project-card">
    <div class="project-image">
        <div class="project-placeholder">
            <i class="fas fa-car"></i>
        </div>
    </div>
    <div class="project-content">
        <h3>Blind U Bend Safety System</h3>
        <p class="project-description">
            Real-time vehicle detection and alerting system...
        </p>
        <div class="project-tech">
            <span class="tech-tag">ATmega328P</span>
            <span class="tech-tag">NRF24L01</span>
        </div>
        <p class="project-features">
            <strong>Key Features:</strong> Real-time detection...
        </p>
        <a href="#" class="btn-learn-more">Learn More</a>
    </div>
</div>

<!-- Update with your project info: -->
<div class="project-card">
    <div class="project-image">
        <div class="project-placeholder">
            <i class="fas fa-your-icon"></i>  <!-- Change icon -->
        </div>
    </div>
    <div class="project-content">
        <h3>Your Project Title</h3>
        <p class="project-description">
            Your project description goes here...
        </p>
        <div class="project-tech">
            <span class="tech-tag">Technology1</span>
            <span class="tech-tag">Technology2</span>
        </div>
        <p class="project-features">
            <strong>Key Features:</strong> Your features here...
        </p>
        <a href="https://github.com/your-repo" class="btn-learn-more">Learn More</a>
    </div>
</div>
```

### Change Project Icons

Available Font Awesome icons:
- `fa-car` - Vehicle/Transport
- `fa-server` - Server/Cloud
- `fa-microchip` - Processor/Electronics
- `fa-wrench` - Tools/Services
- `fa-magnet` - Magnetic/Special
- `fa-graduation-cap` - Education
- `fa-code` - Programming
- `fa-chart-line` - Analytics
- `fa-robot` - AI/Automation
- [More icons at fontawesome.com](https://fontawesome.com/icons)

---

## 7. Update Services

### Modify Service Card

```html
<!-- Find service card: -->
<div class="service-card">
    <div class="service-icon">
        <i class="fas fa-microchip"></i>
    </div>
    <h3>Embedded System Design</h3>
    <p>Service description...</p>
    <ul class="service-features">
        <li>Feature 1</li>
        <li>Feature 2</li>
    </ul>
</div>

<!-- Update with your service: -->
<div class="service-card">
    <div class="service-icon">
        <i class="fas fa-your-icon"></i>
    </div>
    <h3>Your Service Title</h3>
    <p>Your service description...</p>
    <ul class="service-features">
        <li>Your feature 1</li>
        <li>Your feature 2</li>
    </ul>
</div>
```

---

## 8. Update Technical Skills

### Modify Skill Categories

```html
<!-- Find skill category: -->
<div class="skill-category">
    <h3>Programming Languages</h3>
    <div class="skill-list">
        <span>Python</span>
        <span>C</span>
        <span>C++</span>
    </div>
</div>

<!-- Update with your skills: -->
<div class="skill-category">
    <h3>Your Skill Category</h3>
    <div class="skill-list">
        <span>Skill 1</span>
        <span>Skill 2</span>
        <span>Skill 3</span>
    </div>
</div>
```

---

## 9. Change Color Scheme

In `styles.css`, find `:root` section:

```css
:root {
    --primary-color: #00d4ff;      /* Cyan/Blue - Main color */
    --secondary-color: #7c3aed;    /* Purple - Secondary */
    --accent-color: #a855f7;       /* Light Purple - Accent */
    --dark-bg: #0a0e27;            /* Background */
    --darker-bg: #050810;          /* Darker background */
    --card-bg: #1a1f3a;            /* Card background */
    --text-primary: #e0e6ff;       /* Main text */
    --text-secondary: #a0aec0;     /* Secondary text */
    --border-color: #2d3748;       /* Borders */
    --success-color: #10b981;      /* Success messages */
}
```

### Example: Change to Blue/Orange Theme
```css
:root {
    --primary-color: #3b82f6;      /* Blue */
    --secondary-color: #f97316;    /* Orange */
    --accent-color: #fb923c;       /* Light Orange */
    /* ... rest stays same ... */
}
```

### Example: Change to Green/Teal Theme
```css
:root {
    --primary-color: #10b981;      /* Green */
    --secondary-color: #06b6d4;    /* Teal */
    --accent-color: #14b8a6;       /* Teal Green */
    /* ... rest stays same ... */
}
```

---

## 10. Set Up Contact Form

### Option A: Using Formspree

1. Go to [formspree.io](https://formspree.io/)
2. Sign up and create new form
3. Get your form ID
4. Update form in HTML:

```html
<!-- Find the contact form: -->
<form class="contact-form" id="contactForm">

<!-- Change to: -->
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option B: Using Basin

1. Go to [basinapp.com](https://www.basinapp.com/)
2. Create account and form
3. Update form action:

```html
<form class="contact-form" action="https://usebasin.com/f/YOUR_FORM_ID" method="POST">
```

### Option C: Using Web3Forms

1. Go to [web3forms.com](https://web3forms.com/)
2. Get access key
3. Update form:

```html
<form class="contact-form" action="https://api.web3forms.com/submit" method="POST">
    <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY">
    <!-- rest of form stays same -->
</form>
```

---

## 11. Add Custom Fonts

In `index.html`, add to `<head>`:

```html
<!-- Google Fonts Example -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

<!-- Then in styles.css, update body font: -->
body {
    font-family: 'Inter', sans-serif;
    /* ... rest stays same ... */
}
```

---

## 12. Add Google Analytics

In `index.html`, add to `<head>` before closing tag:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your Google Analytics ID.

---

## 13. Add Resume Download Link

Add to the hero buttons section:

```html
<div class="hero-buttons">
    <a href="#projects" class="btn btn-primary">View My Work</a>
    <a href="resume.pdf" class="btn btn-secondary" download>Download Resume</a>
    <a href="#contact" class="btn btn-secondary">Get In Touch</a>
</div>
```

Place your `resume.pdf` in the same folder as `index.html`.

---

## 14. Add Social Links

Add more social profiles:

```html
<div class="hero-socials">
    <a href="https://www.linkedin.com/in/your-profile/" target="_blank" class="social-link">
        <i class="fab fa-linkedin"></i>
    </a>
    <a href="https://github.com/your-username" target="_blank" class="social-link">
        <i class="fab fa-github"></i>
    </a>
    <a href="https://twitter.com/your-handle" target="_blank" class="social-link">
        <i class="fab fa-twitter"></i>
    </a>
    <a href="mailto:your.email@gmail.com" class="social-link">
        <i class="fas fa-envelope"></i>
    </a>
</div>
```

Available social icons:
- `fa-linkedin` - LinkedIn
- `fa-github` - GitHub
- `fa-twitter` - Twitter
- `fa-facebook` - Facebook
- `fa-instagram` - Instagram
- `fa-youtube` - YouTube
- `fa-envelope` - Email

---

## Common CSS Changes

### Adjust Container Width
```css
.container {
    max-width: 1200px;  /* Change this value */
}
```

### Increase Section Padding
```css
section {
    padding: 5rem 0;  /* Change this value */
}
```

### Change Button Size
```css
.btn {
    padding: 12px 30px;  /* Increase or decrease */
}
```

### Adjust Font Size
```css
html {
    font-size: 16px;  /* Default, adjust as needed */
}
```

---

## Testing Your Changes

After making modifications:

1. Save the file
2. Refresh browser (Ctrl+R or Cmd+R)
3. Clear cache if needed (Ctrl+Shift+Delete)
4. Test on mobile (F12 > Responsive Design Mode)
5. Check console for errors (F12 > Console)

---

**Need Help?**
- Check README.md for overview
- Review CUSTOMIZATION_CHECKLIST.md for complete list
- Search for specific section in this guide
- Check Font Awesome docs: fontawesome.com
- Check HTML structure for proper nesting

Good luck customizing! 🎨
