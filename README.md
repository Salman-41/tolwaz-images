# Tolwaz Images CDN

A dedicated repository for hosting image assets for the Tolwaz commercial website via jsDelivr CDN.

## 🚀 Quick Start

Access any image through jsDelivr CDN using the following URL pattern:

```
https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/{category}/{filename}
```

## 📁 Directory Structure

```
dist/images/
├── logos/          # Brand logos and identity assets
├── icons/          # UI icons and symbols
├── banners/        # Marketing banners and hero images
├── products/       # Product images and galleries
└── ui/            # User interface elements
```

## 💻 Usage Examples

### HTML Integration

```html
<!-- Logo -->
<img src="https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/logos/logo.png" 
     alt="Tolwaz Logo" 
     loading="lazy">

<!-- Hero Banner -->
<img src="https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/banners/hero-banner.jpg" 
     alt="Hero Banner" 
     loading="lazy">

<!-- Product Image -->
<img src="https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/products/product-001.jpg" 
     alt="Product" 
     loading="lazy">
```

### CSS Background Images

```css
.hero-section {
  background-image: url('https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/banners/hero-banner.jpg');
  background-size: cover;
  background-position: center;
}

.logo {
  background-image: url('https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/logos/logo.png');
}
```

### JavaScript/React

```javascript
// React component
const Logo = () => (
  <img 
    src="https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/logos/logo.png"
    alt="Tolwaz Logo"
    loading="lazy"
  />
);

// Vanilla JavaScript
const logoUrl = 'https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/logos/logo.png';
document.getElementById('logo').src = logoUrl;
```

## 🏷️ Version Management

### Using Specific Versions
For production stability, use specific version tags:

```html
<!-- Using a specific version -->
<img src="https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@v1.0.0/dist/images/logos/logo.png">

<!-- Using latest version (auto-updates) -->
<img src="https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@latest/dist/images/logos/logo.png">
```

### Version Tags
- `@latest` - Always points to the most recent version
- `@v1.0.0` - Specific version for production use
- `@main` - Latest commit on main branch (not recommended for production)

## 🌐 CDN Benefits

- **Global Distribution**: jsDelivr provides worldwide CDN coverage
- **High Performance**: Optimized delivery with caching
- **No Bandwidth Costs**: Free CDN hosting via GitHub + jsDelivr
- **Version Control**: All images are version-controlled with Git
- **HTTPS Support**: Secure delivery by default
- **High Availability**: 99.9% uptime guarantee

## 📊 Performance Optimization

### Recommended Practices

1. **Use appropriate image formats**:
   - JPG for photographs
   - PNG for images with transparency
   - SVG for scalable graphics
   - WebP for modern browsers

2. **Optimize file sizes**:
   - Compress images before uploading
   - Use responsive images with different sizes
   - Implement lazy loading

3. **Cache Strategy**:
   - Use specific version tags for long-term caching
   - Update versions when images change

## 🔄 Adding New Images

1. Clone this repository
2. Add images to appropriate `dist/images/` subdirectory
3. Commit and push changes
4. Create a new release tag for version control
5. Update your website to use the new CDN URLs

## 📝 Naming Conventions

- Use lowercase filenames
- Use hyphens for spaces (`hero-banner.jpg`)
- Include descriptive names (`product-category-item.jpg`)
- Add size suffixes when needed (`logo-small.png`, `banner-mobile.jpg`)

## 🛡️ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For questions or issues related to this CDN repository, please [open an issue](https://github.com/Salman-41/tolwaz-images/issues).

---

**Note**: This repository is optimized for jsDelivr CDN delivery. All images should be placed in the `dist/images/` directory to ensure proper CDN access.