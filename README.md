[README (1).md](https://github.com/user-attachments/files/29912795/README.1.md)
# Shivansh Awasthi — Portfolio Website

A modern, responsive personal portfolio website showcasing web development skills and cybersecurity interests.

## 📋 Overview

This is a sleek, single-page portfolio website built with HTML and CSS. The site presents Shivansh Awasthi's professional profile, skills, and contact information with a clean, modern design.

### Key Features

- **Responsive Design**: Adapts beautifully to mobile, tablet, and desktop screens
- **Dark Mode Support**: Automatically adapts to system color preferences
- **Modern Styling**: Custom CSS with color variables and smooth transitions
- **Fast Performance**: Lightweight, no frameworks or heavy dependencies
- **Clean Navigation**: Sticky navigation bar with smooth scrolling anchors
- **Professional Layout**: Well-organized sections for easy information access

## 📁 File Structure

```
shivansh_awasthi.html
├── Embedded CSS Styles
├── Navigation Bar
├── Hero Section (Introduction)
├── About Section
├── Skills Section
├── Contact Section
└── Footer
```

## 🎨 Design Elements

### Color Scheme

- **Primary Purple**: `#7F77DD` — Main branding color
- **Pink Accent**: `#D4537E` — Web development skills
- **Teal Accent**: `#1D9E75` — Cybersecurity focus
- **Amber Accent**: `#BA7517` — Tools & interests
- **Dark/Light Modes**: Full support with CSS variables

### Sections

| Section | Purpose |
|---------|---------|
| **Navigation** | Quick links to About, Skills, and Contact |
| **Hero** | Introduction with avatar and key tags |
| **About** | Personal bio and professional summary |
| **Skills** | Categorized skill cards (Web, Cybersecurity, Tools) |
| **Contact** | Phone and email contact buttons |
| **Footer** | Copyright and attribution |

## 📱 Responsive Breakpoints

- **Desktop**: Full layout with side-by-side arrangements
- **Mobile** (< 540px): Optimized for smaller screens with adjusted padding and single-column layouts

## 🚀 How to Use

### Opening the File

1. **Direct Opening**: Simply double-click `shivansh_awasthi.html` to open in your default browser
2. **Drag & Drop**: Drag the HTML file onto a browser window
3. **Via Server**: For the best experience, serve through a local web server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

### Customization

#### Change Colors
Edit the CSS variables in the `:root` selector (lines 18-38):
```css
:root {
  --purple-mid: #7F77DD;  /* Change brand color */
  --pink-mid: #D4537E;    /* Change accent colors */
  /* ... etc */
}
```

#### Update Personal Information

- **Name**: Line 433 in the hero section
- **Subtitle**: Line 434
- **Tags**: Lines 436-438
- **About Text**: Lines 445-450
- **Contact Number**: Line 527
- **Email**: Line 536

#### Add More Skills

In the skills section, duplicate a skill-card div and modify:
```html
<div class="skill-card">
  <div class="skill-cat">Category Name</div>
  <div class="skill-list">
    <div class="skill-item"><span class="dot dot-purple"></span>Skill Name</div>
  </div>
</div>
```

#### Uncomment Features

Several features are commented out in the HTML:
- **Contact Form** (lines 410-416): Requires Web3Forms setup
- **Certificates Section** (lines 496-521): Uncomment to enable
- **LinkedIn/GitHub/Twitter Links** (lines 545-558): Uncomment and update URLs

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: 
  - CSS Variables for theming
  - Flexbox for layout
  - CSS Grid for responsive cards
  - Media queries for mobile optimization
- **No JavaScript** required (fully static)

## 🔧 Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome/Chromium | ✅ Full support |
| Firefox | ✅ Full support |
| Safari | ✅ Full support |
| Edge | ✅ Full support |
| IE 11 | ⚠️ Limited (CSS variables not supported) |

## 💡 Tips for Customization

1. **Font**: Change system font stack in `body` selector (line 55)
2. **Max Width**: Adjust `max-width: 760px` in body for different content widths
3. **Spacing**: Modify `padding` values in section styles
4. **Radius**: Change `--radius-md` and `--radius-lg` for rounder/sharper corners
5. **Hover Effects**: Modify transition effects in `.cert-card:hover` (line 278)

## 📞 Contact Information

- **Phone**: +91 7905191774
- **Email**: shivanshawasthi51@gmailcom (note: appears to have typo in email)

## 🎯 Current Skills

- **Web**: HTML, CSS, Responsive Design
- **Cybersecurity**: Ethical Hacking
- **Tools**: VS Code, Open Source

## 🔗 Notes

- Several contact links are commented out (LinkedIn, GitHub, Twitter) — uncomment and update as needed
- Email link appears to have a typo (missing dot before 'com')
- Certificate section is available but commented out
- Form integration with Web3Forms is commented out but configured

## 📄 License

This is a personal portfolio. Feel free to use as a template for your own portfolio website.

---

**Built with ♥ · 2026**
