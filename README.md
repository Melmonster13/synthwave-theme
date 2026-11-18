# synthwave-theme

A synthwave / 80s Jekyll theme for GitHub Pages: midnight purple, sunset-gradient title, neon pink and cyan accents, and a unicorn chess knight. It's built on GitHub's [Primer](https://github.com/pages-themes/primer) theme, so Markdown and READMEs stay as readable as on github.com.

## Use it

Add a `_config.yml` to the repo (or folder) your Pages site builds from:

```yaml
title: My Project
remote_theme: Melmonster13/synthwave-theme
plugins:
  - jekyll-remote-theme
```

Then in **Settings → Pages**, publish from your branch. The first build can take a minute or two to appear.

## What you get

- **Brand bar** on every page: the unicorn-knight logo and your `title` in a sunset gradient.
- **Dark, readable Markdown**: cyan headings, pink links, dark code panels, and tables that scroll inside their own box on small screens.
- **Mermaid diagrams** rendered from ` ```mermaid ` blocks, in matching neon colours. (github.com renders these itself; plain Pages doesn't.)
- **Favicon** and home-screen icon.
- A small **`=^..^=` sign-off** at the bottom of each page.

## Options

```yaml
synthwave:
  hide_home_title: false   # default true: hides the home page's first heading,
                           # since a README usually repeats the site title
```

## Customising a site

- Add `_includes/head-custom.html` to a site for extra `<head>` tags (analytics, meta). The theme's own fonts, favicon and diagram script live in a separate include, so they keep working.
- Add `assets/css/style.scss` to a site to append your own styles:

  ```scss
  ---
  ---
  @import "jekyll-theme-primer";
  @import "synthwave";
  // your styles here
  ```

## License

The theme code is MIT-licensed; the layouts and base styles come from Primer (MIT, © GitHub, Inc.). The unicorn-knight logo is not covered by the MIT license. See [LICENSE](LICENSE).
