# CSS Rapid Prototyping

This bookmarklet creates a grid overlay to the page and allows for any text in the page to be modified for the sake of rapid prototyping.
It uses basic CSS and a base64 SVG, therefore it's very easy for anyone to customise it (disable the grid, add features, etc.).

I took the original idea from an 2011 article on [css-101.org](http://cssmojo.com/trick_for_rapid_prototyping/): I used to copy-paste that CSS to an open page with the **MyStyle** extension for Chrome, but then I thought it would have been quicker to create this bookmarklet.

Later the same year, I found out that someone else had the same idea, and had also added a useful on/off functionality. You can still check that out: [grid.js](https://gist.github.com/webxl/1232664).

If you still want to try this version 0.1 of the bookmarklet, download `cssprototyping.js` and host it somewhere, then edit the url in `css-rapid-prototyping` accordingly. You can then create a new bookmark in Chrome and copy the code as the URL associated with the bookmark.

Version 2 (`WebKit-rapid-prototyping.js`) is a combination of the original source code, the idea behind grid.js, and an upgrade that was suggested somewhere in the comments.

In 2025, I decided to test a LLM model I was working on locally by asking it to refactor the code to a modern version. And that is now version 3, or `WebKit-rapid-prototyping-2025.js`. Which should probably be renamed as it's not WebKit-only anymore.


## Changelog

### Version 3, refactored in 2025 - JS

- Replaced old, non-standard, properties like `-webkit-user-modify` with their modern equivalent or alternative approach
- Added event listener to make the text editable when clicked (except input fields, as they are already editable)
- Replaced visual toggle with key combination `Cmd + ;` as the visual version may go above UI elements
- Tested in Chrome 134.0.6998.89 (Official Build) (arm64)


### Version 2, created in 2012 - JS
(Works in Webkit browsers only)

- Fixed url reference in main file
- Added bookmarklet based on Grid.js (separate prototyping tool)


### Version 0.1, created in 2011 - CSS
(Works in Webkit browsers only)

This is the CSS applied to the page:

```css
* {
-webkit-user-modify: read-write;
word-wrap: break-word;
-webkit-nbsp-mode: space;
-webkit-line-break: after-white-space;
}
a {
-webkit-user-modify: initial;
}
```

When you're done with the tests, refresh the page to remove the effect.

## Thank you!
