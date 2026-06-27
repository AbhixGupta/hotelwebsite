# 🏨 Ganga Heritage - Haridwar Hotel Website

A beautifully designed, fully responsive hotel website with three distinct versions - from clean modern to artistic watercolor aesthetics. Built with Tailwind CSS and featuring smooth animations, cultural elements, and spiritual themes.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 📸 Live Preview

**Choose your style:**
- 🎯 **Clean Modern** → `index.html`
- ✨ **Animated Wix-Style** → `index-animated.html`
- 🎨 **Artistic Watercolor** → `index-painted.html`

## 🌟 Features

### Common to All Versions:
- ✅ **Fully Responsive** - Mobile-first design that works on all devices
- ✅ **Authentic Haridwar Theme** - Saffron, terracotta, and Ganges blue color palette
- ✅ **Cultural Elements** - Om symbols, traditional patterns, Vedic architecture
- ✅ **Booking System** - Contact forms and booking widgets
- ✅ **Room Showcase** - Beautiful room cards with pricing
- ✅ **Experiences Section** - Yoga, Ganga Aarti, Ayurveda offerings
- ✅ **Testimonials** - Guest reviews with ratings
- ✅ **Gallery** - Image showcase section
- ✅ **Smooth Navigation** - Sticky navbar with smooth scroll

### Version-Specific Features:

#### 1. **index.html** - Clean Modern Version
- Professional, clean design
- Fast loading (~49KB)
- Perfect for production use
- Simple hover effects

#### 2. **index-animated.html** - Wix-Style Animated
- **AOS Library** - Scroll-triggered animations (fade, zoom, flip)
- **Parallax Effect** - Hero image moves on scroll
- **Counter Animations** - Stats count up from 0
- **Image Zoom** - Smooth zoom on hover
- **Stagger Effects** - Sequential card animations
- **Shine Effects** - Button hover animations

#### 3. **index-painted.html** - Artistic Watercolor ⭐ RECOMMENDED
- **Watercolor Backgrounds** - Organic gradient overlays
- **Om Symbol Decorations** - Rotating sacred symbols
- **Floating Organic Shapes** - Animated blob shapes with blur
- **Brush Stroke Dividers** - Hand-painted style separators
- **Lotus Petal Patterns** - Traditional Indian motifs
- **Paper Texture** - Canvas-like backgrounds
- **Botanical Accents** - Decorative plant illustrations
- All animations from the animated version + artistic flair

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/AbhixGupta/hotelwebsite.git
cd hotelwebsite
```

### 2. Open Locally
Simply open any HTML file in your browser:
```bash
# On macOS
open index-painted.html

# On Windows
start index-painted.html

# On Linux
xdg-open index-painted.html
```

Or use a local server (recommended for best experience):
```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using VS Code Live Server extension
# Right-click on HTML file → "Open with Live Server"
```

Then visit: `http://localhost:8000/index-painted.html`

### 3. No Build Process Required!
All versions use **CDN-based Tailwind CSS** - no installation or build tools needed. Just edit and refresh!

## 🎨 Customization Guide

### 1. Change Hotel Name & Details

**Update in all three files:**

```html
<!-- Find and replace these sections -->

<!-- Logo & Brand Name -->
<h3 class="font-heading text-2xl font-bold text-ganges">Ganga Heritage</h3>
<p class="text-xs text-terracotta -mt-1">The Sacred Stay</p>

<!-- Hero Headline -->
<h1>Where The Ganges Whispers and Tradition Breathes</h1>

<!-- Contact Information -->
<p class="text-white/80">Near Har Ki Pauri, Upper Road<br/>Haridwar, Uttarakhand 249401</p>
<p class="text-white/80">+91 1334 225 XXX<br/>reservations@gangaheritage.com</p>
```

### 2. Change Colors

**Edit the Tailwind config in `<script>` tag:**

