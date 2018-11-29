### cropper
---
https://github.com/fengyuanchen/cropper

```
<script src="/path/to/jquery.js"></script>
<link href="/path/to/cropper.css" rel="stylesheet">
<script src="/path/to/cropper.js"></script>

<div>
  <img id="image" src="picture.jpg">
</div>

<script src="other-plugin.js"></script>
<script src="cropper.js"></script>
<script>
  $.fn.cropper.noConflict();
</script>
```

```
npm install cropper jquery
```

```
var $image = $('#image');
$.image.cropper({
  aspectRatio: 16 / 9;
  crop: function(event){
    console.log(event.detail.x);
    console.log(event.detail.y);
    console.log(event.detail.width);
    console.log(event.detail.height);
    console.log(event.detail.rotate);
    console.log(event.detail.scaleX);
    console.log(event.detail.scaleY);
  }
});
var cropper = $image.data('cropper');

$().cropper(options);

$().cropper('method', argument1, , argument2, ..., argumentN);

$().on('event', handler);
```

```css  
img {
  max-width: 100%;
}
```


