# Contributing to Tolwaz Images CDN

Thank you for your interest in contributing to the Tolwaz Images CDN repository!

## Adding New Images

### Guidelines

1. **File Formats**: Use appropriate formats for different types of images:
   - **JPG**: For photographs and complex images
   - **PNG**: For images with transparency or simple graphics
   - **SVG**: For scalable vector graphics and icons
   - **WebP**: For modern browsers (provide fallbacks)

2. **File Naming**: Use descriptive, lowercase names with hyphens:
   - ✅ `hero-banner.jpg`
   - ✅ `product-laptop-001.png`
   - ✅ `logo-white-small.svg`
   - ❌ `Image1.JPG`
   - ❌ `banner_hero.png`

3. **File Sizes**: Optimize images before uploading:
   - Compress images to reduce file sizes
   - Consider multiple sizes for responsive design
   - Aim for web-optimized quality

4. **Directory Structure**: Place files in appropriate directories:
   - `dist/images/logos/` - Brand logos
   - `dist/images/icons/` - UI icons
   - `dist/images/banners/` - Marketing banners
   - `dist/images/products/` - Product images
   - `dist/images/ui/` - UI elements

### Process

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Salman-41/tolwaz-images.git
   cd tolwaz-images
   ```

2. **Add your images** to the appropriate directory in `dist/images/`

3. **Test the CDN URLs** using the jsDelivr format:
   ```
   https://cdn.jsdelivr.net/gh/Salman-41/tolwaz-images@main/dist/images/{category}/{filename}
   ```

4. **Commit your changes**:
   ```bash
   git add dist/images/
   git commit -m "Add new images for [category/purpose]"
   ```

5. **Create a pull request** with a description of the images added

## Version Management

### Creating Releases

1. Update `CHANGELOG.md` with new additions
2. Update version in `package.json`
3. Create a new release tag:
   ```bash
   git tag v1.x.x
   git push origin main --tags
   ```

### Using Versions

- **Development**: Use `@main` for testing
- **Production**: Use specific version tags like `@v1.0.0`
- **Auto-update**: Use `@latest` for automatic updates

## Image Optimization Tips

### Recommended Tools
- **TinyPNG**: For PNG compression
- **JPEGmini**: For JPEG optimization
- **SVGO**: For SVG optimization
- **ImageOptim**: For batch optimization

### Best Practices
- Compress images before uploading
- Use appropriate dimensions for intended use
- Consider providing multiple sizes
- Test on different devices and connections

## Questions or Issues?

If you have questions about contributing or encounter any issues:

1. Check existing [issues](https://github.com/Salman-41/tolwaz-images/issues)
2. Create a new issue with detailed information
3. Contact the repository maintainers

Thank you for helping improve the Tolwaz Images CDN!