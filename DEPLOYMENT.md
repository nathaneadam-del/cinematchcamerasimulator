# Magic Hour: Camera Simulator — Deployment Guide

## Folder Structure for Netlify

Your final project folder should look like this:

```
your-project/
├── index.html          (the main game file)
├── images.json         (manifest listing all image paths)
└── images/
    ├── image-01.jpg
    ├── image-02.jpg
    ├── image-03.jpg
    │ ... (up to 50 images)
    └── image-50.jpg
```

## Setup Steps

### 1. Prepare Your Images

- Place your 50 images in an `images/` folder within your project
- Name them sequentially: `image-01.jpg`, `image-02.jpg`, etc. (or use any names you prefer)
- Supported formats: JPG, PNG, WebP, AVIF, GIF

### 2. Update images.json

Edit `images.json` and replace the placeholder paths with your actual image filenames:

**Example:**
```json
[
  "images/nyc-street-01.jpg",
  "images/nyc-street-02.jpg",
  "images/nyc-street-03.jpg",
  ...
]
```

The paths are relative to your site root. Each entry should be a path string like `"images/filename.jpg"`.

### 3. Deploy to Netlify

**Option A: Drag & Drop (Easiest)**
1. Go to [netlify.com/drop](https://app.netlify.com/drop)
2. Drag your entire project folder (containing index.html, images.json, and images/) onto the page
3. Your site is live immediately

**Option B: GitHub + Auto-Deploy**
1. Push your project to a GitHub repo
2. Connect the repo to Netlify
3. Netlify auto-deploys on every push

**Option C: Netlify CLI**
```bash
npm install -g netlify-cli
netlify deploy --prod --dir .
```

## How It Works

1. When students visit the site, `index.html` loads automatically
2. The page fetches `images.json` and loads all 50 images
3. Scenes are randomly assigned to images with generated descriptions
4. Scene edits are saved in the browser's localStorage (persists across sessions)

## Notes

- **localStorage is local to each browser**, so students' edits are private to them
- **No backend needed** — this is a static site with client-side storage
- If you update images or images.json, students should **clear their browser cache** or use a fresh browser session to see changes
- The manifest file must be valid JSON or the game will show a loading error

## Troubleshooting

**"Loading..." stays stuck**
- Check browser console (F12 → Console) for error messages
- Verify `images.json` is in the project root and has valid JSON
- Check that image paths in `images.json` match actual file paths

**Images won't load**
- Ensure image filenames match exactly in `images.json`
- Verify images are in the `images/` folder
- Check that paths use forward slashes: `images/name.jpg` (not backslashes)

**Students see different scenes on refresh**
- This is normal! Each image gets a random archetype and description on first load, then that config is cached in localStorage
- To reset, students can clear their browser cache or use a private/incognito window
