# Portfolio Deployment Guide

## Quick Start

1. **Open locally**: Double-click `index.html` in your file explorer
2. **Or use a local server**: Run one of these commands in the portfolio directory:

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js
npx http-server

# Live Server (VS Code)
# Install extension: "Live Server"
# Right-click index.html > Open with Live Server
```

Then visit: `http://localhost:8000` (or shown port number)

---

## Deploy to Netlify (Easiest)

### Method 1: Drag and Drop
1. Go to https://app.netlify.com/drop
2. Drag the entire Portfolio folder into the drop zone
3. Your site is live instantly!
4. You'll get a live URL like: `https://charming-pancake-abc123.netlify.app`

### Method 2: Git Integration
1. Push files to GitHub
2. Connect GitHub to Netlify
3. Select your repository
4. Click deploy
5. Automatic updates on every push

---

## Deploy to Vercel

1. Go to https://vercel.com
2. Sign up/Log in
3. Click "New Project"
4. Import your GitHub repository (or upload files)
5. Click "Deploy"
6. Get instant live URL

---

## Deploy to GitHub Pages

1. Create a GitHub account and repository
2. Name the repository: `username.github.io`
3. Push your portfolio files to the repository
4. Files are automatically deployed to: `https://username.github.io`

### Using Git Commands:
```bash
git init
git add .
git commit -m "Initial portfolio commit"
git remote add origin https://github.com/username/username.github.io.git
git branch -M main
git push -u origin main
```

---

## Deploy to Traditional Web Hosting

### Using FTP:
1. Get FTP credentials from your hosting provider
2. Use FTP client (FileZilla, Cyberduck, etc.)
3. Connect to your server
4. Upload all files to `public_html` or `www` directory
5. Your site is live at your domain name

### File Upload:
1. Log into your hosting control panel (cPanel, etc.)
2. Use File Manager
3. Upload `index.html`, `styles.css`, `script.js`
4. Wait for files to process
5. Visit your domain

---

## Pre-Deployment Checklist

- [ ] Replace placeholder profile image with actual photo
- [ ] Update all personal information (name, email, phone, links)
- [ ] Verify all external links work (LinkedIn, GitHub, email)
- [ ] Test contact form functionality
- [ ] Test mobile responsiveness
- [ ] Check all animations work
- [ ] Verify no broken image links
- [ ] Update resume/CV links if included
- [ ] Test in multiple browsers
- [ ] Check spelling and grammar
- [ ] Update meta tags for SEO

---

## Custom Domain Setup

### With Netlify:
1. Go to Site Settings > Domain management
2. Click "Add custom domain"
3. Enter your domain name
4. Follow DNS setup instructions
5. Update your domain registrar DNS records

### With GitHub Pages:
1. Create `CNAME` file in repository root
2. Add one line: `yourdomain.com`
3. Push to repository
4. Update DNS records at your registrar

### With Vercel:
1. Go to Project Settings > Domains
2. Add your custom domain
3. Update DNS records
4. Vercel provides SSL automatically

---

## SSL Certificate

Most modern hosting provides free SSL:
- **Netlify**: Automatic
- **Vercel**: Automatic
- **GitHub Pages**: Automatic
- **Traditional Hosting**: Ask your provider (usually free or cheap)

---

## Performance Optimization Tips

1. **Optimize Images**
   - Replace placeholder images with optimized versions
   - Use PNG/JPG for photos
   - Consider WebP format for better compression

2. **Use CDN**
   - Netlify, Vercel, and GitHub Pages use CDN by default
   - Faster delivery worldwide

3. **Enable Caching**
   - Set appropriate cache headers
   - Most hosting does this automatically

4. **Minify Assets** (Optional)
   - Compress CSS and JavaScript
   - Most platforms do this automatically

---

## Monitoring and Analytics

### Add Google Analytics:
1. Create Google Analytics account
2. Add this to `<head>` in index.html:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```
3. Replace `GA_ID` with your tracking ID

---

## Troubleshooting Deployment

### Site shows "File Not Found"
- Ensure `index.html` is in the root directory
- Check file names are correct (case-sensitive on some servers)
- Verify all linked files (CSS, JS) are uploaded

### Styles not loading
- Check file paths in `index.html`
- Ensure `styles.css` is in same directory as `index.html`
- Clear browser cache (Ctrl+Shift+Delete)

### JavaScript not working
- Verify `script.js` is uploaded
- Check console for errors (F12 > Console tab)
- Ensure JavaScript is enabled in browser

### Images not showing
- Replace placeholder URLs with actual image paths
- Upload images to server
- Check image file names and extensions
- Ensure images folder permissions allow access

### Contact form not working
- For GitHub Pages/Static hosting: Need backend service
- Use Formspree, Basin, or Web3Forms for free form handling
- Or deploy to hosting with backend support

---

## Maintenance

### Regular Updates:
1. Update projects and skills regularly
2. Keep experience section current
3. Review and fix broken links quarterly
4. Update contact information if changed
5. Maintain performance monitoring

### Backup:
- Keep local copy of files
- Use version control (Git)
- Regular backups to cloud storage

---

## Domain Registration

Register domain from:
- **GoDaddy**: godaddy.com
- **Namecheap**: namecheap.com
- **Google Domains**: google.com/domains
- **AWS Route 53**: aws.amazon.com
- **Cloudflare**: cloudflare.com (Registrar)

---

## Email Setup

Forward emails from your domain:
- **Netlify**: Built-in email routing
- **Cloudflare**: Free email forwarding
- **Gmail**: Use custom domain with forwarding
- **Workspace**: Business email (paid)

---

## Security

✅ Best Practices:
- Use HTTPS (automatic on all modern hosting)
- Don't expose sensitive information in code
- Keep forms secure with validation
- Regular security updates
- Use strong passwords for hosting

---

## Support

Having issues?
1. Check the README.md file
2. Review this deployment guide
3. Check your hosting provider's support
4. Verify file uploads and permissions
5. Clear browser cache and try again

---

**Happy Deploying! 🚀**
