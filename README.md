# CSS Tips
Collection of CSS tips


## Positioning

### inset

`inset` allows to specify `top`, `right`, `bottom` and `left` with a single CSS line.
[Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/inset)

### anchor()

![image](https://github.com/user-attachments/assets/677b666e-4d09-4ae3-99ef-92658a4c696f)


```html
<body>
  <div id="box1"></div>
  <div id="box2" anchor="box1"></div>
</body>
```

```css
. {
  position: absolute;
  bottom: anchor(top);
  left: anchor(center);
}
```

[Reference video](https://www.youtube.com/shorts/fO0XD75u2TI)


## Text

### Avoid wrapping text

You can use `min-width: fit-content;` instead of `white-space: nowrap;`
[Reference Video](https://www.youtube.com/shorts/4GR_lE1W09o)

## Transitions

### Transition to and from `display: none`

[Youtube video](https://youtu.be/vmDEHAzj2XE?si=kXEVH8Xy8jIgY5Od)


## CSS Reset

### Minimal Reset

[Reference](https://www.youtube.com/shorts/2lyDv0wOQuQ)

```css
*, *::before, *::after {
  box-sizing: border-box;
}

* {
  margin: 0;
  padding: 0;
  font-inherit;
}

html {
  color-scheme: dark light;
}

body {
  min-height: 100vh;
}

img, picture, svg, video {
  display: block;
  max-width: 100%
}
```