```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                saffron: '#FF9933',      // Change primary color
                terracotta: '#C8654A',   // Change secondary color
                ganges: '#1E5F74',       // Change accent color
                gold: '#D4AF37',         // Change highlight color
                // ... add more colors
            }
        }
    }
}
```

### 3. Replace Images

**Find all image URLs and replace with your own:**

```html
<!-- Example: Hero background -->
<img src="https://images.unsplash.com/photo-1609920658906-8223bd289001?w=1920&q=80"
     alt="Your alt text">

<!-- Replace with your image path -->
<img src="./images/your-hotel-photo.jpg" alt="Your alt text">
```

**Recommended image sizes:**
- Hero: 1920x1080px
- Room cards: 800x600px
- Gallery: 600x600px
- Experiences: 800x500px

### 4. Update Room Details

**Find room cards section:**

```html
<div class="p-6">
    <h3>Ganges View Suite</h3>          <!-- Room name -->
    <p>Wake up to breathtaking...</p>    <!-- Description -->
    <span>2 Guests</span>                <!-- Capacity -->
    <span>35 m²</span>                   <!-- Size -->
    <span>₹4,999</span>                  <!-- Price -->
</div>
```

### 5. Modify Animation Speed (animated & painted versions)

**Edit AOS initialization in `<script>` section:**

```javascript
AOS.init({
    duration: 800,        // Change animation duration (ms)
    easing: 'ease-in-out', // Change easing function
    once: true,           // Animate only once
    offset: 100           // Trigger offset (px)
});
```

### 6. Change Fonts

**Replace Google Fonts in `<head>`:**

```html
<!-- Current fonts -->
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<!-- Replace with your preferred fonts -->
<link href="https://fonts.googleapis.com/css2?family=Your+Font&display=swap" rel="stylesheet">
```

Then update in config:
```javascript
fontFamily: {
    heading: ['Your Heading Font', 'serif'],
    body: ['Your Body Font', 'sans-serif']
}
```

## 📁 File Structure

```
hotelwebsite/
│
├── index.html              # Clean modern version (49KB)
├── index-animated.html     # Animated Wix-style version (69KB)
├── index-painted.html      # Artistic watercolor version (95KB)
└── README.md              # This file
```

**Optional folders you can add:**
```
├── images/                # Your hotel photos
├── css/                   # Additional custom CSS
└── js/                    # Additional custom JavaScript
```

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS 3.x** - Utility-first CSS framework (via CDN)
- **Vanilla JavaScript** - No frameworks needed
- **AOS Library** - Animate On Scroll (animated & painted versions)
- **Google Fonts** - Cormorant Garamond + Inter

## 🌐 Deployment

### Deploy to GitHub Pages (FREE)

1. **Push to GitHub** (already done!)
2. **Enable GitHub Pages:**
   - Go to your repo: https://github.com/AbhixGupta/hotelwebsite
   - Click **Settings** → **Pages**
   - Under "Source", select **main** branch
   - Click **Save**
3. **Your site will be live at:**
   ```
   https://abhixgupta.github.io/hotelwebsite/
   ```

4. **Set default page** (optional):
   - Rename your preferred version to `index.html`
   - Or update GitHub Pages settings to point to specific file

### Deploy to Netlify (FREE)

