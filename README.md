### Tilting Rectangle

Hover over the box below to see it tilt towards your mouse!

```html
<div class="tilt-box">
  <h2>Hover over the box to tilt it!</h2>
</div>
```

```css
.tilt-box {
  width: 300px;
  height: 150px;
  background-color: pink;
  position: relative;
}

.tilt-box:hover {
  transform: rotateX(20deg) rotateY(-20deg);
}

.tilt-box h2 {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}
```

In this example, we create a tilting rectangle using HTML and CSS. The rectangle is contained in a `div` with the class `tilt-box`, and includes an `h2` with a prompt to hover over the box.

On hover, the `tilt-box` element tilts towards the mouse using CSS transitions. The `rotateX` and `rotateY` functions specify the angles of rotation along the x and y axes, respectively.

You can customize the size and styles of the box and text to fit your needs.
