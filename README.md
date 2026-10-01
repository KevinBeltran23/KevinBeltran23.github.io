# Kevin Beltran - Personal Website

A clean, dark-themed personal site inspired by [gitfolio](https://github.com/imfunniee/gitfolio).

## Structure

```
index.html          - Main page (profile sidebar + projects + blog)
styles.css          - All styling
blog.json           - Blog post registry (drives the blog section)
blog/               - Blog post folders
  hello-world/
    index.html      - Individual blog post
    cover.jpg       - Optional cover image
KevinBeltran_Resume.pdf - Resume for download
ProfilePicture.jpg  - Profile photo
```

## How to Add a Blog Post

1. **Create a folder** in `blog/` with a URL-friendly name (e.g., `blog/my-new-post/`)
2. **Add an `index.html`** inside it (copy from `blog/hello-world/index.html` as a template)
3. **Optionally add a cover image** (e.g., `cover.jpg`) in the same folder
4. **Register it in `blog.json`**:

```json
{
  "url_title": "my-new-post",
  "title": "My New Post Title",
  "sub_title": "A short description of the post",
  "top_image": "cover.jpg",
  "date": "June 2025"
}
```

If you don't have a cover image, set `"top_image": ""` or remove the field.

## How to Add/Edit Experience or Projects

Open `index.html` and find the `<!-- ADD EXPERIENCE / PROJECTS HERE -->` comment. Copy an existing `<section>` block into the `Experience.` or `Projects.` grid and update it:

```html
<section>
  <div class="card_head">
    <div class="section_title">Company or Project</div>
    <div class="date">Sep 2025 – May 2026</div>
  </div>
  <div class="role">Role</div>
  <div class="about_section">One or two sentences on impact.</div>
  <div class="tags"><span>React</span><span>Node.js</span></div>
  <div class="links">
    <a href="https://github.com/..." target="_blank" rel="noopener"><i class="fab fa-github"></i> Code</a>
    <a href="https://..." target="_blank" rel="noopener"><i class="fas fa-external-link-alt"></i> Live Demo</a>
  </div>
</section>
```

Remove the `.links` div if there is nothing public to link to.

## How to Update Contact Info

Edit the `#profile` section in `index.html`. All contact info is in the left sidebar.

## How to Update Resume

Replace `KevinBeltran_Resume.pdf` with the new file (keep the same filename).
