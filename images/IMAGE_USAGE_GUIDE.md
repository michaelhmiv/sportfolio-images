# Image Usage Guide

This guide explains how to upload images to this repository and use them across various platforms like social media, websites, and applications.

## How to Upload Images

### Method 1: Via GitHub Web Interface

1. Navigate to the `/images` folder in this repository
2. Click the **"Add file"** button, then select **"Upload files"**
3. Drag and drop your image files or click **"choose your files"** to browse
4. Add a descriptive commit message (e.g., "Add profile photo for basketball portfolio")
5. Click **"Commit changes"** to upload

### Method 2: Via Git Command Line

```bash
# Clone the repository (if you haven't already)
git clone https://github.com/michaelhmiv/sportfolio-images.git
cd sportfolio-images

# Add your images to the images folder
cp /path/to/your/image.jpg images/

# Commit and push
git add images/image.jpg
git commit -m "Add new image"
git push origin main
```

## Getting Raw GitHub URLs

Once your image is uploaded, you can access it directly using GitHub's raw content URL. This URL can be used anywhere that accepts image links.

### Raw URL Format

```
https://raw.githubusercontent.com/USERNAME/REPOSITORY/BRANCH/PATH/FILENAME.EXT
```

### Example URLs

For this repository (`sportfolio-images`):

```
https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/profile-photo.jpg
https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/basketball-action.png
https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/team-logo.svg
```

### How to Construct Your Raw URL

1. **Base URL**: `https://raw.githubusercontent.com/`
2. **Username**: `michaelhmiv`
3. **Repository**: `sportfolio-images`
4. **Branch**: `main` (or another branch if specified)
5. **Path**: `images/` (or subdirectory within images/)
6. **Filename**: Your exact filename with extension

**Complete Example:**
```
https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/my-image.jpg
```

## Using Your Images

Once you have the raw GitHub URL, you can use it in:

### Social Media
- **Twitter/X**: Paste the URL when creating a post
- **LinkedIn**: Use in articles or posts that support external images
- **Discord/Slack**: Paste the URL to embed images in messages

### Websites and Web Applications
```html
<!-- HTML -->
<img src="https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/profile-photo.jpg" alt="Profile Photo">
```

```markdown
<!-- Markdown -->
![Profile Photo](https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/profile-photo.jpg)
```

### React/JavaScript Applications
```javascript
const imageUrl = 'https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/profile-photo.jpg';

<img src={imageUrl} alt="Profile Photo" />
```

### CSS Background Images
```css
.hero-section {
  background-image: url('https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/background.jpg');
}
```

## Best Practices

1. **Use descriptive filenames**: Instead of `IMG_1234.jpg`, use `basketball-game-2026-01-03.jpg`
2. **Organize with subdirectories**: Create folders like `images/profiles/`, `images/events/`, etc.
3. **Optimize image sizes**: Compress images before uploading to reduce load times
4. **Supported formats**: JPG, PNG, GIF, SVG, WebP, and most common image formats
5. **File naming**: Avoid spaces in filenames; use hyphens (`-`) or underscores (`_`) instead
6. **Keep it public**: This repository must remain public for raw URLs to work without authentication

## Quick Reference

| Component | Value |
|-----------|-------|
| Username | `michaelhmiv` |
| Repository | `sportfolio-images` |
| Default Branch | `main` |
| Images Directory | `images/` |
| Raw URL Template | `https://raw.githubusercontent.com/michaelhmiv/sportfolio-images/main/images/YOUR-IMAGE.ext` |

## Troubleshooting

**Image not loading?**
- Verify the filename matches exactly (including case sensitivity)
- Ensure the image was successfully committed to the repository
- Check that the branch name is correct (usually `main`)
- Confirm the repository is public

**Need to update an image?**
- You can upload a new file with the same name, and it will replace the old one
- The raw URL will remain the same, so all your links will automatically show the new image

## Need Help?

If you encounter any issues or have questions about image hosting, check the [GitHub Documentation](https://docs.github.com/en/repositories/working-with-files) or open an issue in this repository.