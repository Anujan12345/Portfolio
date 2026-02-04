# Formspree Contact Form Setup

Your portfolio now uses **Formspree** for email handling - which is much simpler and more reliable than EmailJS!

## ✅ Current Status

The contact form is **already configured** with Formspree endpoint:
- Form Action: `https://formspree.io/f/mzzplwzp`
- This endpoint is temporary/demo

## 🔧 To Make It Your Own (2 minutes)

### Step 1: Create Formspree Account
1. Go to [https://formspree.io/](https://formspree.io/)
2. Click **Sign Up** (or Sign In if you have account)
3. Verify your email

### Step 2: Create New Form
1. Click **Create Form**
2. Name it: `Contact Form` (or any name)
3. You'll get a **Form ID** (looks like: `mzzplwzp`)

### Step 3: Verify Email
1. Formspree will send verification email to your address
2. Click the verification link in the email

### Step 4: Update Portfolio Form
Once you have your form ID from Formspree:

**In index.html**, find this line (around line 673):
```html
<form class="contact-form" id="contactForm" action="https://formspree.io/f/mzzplwzp" method="POST">
```

Replace `mzzplwzp` with your actual Formspree Form ID:
```html
<form class="contact-form" id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Step 5: Test It!
1. Refresh browser
2. Fill out contact form
3. Click "Send Message"
4. You should receive the email

## How It Works

1. User fills form and clicks send
2. Form data is sent to Formspree
3. Formspree forwards email to you
4. Formspree redirects back to your site

**No external JavaScript libraries needed!**
**No API keys to manage!**
**Just works!**

## Features

✅ **Free Plan Includes:**
- Unlimited forms
- Unlimited submissions
- Email forwarding
- Basic spam protection
- Mobile responsive forms

✅ **What You Get:**
- Emails sent to your inbox
- Custom email addresses
- Form data saved in dashboard
- No coding required

## Testing

### Current Status
- Form is ready to use
- Currently uses demo Form ID: `mzzplwzp`
- Emails go to Formspree (you can view in dashboard)

### To Receive Emails
- Complete Steps 1-3 above
- Update your Form ID in HTML
- Now emails come to YOU

## Troubleshooting

### Form not submitting
- Check internet connection
- Verify form action URL is correct
- Check browser console (F12) for errors

### Not receiving emails
- Verify email was confirmed in Formspree
- Check spam/junk folder
- Log into Formspree dashboard to see submissions

### Customize Form Submission
You can customize behavior in Formspree dashboard:
- Auto-reply to users
- Redirect after submission
- Customize confirmation page
- Set up webhooks

## Alternative Services

If you want different functionality:
- **Basin** - Basin.app (simple alternative)
- **Netlify Forms** - If deployed on Netlify
- **Web3Forms** - Web3forms.com (modern option)

## Important Notes

⚠️ **Current Form ID** (`mzzplwzp`) is for testing
- If you don't create your own, emails won't reach you
- Takes 2 minutes to set up your own

## FAQ

**Q: Is this free?**
A: Yes! Formspree has a generous free plan.

**Q: Will my emails be private?**
A: Yes, only you receive emails from your form.

**Q: Can I customize the form?**
A: Yes, in your Formspree dashboard.

**Q: What if I get spam?**
A: Formspree has spam protection. You can block addresses.

## Quick Checklist

- [ ] Go to formspree.io
- [ ] Sign up (free)
- [ ] Create new form
- [ ] Verify your email
- [ ] Copy your Form ID
- [ ] Update HTML with your Form ID
- [ ] Test the form
- [ ] Deploy to live server
- [ ] Share your portfolio!

---

**Questions?**
- Formspree Docs: https://formspree.io/docs/
- Formspree Support: support@formspree.io

**All set! Your contact form is ready to go!** 🚀
