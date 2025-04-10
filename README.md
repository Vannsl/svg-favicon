# SVG Favicon Color Modes

This is a simple HTML test demonstrating **dark mode support for SVG favicons** using CSS media queries inside the SVG. It also visually shows the effect with an inline SVG in the page body.

## 🧪 How It Works

The favicon (`favicon.svg`) includes embedded CSS that changes colors based on the user's system color scheme (light or dark mode). This is achieved via the `prefers-color-scheme` media query inside the SVG.

```css
@media (prefers-color-scheme: dark) {
  .favicon-fill {
    fill: black;
  }

  .favicon-stroke {
    stroke: white;
  }
}

You’ll also see the SVG rendered inline on the page for comparison/testing.

## 🧭 Browser Support

### ✅ Works In:

* __Chrome__  
  You might need to refresh the browser tab to see the effect of switching between light and dark mode.
* __Firefox__  
  Works without refreshing the tab during testing. Updates dynamically with color scheme changes.

#### ❌ Does Not Work In:

* __Safari__  
  As of now, Safari does not support SVG favicons. This means the dark mode adaptation will not appear in the tab icon.

You can check support status here:
👉 [Can I use SVG favicons](https://caniuse.com/link-icon-svg)