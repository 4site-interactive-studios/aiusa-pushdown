# Amnesty International USA Pushdown Project

## How to use

Add the script below to your website.

## Image Mode Example

```html
<script
  defer="defer"
  src="https://aaf1a18515da0e792f78-c27fdabe952dfc357fe25ebf5c8897ee.ssl.cf5.rackcdn.com/1839/pushdown.js"
  data-pushdown-mode="image"
  data-pushdown-content="ALL GIFTS MATCHED TODAY: PROTECT HUMAN RIGHTS AND SAVE LIVES"
  data-pushdown-image="https://source.unsplash.com/860x250/?refugees"
  data-pushdown-link="https://www.4sitestudios.com"
></script>
```

## Text Mode Example

```html
<script
  defer="defer"
  src="https://aaf1a18515da0e792f78-c27fdabe952dfc357fe25ebf5c8897ee.ssl.cf5.rackcdn.com/1839/pushdown.js"
  data-pushdown-mode="text"
  data-pushdown-content="Help us continue to fight human rights abuses. Please give now to support our work"
  data-pushdown-link="https://www.4sitestudios.com"
></script>
```

## Options:

- **data-pushdown-mode**: `image` or `text`
- **data-pushdown-content**: The text to display in the pushdown.
- **data-pushdown-image**: The image to display in the pushdown.
- **data-pushdown-link**: The link to open when the pushdown is clicked.

Change the data attributes with the information you need.

## Example of implementation via Google Tag Manager

```javascript
window.addEventListener("load", function(){
var script = document.createElement('script');
script.src = "https://aaf1a18515da0e792f78-c27fdabe952dfc357fe25ebf5c8897ee.ssl.cf5.rackcdn.com/1839/pushdown.js";
script.dataset.pushdownMode = "image";
// script.dataset.pushdownContent = "Help us continue to fight human rights abuses. Please give now to support our work";
script.dataset.pushdownContent = "ALL GIFTS MATCHED TODAY: PROTECT HUMAN RIGHTS AND SAVE LIVES";
script.dataset.pushdownImage = "https://source.unsplash.com/860x250/?refugees";
script.dataset.pushdownLink = "https://4sitestudios.com";
document.querySelector('head').appendChild(script);
});
```

## Development

Your js code must be on the `src/app` folder. Styling changes must be on `src/scss/main.scss`.

## Install Dependencies

1. `npm install`

## Deploy

1. `npm run build` - Builds the project
2. `npm run watch` - Watch for changes and rebuilds the project

It will create a `dist` folder, where you can get the `pushdown.js` file and publish it.

Currently it's published on Engaging Networks:     
https://aaf1a18515da0e792f78-c27fdabe952dfc357fe25ebf5c8897ee.ssl.cf5.rackcdn.com/1839/pushdown.js
