# Astro SVG Icon

This is a component that lets you add SVG icons to your Astro project using modern Web Standards. #UseThePlatform
The component utilizes the SVG `<use>` tag, allowing the developer to include any external SVG asset, typically an icon for websites.

## How to use

```jsx
---
import Icon from 'astro-svg-icon';
import { Calendar } from 'Calendar.svg';
---

<Icon src={Calendar.src} viewBox={`0 0 ${Calendar.width} ${Calendar.height}`} />
```

## Advantages

- 🚀 The image is loaded by the browser as an image, making caching possible
- 💅 An inline SVG tag allows for flexible styling with CSS.

## Limitations

- The `id` of the SVG must be the same as the name of the file. For example:

```html title="Calendar.svg"
<!-- Calendar.svg -->
<svg id="Calendar" ... />
```

## References

Read on to find out why it's useful.

- https://kurtextrem.de/posts/svg-in-js
- https://karolytorok.netlify.app/blog/styling-an-svg/

