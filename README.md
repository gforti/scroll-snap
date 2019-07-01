# Scroll Snap CSS
CSS Scroll Snap demo

The scroll-snap-type CSS property sets how strictly snap points are enforced on the scroll container in case there is one.

## Format

> scroll-snap-type: none | [ x | y | block | inline | both ] [ mandatory | proximity ]

## Sample CSS 

```css
/* Optional mandatory | proximity*/
scroll-snap-type: x mandatory;
scroll-snap-type: y proximity;
scroll-snap-type: both mandatory;
```

The inner container must also have the following style

```css
scroll-snap-align: center;
```

Final

```css
.container {
  scroll-snap-type: y mandatory;
}

.child {
  scroll-snap-align: start;
}
```

## Resoruces

- https://css-tricks.com/practical-css-scroll-snapping/
- https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-snap-type
- https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-snap-align
- https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API