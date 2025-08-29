# 🛠️ Development Guide - Hindu YUVA Website

## 🚀 Quick Start Development

### 1. Initial Setup

```bash
# Install Node.js dependencies
npm install

# Start development server with live reload
npm run dev
```

### 2. Real-Time Development Workflow

1. **Start Development Server**
   ```bash
   npm run dev
   ```
   - Opens browser automatically at `http://localhost:3000`
   - Live reload enabled - changes appear instantly
   - Watches all files for changes

2. **Make Changes**
   - Edit any HTML, CSS, or JS file
   - Save the file
   - Browser automatically refreshes
   - See changes immediately

3. **Test Changes**
   - Test on different screen sizes
   - Check all pages work correctly
   - Verify navigation and links

## 📁 File Structure & Development

### Core Files
- `home.html` - Main homepage (entry point)
- `aboutus.html` - About page
- `events.html` - Events listing
- `gallery.html` - Photo gallery
- `resources.html` - Resources hub
- `temple.html` - Temple directory
- `academic.html` - Academic resources
- `career.html` - Career resources

### Styling & Scripts
- `styles.css` - All CSS styles
- `script.js` - JavaScript functionality
- `index.html` - Redirect to home

### Configuration
- `package.json` - Project settings
- `vercel.json` - Deployment config
- `.gitignore` - Git ignore rules

## 🎨 Development Best Practices

### HTML Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title - Hindu YUVA</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <!-- Navigation content -->
    </nav>
    
    <!-- Main content -->
    <main>
        <!-- Page content -->
    </main>
    
    <!-- Footer -->
    <footer>
        <!-- Footer content -->
    </footer>
    
    <script src="script.js"></script>
</body>
</html>
```

### CSS Organization
```css
/* Reset and base styles */
* { /* ... */ }

/* Layout components */
.container { /* ... */ }
.navbar { /* ... */ }

/* Page-specific styles */
.hero { /* ... */ }
.about { /* ... */ }

/* Responsive design */
@media (max-width: 768px) { /* ... */ }
```

### JavaScript Structure
```javascript
// DOM ready
document.addEventListener('DOMContentLoaded', function() {
    // Initialize components
    initNavigation();
    initGallery();
    initForms();
});

// Component functions
function initNavigation() {
    // Navigation logic
}
```

## 🔄 Real-Time Development Tips

### 1. Live Reload
- Server automatically detects file changes
- Browser refreshes instantly
- No manual refresh needed

### 2. Cross-Browser Testing
- Test in Chrome, Firefox, Safari, Edge
- Check mobile responsiveness
- Verify all features work

### 3. Performance Testing
- Use browser dev tools
- Check loading times
- Optimize images and assets

### 4. Accessibility Testing
- Use screen readers
- Check keyboard navigation
- Verify color contrast

## 🚀 Deployment Workflow

### 1. Development Phase
```bash
npm run dev          # Start development
# Make changes...
# Test changes...
# Repeat...
```

### 2. Preview Phase
```bash
npm run preview      # Preview on port 3001
# Final testing before deployment
```

### 3. Deployment Phase
```bash
npm run build        # Prepare for deployment
# Push to GitHub
# Deploy to Vercel/Netlify
```

## 📱 Responsive Development

### Breakpoints
- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

### Testing Strategy
1. Start with mobile design
2. Scale up to tablet
3. Finalize desktop version
4. Test all breakpoints

## 🎯 Development Commands

| Command | Purpose |
|---------|---------|
| `npm run dev` | Start development server |
| `npm start` | Alias for dev command |
| `npm run preview` | Preview build |
| `npm run build` | Prepare for deployment |
| `npm run deploy` | Ready for deployment |

## 🔧 Troubleshooting

### Common Issues

1. **Port already in use**
   ```bash
   # Kill process on port 3000
   npx kill-port 3000
   npm run dev
   ```

2. **Live reload not working**
   - Check file permissions
   - Restart development server
   - Clear browser cache

3. **Styles not updating**
   - Hard refresh browser (Ctrl+F5)
   - Check CSS syntax
   - Verify file paths

4. **Navigation issues**
   - Check file names match links
   - Verify all HTML files exist
   - Test all internal links

## 📊 Development Tools

### Recommended Extensions (VS Code)
- Live Server
- HTML CSS Support
- JavaScript (ES6) code snippets
- Auto Rename Tag
- Bracket Pair Colorizer

### Browser Dev Tools
- Chrome DevTools
- Firefox Developer Tools
- Safari Web Inspector

## 🚀 Next Steps

1. **Start Development**
   ```bash
   npm run dev
   ```

2. **Make Your First Change**
   - Edit `home.html`
   - Save the file
   - See changes instantly

3. **Test Everything**
   - Navigate all pages
   - Test responsive design
   - Check all functionality

4. **Deploy When Ready**
   - Push to GitHub
   - Deploy to Vercel/Netlify
   - Share with community

---

**Happy Coding! 🕉️**
