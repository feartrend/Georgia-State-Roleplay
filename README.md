# Georgia State Roleplay — Official Website

ERLC Law Enforcement Roleplay Community

## Pages

| File | URL | Access |
|------|-----|--------|
| `index.html` | `/` | Public — Home & Welcome |
| `leo.html` | `/leo.html` | Public — LEO SOP |
| `news.html` | `/news.html` | Public — News & Announcements |
| `training.html` | `/training.html` | **Staff Only** — Do not share link publicly |

## Hosting on GitHub Pages

1. Create a new GitHub repository (e.g. `gsr-site`)
2. Upload all files: `index.html`, `leo.html`, `news.html`, `training.html`, `style.css`
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch`
5. Choose `main` branch, `/ (root)` folder → click **Save**
6. Your site will be live at: `https://yourusername.github.io/gsr-site/`

## Training Page (Staff Only)

The training guide lives at `/training.html`. It is **not linked anywhere** in the public navigation. Share only via direct link in your private staff Discord channel.

## Updating News & Announcements

To add a new announcement, open `news.html` and copy this block inside the `<!-- MAIN FEED -->` section:

```html
<div class="ann-card">
  <div class="ann-card-top">
    <div class="ann-meta">
      <span class="ann-tag tag-update">Update</span>  <!-- tag-update / tag-policy / tag-general / tag-alert -->
      <span class="ann-date">Month Day, Year</span>
    </div>
    <div class="ann-title">Your Title Here</div>
    <div class="ann-body">
      Your announcement content here.
    </div>
  </div>
  <div class="ann-divider"></div>
  <div class="ann-footer">
    <div class="ann-author">Posted by <span>Your Name</span></div>
  </div>
</div>
```

To pin an announcement, add `style="border-color:rgba(200,168,75,.4);"` to the card and add `<span class="ann-pinned">Pinned</span>` inside `.ann-meta`.
