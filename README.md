# 📱 Shivansh Awasthi - Portfolio Website

> एक आधुनिक, साफ और पूरी तरह responsive personal portfolio website जो HTML5 और CSS3 से बना है।

---

## 🎯 Project Overview

यह एक beautiful portfolio website है **Shivansh Awasthi** के लिए जो उनकी web development और cybersecurity skills को showcase करती है।

### ✨ Key Features:
- ✅ **No JavaScript** - Pure HTML & CSS (कोई external library नहीं)
- 📱 **Fully Responsive** - Mobile, Tablet, Desktop सब पर काम करता है
- 🌓 **Dark Mode Support** - System preference के अनुसार automatically switch होता है
- ⚡ **Lightning Fast** - Performance optimized
- 🎨 **Modern Design** - Clean और professional look
- 🔒 **Secure** - कोई sensitive data नहीं, सब safe है

---

## 🚀 Quick Start - File कैसे खोलें

### Option 1: सीधे Browser में खोलें (सबसे आसान)
```
बस फाइल को double-click करो:
shivansh_awasthi.html
```

### Option 2: Python से Local Server पर चलाएं (Recommended)

**Python 3 के साथ:**
```bash
python -m http.server 8000
# फिर खोलो: http://localhost:8000/shivansh_awasthi.html
```

**Python 2 के साथ:**
```bash
python -m SimpleHTTPServer 8000
```

**Node.js के साथ:**
```bash
npx http-server
```

---

## 📂 Website का Structure

```
📄 shivansh_awasthi.html
├── 🧭 Navigation Bar (Sticky)
│   ├── Logo: "Shivansh ✦"
│   └── Links: About, Skills, Contact
│
├── 🎯 Hero Section
│   ├── Avatar (SA initials)
│   ├── Name: "Hey, I'm Shivansh Awasthi 👋"
│   ├── Subtitle: "Web Developer · Cybersecurity enthusiast"
│   └── Quick Tags (Status badges)
│
├── 📝 About Section
│   └── Professional Bio (web development और cybersecurity के बारे में)
│
├── 🛠️ Skills Section
│   ├── Web Development
│   │   ├── HTML
│   │   ├── CSS
│   │   └── Responsive Design
│   ├── Cybersecurity
│   │   └── Ethical Hacking
│   └── Tools & Interests
│       ├── VS Code
│       └── Open Source
│
├── 💬 Contact Section
│   ├── Phone Button: +91 7905191774
│   └── Email Button
│
└── 📄 Footer
    └── Copyright
```

---

## 🎨 Design System

### Color Palette

| Color | Hex Code | कहाँ use होता है |
|-------|----------|-----------------|
| Purple (Main) | `#7F77DD` | Branding, hover states |
| Purple Light | `#EEEDFE` | Backgrounds |
| Purple Dark | `#3C3489` | Dark text |
| Pink (Web) | `#D4537E` | Web development |
| Pink Light | `#FBEAF0` | Skill backgrounds |
| Teal (Security) | `#1D9E75` | Cybersecurity, Contact |
| Teal Light | `#E1F5EE` | Accent backgrounds |
| Amber (Tools) | `#BA7517` | Tools & interests |

