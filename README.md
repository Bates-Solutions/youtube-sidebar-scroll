<a href="https://bates-solutions.com/?utm_source=github&utm_medium=readme&utm_campaign=youtube-sidebar-scroll">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/readme-banner-dark.svg">
    <img src=".github/assets/readme-banner-light.svg" alt="Sidebar Scroll for YouTube, by Bates Solutions" width="100%">
  </picture>
</a>

# Sidebar Scroll for YouTube

A Chrome extension that scrolls YouTube's recommended videos without scrolling the video out of view.

[![License: MIT](https://img.shields.io/github/license/Bates-Solutions/youtube-sidebar-scroll)](LICENSE)

On a YouTube watch page, the recommendations column gets its own scrollbar, so you can keep
watching while you browse what's next. It is a single stylesheet: no JavaScript and no
permissions.

## Features

- Hover over the recommendations and scroll: only the list moves.
- Hover over the video or comments and scroll: the page scrolls as normal.
- Reaching the end of the list doesn't scroll the page.
- Only applies in the side-by-side layout. Narrow windows are untouched.

## Install

It isn't in the Chrome Web Store yet. To install it from source:

1. Download this repo (**Code**, then **Download ZIP**) and unzip it, or `git clone` it.
2. Open `chrome://extensions` and turn on **Developer mode** (top right).
3. Choose **Load unpacked** and select the folder.
4. Refresh any open YouTube tabs.

It works in any Chromium browser: Chrome, Edge, Brave and others.

## How it works

`styles.css` makes the recommendations column (`#secondary`) sticky, caps its height to the
viewport, and gives it its own scrollbar, with `overscroll-behavior: contain` so reaching the end
of the list doesn't scroll the page.

## Limitations

- If YouTube changes its page structure, the stylesheet may stop matching. Please open an issue if
  it does.
- Not affiliated with or endorsed by YouTube or Google.

## Privacy

The extension collects, stores and sends no data. It only adds a stylesheet to youtube.com.

## Security

Please report a vulnerability privately, as described in
[SECURITY.md](https://github.com/Bates-Solutions/.github/blob/main/SECURITY.md). Don't open a
public issue for it.

## Contributing

Contributions are welcome. See
[CONTRIBUTING.md](https://github.com/Bates-Solutions/.github/blob/main/CONTRIBUTING.md) and the
[code of conduct](https://github.com/Bates-Solutions/.github/blob/main/CODE_OF_CONDUCT.md).

## License

[MIT](LICENSE).

---

<a href="https://bates-solutions.com/?utm_source=github&utm_medium=readme&utm_campaign=youtube-sidebar-scroll">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Bates-Solutions/.github/main/brand/bates-solutions-on-dark.svg">
    <img src="https://raw.githubusercontent.com/Bates-Solutions/.github/main/brand/bates-solutions-on-light.svg" alt="Bates Solutions" width="160">
  </picture>
</a>

Made by [Bates Solutions](https://bates-solutions.com/?utm_source=github&utm_medium=readme&utm_campaign=youtube-sidebar-scroll).
