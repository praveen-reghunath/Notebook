
### 
#### starts with
```css
a[href^="http"] {
    padding: 30px;
}
```

#### ends with
```css
a[href$=".pdf"] {
 ...
}
```

#### substring selector
```scss
a[href*="facebook"] {
....
}
```

#### Exact match selector

```html
<img src="flower.jpg" title="flower" />

img[title=flower] {
...
}
```

#### attribute value includes
```css
<a href="..." class="btn primary" />

a[class~="primary"] {
  font-weight: bold;
}
```

### sibling selector

```css

<p>This is a heading</p>
<span class="primary">hey</span>

p ~ *[class="primary"] {
  font-weight: bold;
}
```
