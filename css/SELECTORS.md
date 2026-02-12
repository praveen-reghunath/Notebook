
### 
#### starts with
```
a[href^="http"] {
    padding: 30px;
}
```

#### ends with
```
a[href$=".pdf"] {
 ...
}
```

#### substring selector
```
a[href*="facebook"] {
....
}
```

#### Exact match selector

```
<img src="flower.jpg" title="flower" />

img[title=flower] {
...
}
```

#### attribute value includes
```
<a href="..." class="btn primary" />

a[class~="primary"] {
  font-weight: bold;
}
```

### sibling selector

```

<p>This is a heading</p>
<span class="primary">hey</span>

p ~ *[class="primary"] {
  font-weight: bold;
}
```
