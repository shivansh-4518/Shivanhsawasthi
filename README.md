# 📱 Shivansh Awasthi Portfolio Website

> A modern, clean, and fully responsive personal portfolio website built with pure HTML5 and CSS3.

![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Version](https://img.shields.io/badge/Version-1.0-blue)
![License](https://img.shields.io/badge/License-Personal-orange)

---

## 🎯 Project Overview

This is a beautiful, minimal portfolio website for **Shivansh Awasthi**, showcasing his skills as a web developer and cybersecurity enthusiast. The website is:

- ✨ **No JavaScript** - Pure HTML & CSS
- 📱 **Fully Responsive** - Mobile, Tablet, Desktop
- 🌓 **Dark Mode Support** - Auto-switches based on system preference
- ⚡ **Lightning Fast** - Optimized for performance
- 🎨 **Modern Design** - Clean and professional aesthetics
- ♿ **Semantic HTML** - Accessibility-focused

---

## 🚀 Quick Start

### Option 1: Direct Browser Opening (Easiest)
```bash
# Simply double-click the file:
shivansh_awasthi.html
```

### Option 2: Local Server (Recommended)

**Using Python 3:**
```bash
python -m http.server 8000
# Then open: http://localhost:8000/shivansh_awasthi.html
```

**Using Python 2:**
```bash
python -m SimpleHTTPServer 8000
```

**Using Node.js:**
```bash
npx http-server
```

**Using PHP:**
```bash
php -S localhost:8000
```

---

## 📂 File Structure & Components

### Main Sections

```
┌─ Navigation Bar (Sticky)
│  ├─ Logo/Branding
│  └─ Links: About, Skills, Contact
│
├─ Hero Section
│  ├─ Avatar (SA initials)
│  ├─ Name & Title
│  └─ Quick Tags (Status badges)
│
├─ About Section
│  └─ Professional Bio
│
├─ Skills Section
│  ├─ Web Development (HTML, CSS, Responsive Design)
│  ├─ Cybersecurity (Ethical Hacking)
│  └─ Tools & Interests (VS Code, Open Source)
│
├─ Contact Section
│  ├─ Phone Button
│  └─ Email Button
│
└─ Footer
   └─ Copyright
```

---

## 🎨 Design System

### Color Palette

| Color | Hex Code | Usage |
|-------|----------|-------|
| **Purple** (Primary) | `#7F77DD` | Branding, hover states |
| **Purple Light** | `#EEEDFE` | Backgrounds |
| **Purple Dark** | `#3C3489` | Text on light |
| **Pink** (Web) | `#D4537E` | Web development skills |
| **Pink Light** | `#FBEAF0` | Skill card backgrounds |
| **Teal** (Security) | `#1D9E75` | Cybersecurity, contact |
| **Teal Light** | `#E1F5EE` | Accent backgrounds |
| **Amber** (Tools) | `#BA7517` | Tools & interests |

### Dark Mode Colors

When users have "Dark Mode" enabled on their system, colors automatically adjust:

```css
@media (prefers-color-scheme: dark) {
  --text-primary: #f0f0ee;      /* Light text */
  --bg-primary: #1a1a18;        /* Dark background */
  --border: rgba(255,255,255,0.1);
}
```

### Responsive Breakpoints

| Device | Width | Changes |
|--------|-------|---------|
| **Mobile** | < 540px | Single column, reduced padding |
| **Tablet** | 540-1024px | Full layout |
| **Desktop** | > 1024px | Full layout, max-width 760px |

---

## 🛠️ How to Edit

### 1. Update Personal Information

**Change Name & Title:**
```html
<!-- Line 433-434 -->
<h1>Hey, I'm Shivansh Awasthi 👋</h1>
<p class="subtitle">· Web Developer · Cybersecurity enthusiast</p>
```

**Update Status Tags:**
```html
<!-- Lines 436-438 -->
<span class="tag tag-purple">🎓 Student · Kanpur</span>
<span class="tag tag-pink">🔐 Exploring Cybersecurity</span>
<span class="tag tag-teal">🚀 Open to internships</span>
```

**Update About Section:**
```html
<!-- Lines 445-450 -->
<p class="about-text">
  I'm Shivansh Awasthi, its my passion for web development
  and cybersecurity...
</p>
```

### 2. Add/Remove Skills

**Add a new skill card:**
```html
<div class="skill-card">
  <div class="skill-cat">Category Name</div>
  <div class="skill-list">
    <div class="skill-item">
      <span class="dot dot-purple"></span>JavaScript
    </div>
    <div class="skill-item">
      <span class="dot dot-purple"></span>React
    </div>
  </div>
</div>
```

**Available dot colors:**
- `dot-purple` - Purple dots
- `dot-pink` - Pink dots
- `dot-teal` - Teal dots
- `dot-amber` - Amber dots

### 3. Update Contact Information

**Phone Number:**
```html
<!-- Line 527 -->
<a class="contact-btn" href="tel:+917905191774">
  +91 7905191774
</a>
```

**Email Address:**
```html
<!-- Line 536 -->
<a class="contact-btn" href="mailto:shivanshawasthi51@gmailcom">
  Email me
</a>
```

⚠️ **Note:** Email appears to have a typo. Should be: `shivanshawasthi51@gmail.com`

### 4. Customize Colors

Edit CSS variables at the top:
```css
:root {
  --purple-light: #EEEDFE;
  --purple-mid: #7F77DD;
  --purple-dark: #3C3489;
  --pink-light: #FBEAF0;
  --pink-mid: #D4537E;
  --pink-dark: #72243E;
  /* ... more colors */
}
```

### 5. Change Fonts

```css
body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  /* Replace with your preferred font */
}
```

### 6. Adjust Layout Width

```css
body {
  max-width: 760px;  /* Change this value */
  margin: 0 auto;
}
```

---

## 🔓 Uncomment Features

Several features are currently commented out. To enable them:

### Enable Certificate Section
```html
<!-- Uncomment lines 496-521 -->
<section id="certificates">
  <div class="section-label">certificates</div>
  <!-- certificate cards here -->
</section>
```

### Enable Social Links
```html
<!-- Uncomment lines 545-558 for LinkedIn, GitHub, Twitter buttons -->
<a class="contact-btn" href="https://linkedin.com/in/yourname">LinkedIn</a>
<a class="contact-btn" href="https://github.com/yourname">GitHub</a>
<a class="contact-btn" href="https://twitter.com/yourname">Twitter</a>
```

### Enable Contact Form
```html
<!-- Uncomment lines 410-416 -->
<!-- Requires Web3Forms API setup -->
<form action="https://api.web3forms.com/submit" method="POST">
  <input type="hidden" name="access_key" value="YOUR_KEY">
  <!-- form fields -->
</form>
```

---

## 📱 Browser Compatibility

| Browser | Version | Support |
|---------|---------|---------|
| **Chrome** | Latest | ✅ Full |
| **Firefox** | Latest | ✅ Full |
| **Safari** | Latest | ✅ Full |
| **Edge** | Latest | ✅ Full |
| **Opera** | Latest | ✅ Full |
| **IE** | 11 | ⚠️ Partial (CSS Variables not supported) |

---

## 🐛 Troubleshooting

### Issue: Colors not showing correctly
**Solution:** Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)

### Issue: Email link not working
**Solution:** Check email format in href attribute
```html
<a href="mailto:email@example.com">Email</a>
```

### Issue: Mobile layout not responsive
**Solution:** Ensure viewport meta tag is present in `<head>`:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

### Issue: Dark mode not working
**Solution:** Check system preferences:
- **Windows:** Settings > Personalization > Colors > Dark
- **Mac:** System Preferences > General > Appearance > Dark
- **Linux:** Depends on your desktop environment

### Issue: Phone number link not working
**Solution:** Use proper tel: format
```html
<a href="tel:+917905191774">+91 7905191774</a>
```

---

## 📊 CSS Classes Reference

### Navigation
```css
.nav-logo      /* Logo/branding */
.nav-links     /* Navigation links container */
.nav-links a   /* Individual links */
```

### Hero Section
```css
.hero          /* Hero container */
.avatar        /* Profile avatar circle */
.tags          /* Tags container */
.tag           /* Individual tag */
.tag-purple    /* Purple tag variant */
.tag-pink      /* Pink tag variant */
.tag-teal      /* Teal tag variant */
```

### Skills Section
```css
.skills-grid   /* Grid container */
.skill-card    /* Individual skill card */
.skill-cat     /* Category label */
.skill-list    /* Skills list */
.skill-item    /* Individual skill */
.dot           /* Colored dot */
.dot-purple    /* Purple dot */
.dot-pink      /* Pink dot */
.dot-teal      /* Teal dot */
.dot-amber     /* Amber dot */
```

### Contact Section
```css
.contact-grid  /* Contact buttons grid */
.contact-btn   /* Contact button */
```

---

## 💾 File Specifications

| Property | Value |
|----------|-------|
| **File Type** | HTML5 |
| **Encoding** | UTF-8 |
| **Size** | ~16KB |
| **Lines** | 569 |
| **External Dependencies** | None (self-contained) |
| **JavaScript** | None required |
| **Frameworks** | None |

---

## 🎯 Best Practices

### ✅ Do's
- Use semantic HTML elements
- Test on multiple devices
- Keep descriptions concise
- Use actual profile photo in avatar
- Update contact info regularly
- Test links before deployment

### ❌ Don'ts
- Don't add heavy external libraries
- Don't use inline styling for repeated elements
- Don't forget to test dark mode
- Don't leave placeholder email addresses
- Don't add too many external images
- Don't use deprecated HTML elements

---

## 🚀 Deployment

### Deploy to GitHub Pages
1. Create a GitHub repository
2. Upload `shivansh_awasthi.html` as `index.html`
3. Enable GitHub Pages in settings
4. Visit `username.github.io`

### Deploy to Netlify
1. Drag and drop folder to Netlify
2. Site automatically deploys
3. Get custom domain link

### Deploy to Vercel
1. Push to GitHub
2. Connect repository to Vercel
3. Auto-deploys on push

### Deploy to Firebase Hosting
```bash
npm install -g firebase-tools
firebase login
firebase init
firebase deploy
```

---

## 📝 Current Profile Information

| Field | Value |
|-------|-------|
| **Name** | Shivansh Awasthi |
| **Location** | Kanpur |
| **Status** | Student |
| **Focus Areas** | Web Development, Cybersecurity |
| **Phone** | +91 7905191774 |
| **Email** | shivanshawasthi51@gmailcom* |
| **Status** | Open to Internships |

*Email appears to have typo - missing period before "com"

---

## 📚 Skills Summary

### Web Development
- HTML5
- CSS3 (Modern, Responsive)
- Responsive Design

### Cybersecurity
- Ethical Hacking

### Tools & Interests
- VS Code
- Open Source

---

## 🔐 Security Notes

- No sensitive information is hardcoded
- All contact info can be modified
- No external API calls required
- Static content only - no database needed
- Safe to deploy publicly

---

## 💡 Enhancement Ideas

- [ ] Add dark mode toggle button
- [ ] Add smooth scroll behavior
- [ ] Add project showcase section
- [ ] Add blog/blog section
- [ ] Add testimonials
- [ ] Add experience timeline
- [ ] Add resume download button
- [ ] Add newsletter signup
- [ ] Add animations on scroll
- [ ] Add search functionality

---

## 📞 Contact Information

For questions about this portfolio:
- **Phone:** +91 7905191774
- **Email:** shivanshawasthi51@gmail.com (corrected)
- **Location:** Kanpur, India

---

## 📄 License & Attribution

This is a personal portfolio website. Feel free to use it as a template for your own portfolio!

---

## 🔄 Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2026 | Initial release |

---

## 🙏 Credits

- **Built with:** HTML5 + CSS3
- **Fonts:** System font stack (Apple System, Segoe UI)
- **Icons:** Inline SVG
- **Emojis:** Unicode

---

**Last Updated:** 2026  
**Built with ♥ by Shivansh Awasthi**
