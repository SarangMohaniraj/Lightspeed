# Lightspeed
### A Star Wars "lightspeed" effect.

***
### `Getting Started`
Download lightspeed.js

Create a canvas with `class="lightspeed"`.
<br />Place the javascript file at the bottom of the HTML body.

**index.html**
```html
<canvas class="lightspeed"></canvas>

<script type="text/javascript" src="lightspeed.js"></script>
```


Add a background to the canvas and make sure there are no margins to the body. If you want, you can disable scrolling.

**styles.css**
```css
body {
  margin: 0;
  overflow: hidden;
}
.lightspeed {
  background-color:#000;
  background-image: radial-gradient(circle at top right, rgba(121, 68, 154, 0.13), transparent), radial-gradient(circle at 20% 80%, rgba(41, 196, 255, 0.13), transparent);
}
```

***
### `Usage`

You may change these values. It is not recommended to change any other values.

| key | description | example |
|---|---|---|
| `STAR_COUNT` | number of stars | `(window.innerWidth + window.innerHeight) / 8; //recommended star count` |
|`THRESHOLD` | value before stars are recycled when out of bounds | `50`|
|`star.opacity` | flicker | `(Math.random()*0.5)+0.5`|
|`star.opacity_speed` | flicker speed | `Math.random()/80`|
|`star.size` | size | `(Math.random()*.2)+2.8`|
|`velocity.z` | velocity | `0.005`|
|`ctx.strokeStyle` | star color | `"white"`|

***
#### `Default`
You can `scroll` to change the velocity of the stars and stay in lightspeed!
If you `click + hold`, then `let go`, you can jump to lightspeed!










