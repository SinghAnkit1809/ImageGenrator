# 🎨 Free AI Image Generator

Create stunning AI images instantly with our free, no-login-required image generator powered by Pollinations.ai.

## ✨ Features

- 🆓 **100% Free** - Unlimited image generation
- ⚡ **Lightning Fast** - Generate images in seconds
- 🎯 **Multiple AI Models** - Flux, Turbo, Anime, 3D, and more
- 🎨 **Style Options** - 12+ artistic styles to choose from
- 📐 **Aspect Ratios** - 8 different aspect ratios (Square, Landscape, Portrait, etc.)
- 🔒 **No Login Required** - Start creating immediately
- ✨ **AI Prompt Enhancement** - Enhance your prompts with AI
- 💾 **Download Support** - Save your creations easily

## 🚀 Deploying to Cloudflare Pages via GitHub

### Step-by-Step Guide

#### 1. Push Your Code to GitHub

```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - Free AI Image Generator"

# Add your GitHub repository
git remote add origin https://github.com/yourusername/your-repo-name.git

# Push to GitHub
git push -u origin main
```

#### 2. Connect to Cloudflare Pages

1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com/)
2. Navigate to **Pages** → **Create a project**
3. Click **"Connect to Git"**
4. Select **GitHub** and authorize Cloudflare
5. Select your repository

#### 3. Configure Build Settings

**IMPORTANT:** Use these exact settings:

```
Framework preset: None
Build command: (leave empty or use: echo "No build required")
Build output directory: /
Root directory: (leave empty)
Branch: main (or your default branch)
```

#### 4. Environment Variables (Optional)

No environment variables are required for this project.

#### 5. Deploy!

Click **Save and Deploy**. Your site will be live in ~1 minute!

### 🔧 Cloudflare Pages Configuration

The key settings in your Cloudflare Pages dashboard should be:

| Setting | Value |
|---------|-------|
| **Build command** | *(empty)* or `echo "No build required"` |
| **Build output directory** | `/` |
| **Root directory** | *(empty)* |
| **Node version** | Any (not used) |

### ✅ What to Push to GitHub

Make sure these files are in your repository:

- ✅ `index.html` (main file)
- ✅ `wrangler.toml` (Cloudflare config)
- ✅ `package.json` (project metadata)
- ✅ `_headers` (security headers)
- ✅ `README.md` (documentation)
- ✅ `.gitignore` (git ignore rules)

### 🐛 Troubleshooting GitHub Deployment

**Error: "Missing entry-point to Worker script"**

This happens when Cloudflare tries to build a Worker instead of a static site.

**Solution:**
1. In Cloudflare Pages dashboard
2. Go to **Settings** → **Builds & deployments**
3. Set **Build command** to empty or `echo "Static site"`
4. Set **Build output directory** to `/`
5. Retry deployment

**Error: "Build failed"**

If you see any build errors:
1. Make sure **Build command** is empty
2. Set **Build output directory** to `/` (just a forward slash)
3. Don't select any framework preset

### 🔄 Auto-Deploy on Push

Once connected, Cloudflare Pages will automatically deploy whenever you push to your main branch!

```bash
# Make changes to index.html
git add .
git commit -m "Updated design"
git push

# Cloudflare automatically deploys! 🚀
```

## 📁 File Structure

```
.
├── index.html          # Main application file
├── wrangler.toml       # Cloudflare configuration
├── package.json        # Node package configuration
├── _headers            # HTTP headers for security
└── README.md           # This file
```

## 🔧 Configuration

The site is pre-configured and ready to deploy. No additional setup required!

### Cloudflare Pages Settings

- **Framework preset**: None (Static HTML)
- **Build command**: (empty)
- **Build output directory**: `/`
- **Root directory**: `/`

## 🎯 SEO Optimization

The site is optimized for these high-volume, low-competition keywords:

- Free AI image generator
- AI art generator free
- Free image generator online
- Create AI images free
- Text to image generator
- AI picture generator free

## 🌐 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## 📝 License

MIT License - Feel free to use and modify!

## 🤝 Support

If you encounter any issues:

1. Check the browser console for errors
2. Ensure you have a stable internet connection
3. Try a different browser
4. Clear browser cache

## 🎨 Customization

To customize the site:

1. Edit `index.html` for content changes
2. Modify CSS variables in the `<style>` section for colors/themes
3. Update meta tags for SEO customization
4. Change default prompts in the JavaScript section

## 🚀 Performance

- Lightweight: Single HTML file (~30KB)
- No external dependencies
- Fast loading times
- Optimized images
- Cached assets

---

Made with ❤️ using Pollinations.ai API