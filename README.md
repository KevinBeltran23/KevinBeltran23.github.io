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

## How to Add/Edit Projects

Open `index.html` and find the `<!-- ADD YOUR PROJECTS HERE -->` comment in the `#work_section` div. Copy an existing project block and update:

```html
<a href="https://github.com/kevinbeltran23/your-repo" target="_blank">
  <section>
    <div class="section_title">Project Name</div>
    <div class="about_section">Short description of the project</div>
    <div class="bottom_section">
      <span><i class="fas fa-code"></i> Tech Stack</span>
    </div>
  </section>
</a>
```

## How to Update Contact Info

Edit the `#profile` section in `index.html`. All contact info is in the left sidebar.

## How to Update Resume

Replace `KevinBeltran_Resume.pdf` with the new file (keep the same filename).
