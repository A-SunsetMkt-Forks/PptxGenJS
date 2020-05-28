---
id: usage-slide-options
title: Slide Methods
---

## Slide Numbers

### Slide Number Syntax

```javascript
slide.slideNumber({ x: 1.0, y: "90%" });
```

### Slide Number Options

| Option       | Type     | Description                      | Possible Values                                                                 |
| :----------- | :------- | :------------------------------- | :------------------------------------------------------------------------------ |
| `x`          | number   | (inches) horizontal location     | 0-n OR 'n%'. (Ex: `x:'10%'` places number 10% from left edge)                   |
| `y`          | number   | (inches) vertical location       | 0-n OR 'n%'. (Ex: `y:'90%'` places number 90% down the Slide)                   |
| `w`          | number   | (inches) containing shape width  | 0-n. Ex: `w:1.5`                                                                |
| `h`          | number   | (inches) containing shape height | 0-n. Ex: `h:1.0`                                                                |
| `background` | BkgdOpts | background color/images          | add background color or image.                                                  |
| `color`      | string   | text color                       | hex color code or [scheme color constant](#scheme-colors). Ex: `color:'0088CC'` |
| `fontFace`   | string   | font face                        | any available font. Ex: `fontFace:Arial`                                        |
| `fontSize`   | number   | font size                        | 8-256. Ex: `fontSize:12`                                                        |
| `hidden`     | boolean  | whether slide is hidden          |                                                                                 |

### Background Examples

```javascript
// Solid color
slide.background = { fill: "F1F1F1" };

// base64 data
slide.background = { data: "image/png;base64,ABC[...]123" };

// image url
slide.background = { path: "https://some.url/image.jpg" };
```

### Slide Number Examples

```javascript
// EX: Add a Slide Number at a given location
slide.slideNumber({ x: 1.0, y: "90%" });

// EX: Styled Slide Numbers
slide.slideNumber({ x: "50%", y: "90%", fontFace: "Courier", fontSize: 32, color: "CF0101" });
```

## Slide Hiding

Hide a given Slide.

### Slide Hiding Syntax

```javascript
slide.hidden = true;
```
