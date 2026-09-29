# Sidebar Scroll for YouTube

A tiny Chrome extension that lets you scroll the list of recommended videos on a YouTube watch page **without scrolling the video out of view** — so you can keep watching while you browse what's next.

- Hover over the recommendations and scroll: only the list moves.
- Hover over the video or comments and scroll: the page scrolls as normal.
- Only applies in the side-by-side layout; narrow windows are untouched.

It's a single CSS file — no JavaScript, no permissions, no data collected.

## Install

### From the Chrome Web Store
_Coming soon._

### Manually (developer mode)
1. Download this repo (**Code → Download ZIP**) and unzip it, or `git clone` it.
2. Open `chrome://extensions` and turn on **Developer mode** (top right).
3. Click **Load unpacked** and select the folder.
4. Refresh any open YouTube tabs.

Works in any Chromium browser (Chrome, Edge, Brave, etc.).

## How it works

`styles.css` makes the recommendations column (`#secondary`) sticky, caps its height to the viewport, and gives it its own scrollbar, with `overscroll-behavior: contain` so reaching the end of the list doesn't scroll the page.

If YouTube changes its page structure and this stops working, please open an issue.

## Privacy

This extension does not collect, store, or transmit any data. It only injects a stylesheet on youtube.com.

Not affiliated with or endorsed by YouTube or Google.

## License

MIT
