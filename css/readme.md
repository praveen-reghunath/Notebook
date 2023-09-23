
## To make all child columns have equal width no matter what content in it.
````css
.parent-element-css-class {
    display: flex;
    gap: 1rem; // for giving a gap between items
}

.parent-element-css-class > * {
    flex-basis: 100%; // force all children share equal width
}
````

### A Grid Style layout without media queries
````css
.parent-element-css-class {
    display: flex;
    flex-wrap: wrap;
}

.parent-element-css-class > * {
    flex: 1 1 30%; // grow shrink & baisis
}
````

### Content & Side bar- To Create a std main content area and side bar.
````css
.parent-element-css-class {
    display: flex;
    flex-wrap: wrap;
}

.parent-element-css-class>*:nth-child(1){
    flex: 1 1 70%;
    min-width: 40ch;
}

.parent-element-css-class>*:nth-child(2){
    flex: 1 1 30%;
    min-width: 10ch;
}
````

### Create a background with stripes 
```
.css-13irs1z {
    background-image: repeating-linear-gradient(-45deg, transparent, transparent 8px, currentcolor 8px, currentcolor 10px);
    padding: 0px;
    aspect-ratio: 6 / 1;
    border: 0px;
    display: block;
    color: inherit;
}
```

The document.getAnimations method returns an array of CSSAnimation objects. 
```
// Make all CSS animations on the page twice as fast
document.getAnimations().forEach((animation) => {
  animation.playbackRate *= 2;
});

// Stop all CSS animations on the page
document.getAnimations().forEach((animation) => {
  animation.cancel();
});
```
