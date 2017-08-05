
## reboot.css (initial, without normalize.css)
```css
html {
  box-sizing: border-box;
  line-height: 1.15;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

body {
  margin: 0;
}

small {
  font-size: 80%;
}

button,
input {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  margin: 0;
}
```


## reboot.css (full, without normalize.css)
```scss
// Document
html {
  box-sizing: border-box;
  line-height: 1.15;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

// Body
body {
  margin: 0;
}

// Content grouping
//
// 1. Add the correct box sizing in Firefox.
// 2. Show the overflow in Edge and IE.
hr {
  box-sizing: content-box; // 1
  height: 0; // 1
  overflow: visible; // 2
}

hr {
  margin-top: 1rem;
  margin-bottom: 1rem;
  border: 0;
  border-top: $hr-border-width solid $hr-border-color;
}

// Typography
// Remove top margins from headings
//
// By default, `<h1>`-`<h6>` all receive top and bottom margins. We nuke the top
// margin for easier control within type scales as it avoids margin collapsing.
h1, h2, h3, h4, h5, h6 {
  margin-top: 0;
  margin-bottom: .5rem;
}

p, ul, ol {
  margin-top: 0;
  margin-bottom: 1rem;
}

b,
strong {
  font-weight: bolder; // Add the correct font weight in Chrome, Edge, and Safari
}

small {
  font-size: 80%;
}

// Links
a {
  color: $link-color;
  text-decoration: $link-decoration;
  background-color: transparent; // Remove the gray background on active links in IE 10.
  -webkit-text-decoration-skip: objects; // Remove gaps in links underline in iOS 8+ and Safari 8+.

  @include hover {
    color: $link-hover-color;
    text-decoration: $link-hover-decoration;
  }
}

// Images and content
img {
  vertical-align: middle;
  border-style: none; // Remove the border on images inside links in IE 10-.
}

// Tables
table {
  border-collapse: collapse; // Prevent double borders
}

th {
  // Matches default `<td>` alignment
  text-align: left;
}

// Forms
button,
input {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  margin: 0;
}
```


## reboot.css (initial, with normalize.css)
```css
html {
  box-sizing: border-box;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

button,
input {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
```


## reboot.css (full, with normalize.css)
```scss
// Document
html {
  box-sizing: border-box;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

// Content grouping
hr {
  margin-top: 1rem;
  margin-bottom: 1rem;
  border: 0;
  border-top: $hr-border-width solid $hr-border-color;
}

// Typography
// Remove top margins from headings
//
// By default, `<h1>`-`<h6>` all receive top and bottom margins. We nuke the top
// margin for easier control within type scales as it avoids margin collapsing.
h1, h2, h3, h4, h5, h6 {
  margin-top: 0;
  margin-bottom: .5rem;
}

// Links
a {
  color: $link-color;
  text-decoration: $link-decoration;

  @include hover {
    color: $link-hover-color;
    text-decoration: $link-hover-decoration;
  }
}

// Images and content
img {
  vertical-align: middle;
}

// Tables
table {
  border-collapse: collapse; // Prevent double borders
}

th {
  // Matches default `<td>` alignment
  text-align: left;
}

// Forms
button,
input {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
```
