# shivanykshenoy.github.io

Personal GitHub Pages site — portfolio and resume.

**Live site:** https://shivanykshenoy.github.io

## Stack

- [Bootstrap 5.3](https://getbootstrap.com/) — layout and styling
- [Mustache.js 4.2](https://github.com/janl/mustache.js) — logicless templating
- No build step, no framework

## Structure

```
index.html        # Portfolio / home page
main.json         # Content for index.html (cards, links, bio)
resume/
  v1.html         # Resume page
  resume.json     # Content for v1.html (experience, skills, etc.)
```

## Updating content

- **Portfolio cards** → edit `main.json`
- **Resume** → edit `resume/resume.json`
- No HTML changes needed for content updates

## Local dev

Requires an HTTP server (plain `file://` won't work due to `fetch()`):

```bash
npx http-server .
# or
python3 -m http.server
```

Then open http://localhost:8080
