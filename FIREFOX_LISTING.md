# Firefox Add-ons listing: copy & answers

Paste these into the Firefox Add-ons Developer Hub (https://addons.mozilla.org/developers/) when you
submit a new add-on. Edit to taste.

## Upload

- **Where to list it:** On this site.
- **File:** the zip from `npx web-ext build --ignore-files "*.md"`. It needs `manifest.json` at the
  top level of the zip, which `web-ext build` does.
- **Platforms:** Firefox only. The manifest needs Firefox 140, and the Android build isn't supported
  (it needs Firefox for Android 142, and the layout it targets is desktop only).
- **Source code:** "Do you use any of the following in your extension: code generators,
  minifiers, template engines, transpilers?" Answer **No**: it is one hand-written stylesheet.

## Name (max 50 chars)

Sidebar Scroll for YouTube

## Add-on URL

youtube-sidebar-scroll

## Summary (max 250 chars)

Scroll the recommended videos on a YouTube watch page without scrolling the video out of view. The
recommendations column gets its own scrollbar. One stylesheet, no JavaScript.

## Description

On a YouTube watch page, scrolling down to browse what's next pushes the video you're watching
off the screen. This add-on gives the recommendations column its own scrollbar, so you can keep
watching while you browse.

- Hover over the recommendations and scroll: only the list moves.
- Hover over the video or comments and scroll: the page scrolls as normal.
- Reaching the end of the list doesn't scroll the page.
- Only applies in the side-by-side layout. Narrow windows are untouched.

It is a single stylesheet: no JavaScript, no tracking, and no access to anything beyond
www.youtube.com.

If the sidebar still scrolls with the page, check that the add-on is allowed to run on
www.youtube.com: in about:addons, open the add-on, then **Permissions**.

Not affiliated with or endorsed by YouTube or Google.

## Categories (up to 2)

- Appearance
- Photos, Music & Videos

## Tags

youtube

AMO tags come from a fixed list (`https://addons.mozilla.org/api/v5/addons/tags/`); `sidebar` and
`scroll` aren't on it.

## Support

- **Support website:** https://github.com/Bates-Solutions/youtube-sidebar-scroll/issues
- **Support email:** leave blank, or a team address.

## License

MIT License

## Privacy policy

Not needed: the add-on runs no code and stores nothing. The manifest declares
`data_collection_permissions: { required: ["none"] }`, so the listing says it collects no data.

## Notes to reviewer

The add-on is one CSS file (`styles.css`) injected on www.youtube.com at `document_start`. It
makes the recommendations column (`#secondary`) sticky with its own scroll in YouTube's two-column
watch layout (`ytd-watch-flexy[is-two-columns_]`). There is no JavaScript. To test it: open any
YouTube video in a wide window and scroll over the recommendations.

## Screenshots

None in the repo yet. Take one of a watch page scrolled partway down the recommendations, with
the video still in view (1280×800 is a good size).
