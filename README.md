:iphone: js-vido — JavaScript Video Download Optimizer
======================================================

A JavaScript library for optimizing html pages with video content that prevents videos from loading on mobile devices.

:question: What it does
-----------------------

Prevents videos with the "optimize-video" class from being downloaded to mobile devices by displaying the poster image instead. This is done by creating the source element of the video node through the data-src attribute only in case the device used is a laptop or desktop computer.

One of the cases where this functionality can be useful is verified with auto-play videos used in web page backgrounds, because auto-play does not work on mobile devices, the video would be downloaded unnecessarily, slowing down the loading of the page and consuming mobile data.

:dash: Usage
------------

1. In the video node add the following attributes:

    | Attribute Name | Attribute Content | Description               | Required            |
    |----------------|-------------------|---------------------------|---------------------|
    | class          | "optimize-video"  | video identifier          | :heavy_check_mark:  |
    | data-src       | "https://..."     | video source              | :heavy_check_mark:  |
    | data-type      | "video/mp4"       | video type                | :heavy_check_mark:  |
    | poster         | "https://..."     | image displayed on mobile |                     |
   
2. Import the js library at the end of the body node:

   `<script src="https://cdn.jsdelivr.net/gh/ariel-mn/js-vido@1.0.0/js-vido.js" integrity="sha256-aLD7G9V/25SfpmWNWLbcGblvtThOEb21GpDUKuHXqD8=" crossorigin="anonymous"></script>`

:dizzy: Example
---------------

```html
<!-- Optimized Video -->
<video class="optimize-video" autoplay muted loop poster="https://image.jpeg" data-src="https://video.mp4" data-type="video/mp4"></video>

<!-- js-vido -->
<script src="https://cdn.jsdelivr.net/gh/ariel-mn/js-vido@1.0.0/js-vido.js" integrity="sha256-aLD7G9V/25SfpmWNWLbcGblvtThOEb21GpDUKuHXqD8=" crossorigin="anonymous"></script>
```

:scroll: License
----------------

[MIT][license] © [Montes][website]

[license]: /LICENSE
[website]: https://montesariel.com
