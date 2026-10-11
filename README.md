# Halal Growth Blog — setup notes

## 1. Add these files to your existing repo
Copy the whole `blog/` folder into the root of your
`irshadakhan-halalgrowth.github.io` repository, next to your existing
`index.html`. Final layout should look like:

```
irshadakhan-halalgrowth.github.io/
├── index.html          (your existing homepage — unchanged)
├── blog/
│   ├── index.html       (blog listing page)
│   ├── assets/
│   │   └── blog.css
│   └── posts/
│       └── sample-post.html
```

Commit and push — GitHub Pages will serve it automatically at
`https://irshadakhan-halalgrowth.github.io/blog/`.

## 2. Link to it from your homepage
Add a nav link on your existing `index.html` pointing to `blog/index.html`
(e.g. next to Resources / Contact), so visitors can find it.

## 3. Publishing a new post
1. Duplicate `blog/posts/post-template.html`, rename it to match the topic
   (e.g. `credit-score-repair.html`). Your first real post,
   `understanding-murabaha.html`, is already written and live in the
   listing — use it as a second reference for tone and structure.
2. Edit the `<title>`, `<meta name="description">`, category, date, `<h1>`,
   and body paragraphs.
3. Update the `cta-box` link if the post should point to a different
   Gumroad product.
4. Add a matching `<article class="post-row">` block to `blog/index.html`,
   above the existing entries (newest first), linking to your new file.
5. Commit and push.

## 4. SEO basics for each post
- Keep the `<title>` under ~60 characters, `<meta name="description">`
  under ~155 characters — both should include your target keyword.
- Use one `<h1>` per post (already handled by the template) and `<h2>`
  for subheadings.
- Link each new post back to at least one Gumroad product and, where
  relevant, to an earlier post.

## Notes
- No build tools required — these are plain HTML/CSS files, consistent
  with how your homepage is built.
- Colors and fonts (navy / gold / green, Newsreader + Inter) live in
  `blog/assets/blog.css` — change them there once and every post updates.