1. **Drag & Drop:**
   - Visit [netlify.com](https://www.netlify.com/)
   - Drag your folder to deploy
   - Get instant live URL

2. **Via Git:**
   - Connect your GitHub repository
   - Auto-deploy on every push

### Deploy to Vercel (FREE)

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Follow prompts
```

## 🎯 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📱 Responsive Breakpoints

```css
sm:  640px  /* Small devices */
md:  768px  /* Tablets */
lg:  1024px /* Laptops */
xl:  1280px /* Desktops */
2xl: 1536px /* Large screens */
```

## 💡 Tips & Best Practices

### For Best Performance:
1. **Optimize Images:**
   - Use WebP format for modern browsers
   - Compress images with [TinyPNG](https://tinypng.com/)
   - Recommended: 80-85% quality

2. **Lazy Load Images:**
   ```html
   <img src="image.jpg" loading="lazy" alt="Description">
   ```

3. **Add Meta Tags for SEO:**
   ```html
   <meta name="description" content="Your hotel description">
   <meta property="og:image" content="your-og-image.jpg">
   <meta name="keywords" content="haridwar, hotel, spiritual, ganges">
   ```

### For Easy Maintenance:
1. Keep one version active
2. Store images in `/images/` folder
3. Use meaningful alt text for all images
4. Test on mobile devices regularly

## 🔧 Common Customizations

### Add WhatsApp Button:
```html
<a href="https://wa.me/919999999999" 
   class="fixed bottom-6 right-6 bg-green-500 text-white p-4 rounded-full shadow-lg z-50">
    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
        <!-- WhatsApp icon SVG -->
    </svg>
</a>
```

### Change Copyright Year Automatically:
```html
<p>© <span id="year"></span> Ganga Heritage. All rights reserved.</p>

<script>
    document.getElementById('year').textContent = new Date().getFullYear();
</script>
```

### Add Google Analytics:
```html
<!-- Add before </head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-GA-ID"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'YOUR-GA-ID');
</script>
```

## 📧 Contact Form Integration

The current forms are **UI-only**. To make them functional:

### Option 1: Formspree (Easy)
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <!-- Your existing form fields -->
</form>
```

### Option 2: Google Forms (Free)
1. Create a Google Form
2. Get the form embed code
3. Replace existing form

### Option 3: EmailJS (No backend needed)
Add to your form:
```javascript
<script src="https://cdn.emailjs.com/dist/email.min.js"></script>
<script>
    emailjs.init("YOUR_USER_ID");
    // Send email on form submit
</script>
```

## 🐛 Troubleshooting

**Problem: Animations not working**
- Check browser console for errors
- Ensure AOS library is loading (check network tab)
- Clear browser cache

**Problem: Images not loading**
- Verify image URLs are correct
- Check if images are accessible
- Try using relative paths for local images

**Problem: Mobile view broken**
- Check viewport meta tag is present
- Test responsive classes work
- Use browser DevTools mobile emulator

**Problem: Slow loading**
- Compress images
- Use WebP format
- Enable browser caching
- Consider using CDN for images

## 🤝 Contributing

Want to improve this website? Contributions are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - feel free to use it for your hotel, modify it, or learn from it!

## 🙏 Acknowledgments

- **Tailwind CSS** - For the amazing utility-first framework
- **AOS Library** - For smooth scroll animations
- **Unsplash** - For placeholder images (replace with your own!)
- **Google Fonts** - For beautiful typography

## 📞 Support

Need help customizing this website?

- 📧 Open an issue on GitHub
- 💬 Check existing issues for solutions
- 📖 Read Tailwind CSS docs: https://tailwindcss.com/docs

## 🗺️ Roadmap

Potential future enhancements:
- [ ] Multi-language support (Hindi/English)
- [ ] Online booking integration
- [ ] Blog section
- [ ] Virtual tour with 360° images
- [ ] Live availability calendar
- [ ] Payment gateway integration
- [ ] Admin dashboard
- [ ] Guest review system

---

**Made with ❤️ for spiritual travelers and hotel owners in Haridwar**

*If you find this useful, please ⭐ star the repository!*

---

### Quick Links:
- [View Live Demo](#) (Update with your GitHub Pages URL)
- [Report Bug](https://github.com/AbhixGupta/hotelwebsite/issues)
- [Request Feature](https://github.com/AbhixGupta/hotelwebsite/issues)

### Version History:
- **v1.0.0** (June 2026) - Initial release with three versions
  - Clean modern design
  - Animated Wix-style version
  - Artistic watercolor version with cultural elements
