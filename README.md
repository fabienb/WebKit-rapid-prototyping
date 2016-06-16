# css-rapid-prototyping
This bookmarklet creates a grid overlay to the page and allows for any text in the page to be modified for the sake of rapid prototyping.
It uses basic CSS and a base64 SVG, therefore it's very easy for anyone to customise it (disable the grid, add features, etc.).

## Version 0.1
works in Webkit browsers only

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
