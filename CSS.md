# Awesome CSS Tips ![Awesome][awesome-badge]

#### Contents

- [Cursors](#cursors)
- [Smooth Scrolling](#smooth-scroll)
- [Truncate Text](#truncate-text)
- [Truncate Text To The Specific Number Of Lines](#truncate-text-to-the-specific-number-of-lines)
- [Calc Function](#calc-function)
- [CSS-only modals](#css-only-modals)

## Cursors

Did you know that you can use your own image, or even emoji as a cursor? 

```css
div {
    cursor: url('path-to-image.png'), url('path-to-fallback-image.png'), auto;
}
```

[Link to Codepen](https://codepen.io/denic/pen/bGVpOPj)

## Smooth Scroll

Smooth scrolling without #javascript, with just one line of CSS.

```css
html {
    scroll-behavior: smooth;
}
```

[Link to Codepen](https://codepen.io/denic/pen/bGVeYqN)

## Truncate Text

Did you know that you can truncate text with plain CSS?

```css
.overflow-truncate {
    text-overflow: ellipsis;
}
```

[Link to Codepen](https://codepen.io/denic/pen/LYpZKMg)

## Truncate Text To The Specific Number Of Lines

You can use `-webkit-line-clamp` property to truncate the text to the specific number of lines. An ellipsis will be shown at the point where the text is clamped.

```css
.overflow-truncate {
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 3;
    overflow: hidden;
}
```

[Link to Codepen](https://codepen.io/denic/pen/pojEKGX)

## Calc Function

The `calc()` CSS function lets you perform calculations when specifying CSS property values.

```css
div {
    width: calc(100% - 30px);
}
```

## CSS-only modals

You can use the :target pseudo-class to create modals with zero JavaScript.

```css
.modal {
    visibility: hidden;
}

/*
    Selects an element with an id matching the current URL's fragment
    Example: example.com#demo-modal
*/
.modal:target {
    visibility: visible;
}
```

[Link to Codepen](https://codepen.io/denic/pen/ZEbKgPp)

[awesome-badge]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

