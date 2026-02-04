# EmailJS Setup Guide

If your contact form is not sending emails, follow these steps to properly set up EmailJS.

## Step 1: Create EmailJS Account

1. Go to [https://www.emailjs.com/](https://www.emailjs.com/)
2. Click **Sign Up**
3. Create a free account
4. Verify your email

## Step 2: Add Email Service

1. Log in to EmailJS dashboard
2. Go to **Email Services** (left sidebar)
3. Click **Add Service**
4. Choose **Gmail** (or your email provider)
5. Connect your email account and grant access
6. Copy your **Service ID** (looks like: `service_xxxxx`)
7. Save the service

## Step 3: Create Email Template

1. Go to **Email Templates** (left sidebar)
2. Click **Create New Template**
3. Fill in the template with these variables:

### Template Settings:
- **Template Name**: `Contact Form` (or any name)
- **Template ID**: Note this (looks like: `template_xxxxx`)
- **To Email**: `{{to_email}}`
- **Subject**: `{{subject}}`

### Email Body Template:

```
Name: {{user_name}}
Email: {{user_email}}
Subject: {{subject}}

Message:
{{message}}
```

4. Click **Save**
5. Copy your **Template ID**

## Step 4: Get Your Credentials

You now need three pieces of information:

1. **Public Key** - From Account Settings > API Keys
   - Currently using: `VNi4qggr8vF4zJZHU`

2. **Service ID** - From your email service (created in Step 2)
   - Example: `service_nrrlr3l`

3. **Template ID** - From your email template (created in Step 3)
   - Example: `template_qg4p9ml`

## Step 5: Update Portfolio Code

Your credentials are already configured:
- Public Key: `VNi4qggr8vF4zJZHU`
- Service ID: `service_nrrlr3l`
- Template ID: `template_qg4p9ml`

If you created new credentials, update in `script.js`:

```javascript
// Line ~1: Change this
emailjs.init('VNi4qggr8vF4zJZHU');

// Line ~57-58: Change these
emailjs.send('service_nrrlr3l', 'template_qg4p9ml', {
```

## Step 6: Test the Form

1. **Refresh browser** (Ctrl+R)
2. **Open Developer Tools** (F12)
3. **Go to Console tab**
4. **Fill the contact form** with test data
5. **Click "Send Message"**
6. **Watch console output** for success/error messages
7. **Check your email** for the received message

## Troubleshooting

### Console Shows: "Template not found"
- Create the template in EmailJS (Step 3)
- Verify Template ID matches in script.js

### Console Shows: "Invalid credentials"
- Check Public Key, Service ID, and Template ID
- Verify they're correct in script.js

### Console Shows: "Network error"
- Check internet connection
- Verify EmailJS script is loading (F12 > Sources)

### No console error but email not received
- Check Spam/Junk folder in email
- Verify email address in template is correct
- Check EmailJS dashboard for email logs

## Console Debug Messages

Open F12 > Console to see:
- ✅ `EmailJS initialized successfully` - Library loaded
- ✅ `Contact form found` - Form detected
- 📨 `Form submission triggered` - User clicked send
- 📋 `Form data:` - What was submitted
- 🔄 `Sending email via EmailJS...` - Processing
- ✅ `Email sent successfully!` - Success
- ❌ `EmailJS error detected` - Error occurred

## Gmail Setup (Recommended)

If using Gmail:

1. Allow "Less secure app access" OR
2. Use [Google App Password](https://support.google.com/accounts/answer/185833):
   - Go to Google Account > Security
   - Generate App Password for Gmail
   - Use that password in EmailJS

## Free Plan Limitations

EmailJS Free Plan:
- 200 emails per month
- Basic support
- All features enabled

## Alternative Services

If EmailJS doesn't work:
- [Formspree](https://formspree.io/) - Simple form backend
- [Basin](https://www.basinapp.com/) - Form submission service
- [Web3Forms](https://web3forms.com/) - Modern form service

## Quick Checklist

- [ ] EmailJS account created
- [ ] Email service added (Gmail/etc)
- [ ] Email template created
- [ ] Template has correct variables
- [ ] Public Key in script.js is correct
- [ ] Service ID in script.js is correct
- [ ] Template ID in script.js is correct
- [ ] Portfolio refreshed in browser
- [ ] Test email sent
- [ ] Email received in inbox

---

**Need Help?**
1. Check browser console (F12 > Console)
2. Review error messages shown
3. Follow the troubleshooting section above
4. Visit [EmailJS Docs](https://www.emailjs.com/docs/)
5. Contact EmailJS support if needed

**Last Updated:** January 31, 2026
