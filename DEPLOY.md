# 🚀 Deploy to GitHub Pages

## Quick Setup (2 minutes)

### Step 1: Enable GitHub Pages
1. Go to your repository: https://github.com/AbhixGupta/hotelwebsite
2. Click on **Settings** (top navigation)
3. Click on **Pages** (left sidebar)
4. Under "Build and deployment":
   - **Source**: Select "Deploy from a branch"
   - **Branch**: Select "main" and "/ (root)"
   - Click **Save**

### Step 2: Wait for Deployment
- GitHub will automatically build and deploy your site (takes ~1-2 minutes)
- You'll see a message: "Your site is ready to be published at..."

### Step 3: Access Your Live Site
Your website will be available at:
```
https://abhixgupta.github.io/hotelwebsite/
```

## 📱 Which Version to Use as Default?

You have 3 versions in your repository:

1. **index.html** - Clean, simple version
2. **index-animated.html** - Animated version with smooth effects
3. **index-painted.html** - Mobile-optimized with Ganga Aarti background ⭐ **RECOMMENDED**

### To set a default homepage:

**Option A: Use the painted version (recommended)**
```bash
# In your hotelweb folder
cp index-painted.html index.html
git add index.html
git commit -m "Set mobile-optimized version as default homepage"
git push origin main
```

**Option B: Keep all versions accessible**
- Main site: `https://abhixgupta.github.io/hotelwebsite/`
- Animated: `https://abhixgupta.github.io/hotelwebsite/index-animated.html`
- Painted: `https://abhixgupta.github.io/hotelwebsite/index-painted.html`

## 🔧 Testing Before Going Live

Test your site on different devices:
- Desktop browser
- Mobile Chrome/Safari
- Tablet view

### Test Checklist:
- [ ] Hero image loads correctly
- [ ] Navigation menu works on mobile
- [ ] All buttons are clickable
- [ ] Forms display properly
- [ ] Images load on slow connections
- [ ] Text is readable on small screens

## 📊 After Deployment

### View Deployment Status
1. Go to your repo → **Actions** tab
2. You'll see "pages build and deployment" workflow
3. Green checkmark ✅ means successful deployment

### Custom Domain (Optional)
If you want to use your own domain (e.g., www.gangaheritage.com):
1. Settings → Pages → Custom domain
2. Enter your domain name
3. Update your domain's DNS settings to point to GitHub Pages

## 🐛 Troubleshooting

**Problem: Site not loading**
- Wait 2-3 minutes after enabling Pages
- Check Actions tab for deployment errors
- Clear browser cache and try again

**Problem: Images not showing**
- Check image URLs in the code
- Make sure images are accessible
- Try using relative paths for local images

**Problem: Mobile view looks broken**
- The painted version is optimized for mobile
- Test on actual device, not just browser resize
- Check viewport meta tag is present

## 🔄 Updating Your Live Site

After making changes to your website:
```bash
git add .
git commit -m "Your update message"
git push origin main
```

GitHub Pages will automatically update your site within 1-2 minutes.

## 💡 Pro Tips

1. **Test Locally First**
   ```bash
   # Start a local server
   python3 -m http.server 8000
   # Visit http://localhost:8000
   ```

2. **Use Browser DevTools**
   - Press F12 to open developer tools
   - Click device icon to test mobile view
   - Check console for errors

3. **Monitor Performance**
   - Use Google PageSpeed Insights: https://pagespeed.web.dev/
   - Compress images if site is slow
   - Use WebP format for better performance

## 📞 Need Help?

- GitHub Pages Docs: https://docs.github.com/en/pages
- Check repository Issues tab
- Verify all files are pushed to GitHub

---

**Your site will be live at:** https://abhixgupta.github.io/hotelwebsite/

After enabling GitHub Pages, wait 2 minutes and visit the URL! 🎉
