# Bedella Plumbing - Luxury Plumbing Website

A professional, high-end single-page website for Bedella Plumbing, serving Kitchener, Ontario and surrounding areas.

## 🎨 Design Features

- **Brand Colors**: Deep Blue (#1a3a52) and Deep Red (#C41E3A)
- **Typography**: Playfair Display (headings) + Inter (body text)
- **Fully Responsive**: Mobile-first design optimized for all devices (320px - 1920px+)
- **Luxury Aesthetic**: Premium spacing, clean lines, and professional imagery
- **Smooth Animations**: Intersection Observer API for fade-in effects and smooth scrolling

## 📋 Page Sections

1. **Fixed Header/Navigation** - Company branding, menu, phone number, CTA button
2. **Hero Section** - Full-width background with overlay and dual CTAs
3. **About Section** - Company story, trust badges, local expertise
4. **Services Section** - 8 premium service cards with images and icons
5. **Why Us Section** - 4 key differentiators with gradient background
6. **Testimonials Section** - 5 customer reviews with star ratings
7. **Contact Form** - Netlify-powered quote request form
8. **Footer** - Contact info, hours, service areas, social links

## 🚀 Deploying to Netlify

### Method 1: Drag & Drop (Quickest)

1. Visit [Netlify Drop](https://app.netlify.com/drop)
2. Drag and drop the entire `Bedella-Plumbing` folder
3. Your site will be live in seconds with a random URL
4. Configure custom domain in Site Settings

### Method 2: Git Integration (Recommended)

1. Push this repository to GitHub
2. Log in to [Netlify](https://app.netlify.com/)
3. Click "Add new site" → "Import an existing project"
4. Connect to your GitHub repository
5. Configure build settings (leave blank for static site):
   - **Build command**: (leave empty)
   - **Publish directory**: `/` or `.`
6. Click "Deploy site"

### Method 3: Netlify CLI

```bash
# Install Netlify CLI globally
npm install -g netlify-cli

# Login to Netlify
netlify login

# Deploy from the project directory
cd Bedella-Plumbing
netlify deploy --prod
```

## 📧 Netlify Form Setup

The contact form is already configured for Netlify Forms with:

- `data-netlify="true"` attribute
- `data-netlify-honeypot="bot-field"` for spam protection
- Form name: `bedella-quote`

### Accessing Form Submissions

1. Go to your Netlify dashboard
2. Select your site
3. Navigate to **Forms** in the sidebar
4. View all form submissions with email notifications

### Setting Up Form Notifications

1. In Netlify dashboard → **Site Settings** → **Forms**
2. Click **Form notifications**
3. Add email notification to receive submissions at your email
4. Optional: Set up Slack, webhook, or other integrations

## 🛠️ Customization Guide

### Update Contact Information

Edit the following sections in `index.html`:

1. **Phone Number** (appears in multiple locations):
   - Line ~303: Navigation header
   - Line ~328: Hero section (tel: link)
   - Line ~987: Footer

2. **Email Address**:
   - Line ~996: Footer contact info

3. **Business Address**:
   - Line ~1000: Footer location

### Update Business Hours

Edit lines 1008-1014 in the footer section.

### Change Colors

Modify CSS variables at the top of the `<style>` section (lines 25-34):

```css
:root {
    --deep-blue: #1a3a52;
    --deep-red: #C41E3A;
    --dark-red: #8B0000;
    /* ... other colors */
}
```

### Replace Images

The site uses professional images from Unsplash. To use your own images:

1. Replace Unsplash URLs with your image paths
2. Update these sections:
   - Line 315: Hero background
   - Line 408: About section image
   - Lines 453-537: Service card images

### Add/Remove Services

Edit the services grid section (lines 445-580). Each service card follows this structure:

```html
<div class="service-card">
    <div class="service-image">
        <img src="IMAGE_URL" alt="SERVICE_NAME">
        <div class="service-icon">
            <i class="fas fa-ICON-NAME"></i>
        </div>
    </div>
    <div class="service-content">
        <h3>Service Title</h3>
        <p>Service description...</p>
    </div>
</div>
```

### Update Testimonials

Edit the testimonials section (lines 660-830). Modify customer names, initials, and review text.

## 📱 Responsive Breakpoints

- **Desktop**: 1200px+ (full layout)
- **Tablet**: 769px - 1199px (2-column grids)
- **Mobile**: 320px - 768px (stacked layout)

## ⚡ Performance Optimization

- Minimal external dependencies (only Google Fonts and Font Awesome)
- Embedded CSS and JavaScript for faster loading
- Optimized images from Unsplash CDN
- Lazy loading with Intersection Observer API
- Mobile-first responsive approach

## 🔍 SEO Features

- Semantic HTML5 structure
- Meta tags for description and keywords
- Proper heading hierarchy (H1 → H6)
- Alt text for all images
- Descriptive page title
- Clean URL structure with anchor links

## 🎯 Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 Files Structure

```
Bedella-Plumbing/
├── index.html          # Main website file (complete single-page site)
└── README.md          # This file
```

## 🔒 Security Features

- Netlify honeypot spam protection
- No sensitive data in frontend code
- HTTPS enabled by default on Netlify
- Form validation (client-side and Netlify-side)

## 💡 Pro Tips

1. **Custom Domain**: Configure in Netlify → Domain Settings → Add custom domain
2. **SSL Certificate**: Automatically provided by Netlify (Let's Encrypt)
3. **Analytics**: Add Netlify Analytics or Google Analytics for visitor tracking
4. **A/B Testing**: Use Netlify Split Testing for form optimization
5. **Performance**: Netlify automatically provides CDN and asset optimization

## 📞 Support

For questions about this website template:
- Review the inline code comments in `index.html`
- Check [Netlify Documentation](https://docs.netlify.com/)
- Refer to [Netlify Forms Guide](https://docs.netlify.com/forms/setup/)

## 📝 License

This website template is created for Bedella Plumbing. Customize as needed for your business.

---

**Built with ❤️ for Bedella Plumbing | Kitchener, Ontario**