### Dark Mode 🌓
जब user के device पर Dark Mode enable है, तो colors automatically adjust हो जाते हैं:
- Text: Light color (#f0f0ee)
- Background: Dark color (#1a1a18)

### Responsive Breakpoints 📱

| Device | Width | Layout |
|--------|-------|--------|
| **Mobile** | < 540px | Single column, stacked |
| **Tablet** | 540-1024px | 2-3 columns |
| **Desktop** | > 1024px | Full layout (max 760px width) |

---

## ✏️ How to Customize/Edit करें

### 1️⃣ अपना नाम और Info बदलें

**Heading बदलें (Line 433-434):**
```html
<h1>Hey, I'm Shivansh Awasthi 👋</h1>
<p class="subtitle">· Web Developer · Cybersecurity enthusiast</p>
```

**Status Tags update करें (Lines 436-438):**
```html
<span class="tag tag-purple">🎓 Student · Kanpur</span>
<span class="tag tag-pink">🔐 Exploring Cybersecurity</span>
<span class="tag tag-teal">🚀 Open to internships</span>
```

### 2️⃣ About Section बदलें

```html
<!-- Line 445-450 -->
<p class="about-text">
  यहाँ अपना bio लिखो...
</p>
```

### 3️⃣ Skills Add/Remove करें

**नया skill add करने के लिए:**
```html
<div class="skill-card">
  <div class="skill-cat">Category Name</div>
  <div class="skill-list">
    <div class="skill-item">
      <span class="dot dot-purple"></span>Skill Name
    </div>
  </div>
</div>
```

**Dot Colors (choose कर सकते हो):**
- `dot-purple` - Purple dot
- `dot-pink` - Pink dot
- `dot-teal` - Teal dot
- `dot-amber` - Amber dot

### 4️⃣ Contact Info Update करें

**Phone Number (Line 527):**
```html
<a class="contact-btn" href="tel:+917905191774">
  +91 7905191774
</a>
```

**Email (Line 536):**
```html
<a class="contact-btn" href="mailto:your-email@gmail.com">
  Email me
</a>
```

⚠️ **Important:** Email में typo fix करो - `shivanshawasthi51@gmailcom` → `shivanshawasthi51@gmail.com`

### 5️⃣ Colors Customize करें

CSS variables को edit करो (Line 18-38):
```css
:root {
  --purple-mid: #7F77DD;    /* अपना color डालो */
  --pink-mid: #D4537E;
  --teal-mid: #1D9E75;
  /* और भी colors... */
}
```

### 6️⃣ Font बदलें

```css
body {
  font-family: 'अपना font name';
  /* Current: -apple-system, BlinkMacSystemFont, 'Segoe UI' */
}
```

### 7️⃣ Layout Width Adjust करें

```css
body {
  max-width: 760px;  /* यह value बदलो */
  margin: 0 auto;
}
```

---

## 🔓 Hidden Features को Enable करें

### ✅ Certificates Section Enable करें

अगर certificates add करना हैं तो lines 496-521 को uncomment करो

### ✅ Social Media Links Enable करें

LinkedIn, GitHub, Twitter buttons के लिए lines 545-558 को uncomment करो:
```html
<a class="contact-btn" href="https://linkedin.com/in/yourname">LinkedIn</a>
<a class="contact-btn" href="https://github.com/yourname">GitHub</a>
<a class="contact-btn" href="https://twitter.com/yourname">Twitter</a>
```

---

## 📱 Browser Support

| Browser | Status |
|---------|--------|
| Chrome | ✅ Full Support |
| Firefox | ✅ Full Support |
| Safari | ✅ Full Support |
| Edge | ✅ Full Support |
| Opera | ✅ Full Support |
| IE 11 | ⚠️ Partial (CSS Variables काम नहीं करते) |

---

## 🐛 Troubleshooting - Common Issues

### ❌ Issue: Colors सही नहीं दिख रहे
**Solution:** Browser cache clear करो
- **Windows:** Ctrl + Shift + Delete
- **Mac:** Cmd + Shift + Delete
- या: Ctrl + Shift + R (या Cmd + Shift + R)

### ❌ Issue: Email link काम नहीं कर रहा
**Solution:** Email format सही करो
```html
<a href="mailto:email@example.com">Email</a>
```

### ❌ Issue: Mobile पर responsive नहीं है
**Solution:** यह meta tag check करो (होना चाहिए `<head>` में):
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

### ❌ Issue: Dark mode काम नहीं कर रहा
**Solution:** अपने device का dark mode check करो:
- **Windows:** Settings > Personalization > Colors > Dark
- **Mac:** System Preferences > General > Appearance > Dark

### ❌ Issue: Phone link काम नहीं कर रहा
**Solution:** सही format use करो:
```html
<a href="tel:+917905191774">Call me</a>
```

---

## 🎯 File की Details

| Detail | Value |
|--------|-------|
| **File Type** | HTML5 |
| **Encoding** | UTF-8 |
| **Size** | ~16KB |
| **Lines** | 569 |
| **External Dependencies** | None |
| **JavaScript** | Required नहीं |
| **Frameworks** | कोई नहीं |

---

## 📊 CSS Classes - Quick Reference

### Navigation
- `.nav-logo` - Logo text
- `.nav-links` - Navigation links container

### Hero Section
- `.hero` - Main hero container
- `.avatar` - Profile avatar circle
- `.tag-purple`, `.tag-pink`, `.tag-teal` - Tag variants

### Skills
- `.skills-grid` - Grid container
- `.skill-card` - Individual skill card
- `.skill-item` - Individual skill
- `.dot-purple`, `.dot-pink`, `.dot-teal`, `.dot-amber` - Colored dots

### Contact
- `.contact-btn` - Contact button

---

## ✅ Best Practices

### करो ✅
- ✅ Real profile photo use करो
- ✅ Multiple devices पर test करो
- ✅ Contact info सही रखो
- ✅ Links को test करो deployment से पहले
- ✅ Dark mode को check करो
- ✅ Mobile view को test करो

### मत करो ❌
- ❌ Heavy external libraries add मत करो
- ❌ Inline styles बार-बार मत लिखो
- ❌ Placeholder info छोड़ मत दो
- ❌ Broken links मत रखो
- ❌ Outdated information मत रखो

---

## 🚀 Deploy करने के तरीके

### GitHub Pages
1. GitHub account बनाओ
2. Repository: `username.github.io`
3. `index.html` upload करो
4. Visit: `username.github.io`

### Netlify
1. Netlify.com पर जाओ
2. Folder drag & drop करो
3. Auto-deploy हो जाएगा

### Vercel
1. Vercel.com पर जाओ
2. GitHub repository connect करो
3. Auto-deploy on push

---

## 👤 Profile Information

| Info | Value |
|------|-------|
| **Name** | Shivansh Awasthi |
| **Location** | Kanpur |
| **Status** | Student |
| **Focus** | Web Development, Cybersecurity |
| **Phone** | +91 7905191774 |
| **Email** | shivanshawasthi51@gmail.com |
| **Open to** | Internships |

---

## 💻 Skills Summary

### Web Development 🌐
- HTML5
- CSS3 (Modern + Responsive)
- Responsive Web Design

### Cybersecurity 🔐
- Ethical Hacking

### Tools 🛠️
- VS Code
- Open Source

---

## 🔐 Security

- ✅ कोई sensitive data नहीं
- ✅ कोई database नहीं
- ✅ Static content only
- ✅ Public deploy करने के लिए safe है

---

## 💡 Future Enhancement Ideas

- [ ] Contact form add करो
- [ ] Projects section add करो
- [ ] Blog/Articles section
- [ ] Experience timeline
- [ ] Testimonials section
- [ ] Resume download button
- [ ] Scroll animations
- [ ] Social media links

---

## 📞 Contact

- **Phone:** +91 7905191774
- **Email:** shivanshawasthi51@gmail.com
- **Location:** Kanpur, India

---

## 📄 License

यह एक personal portfolio है। अपना portfolio बनाने के लिए इसे template के रूप में use कर सकते हो!

---

## 📝 Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2026 | Initial Release |
| 1.1 | 2026 | Fixed HTML structure & Skills section |

---

**Last Updated:** 2026  
**Built with ♥ by Shivansh Awasthi**

✨ Happy customizing! ✨

