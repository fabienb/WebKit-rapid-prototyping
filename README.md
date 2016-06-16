# css-rapid-prototyping
This bookmarklet creates a grid overlay to the page and allows for any text in the page to be modified for the sake of rapid prototyping.
It uses basic CSS and a base64 SVG, therefore it's very easy for anyone to customise it (disable the grid, add features, etc.).

I took the idea from an article on [css-101.org](http://cssmojo.com/trick_for_rapid_prototyping/): I used to copy and paste that CSS to an open page with the MyStyle extension but then I thought it would have been quicker to create this bookmarklet.

I have later found out that someone else had the same idea, and had also added a useful on/off functionality, check that out: [grid.js](https://gist.github.com/webxl/1232664).

If you still want to try this version (thank you), download the .js file and host it somewhere, then edit the url in the bookmarklet accordingly.

## Version 0.1, created in 2011
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
