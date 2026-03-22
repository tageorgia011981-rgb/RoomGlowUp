# Room Glow Up

## Cursor Cloud specific instructions

This is a zero-dependency, static HTML/CSS/JS website. There are no build tools, package managers, frameworks, or backend services.

### Running the development server

Serve the repository root with any static HTTP server. The simplest option:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/index.html` in a browser.

### Key files

- `index.html` — main application (inline CSS + vanilla JS)
- `decor-test.html` — standalone test page for the Decor Closet image cycling feature
- `Assets/` — all image assets (PNG furniture/decor items, JPG room backgrounds and UI elements)

### Notes

- There is no linter, test runner, or build step configured in this project.
- The Google Fonts CDN (`Limelight` font) is loaded at runtime; the page still renders without internet but falls back to `serif`.
- Opening `index.html` via `file://` may cause CORS issues with image loading in some browsers; always use an HTTP server.
