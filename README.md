gitbook-plugin-cloudinary-video
==============

This plugin helps you to include `Cloudinary-Video` tag in your html5 pages.

This plugins requires gitbook `>=2.0.0`.

### Setup

Add it to your `book.json`, then run `gitbook install`:

```
{
    plugins: ["cloudinary-video"]
}
```

### Write in gitbook-markdown.md

```
1. {% video %} cloudinary-public-id {% endvideo %}

2. {% video width="740", height="350" %} cloudinary-public-id {% endvideo %}

3. {% video width="740", height="350", loop="loop", controls="controls" %}cloudinary-public-id{% endvideo %}
...

```

### gitbook build result.
```
<video src="https://www.domain.com/video.mp4" width="100%" height="100%"></video>

<video src="https://www.domain.com/video.mp4" width="740" height="350"></video>

<video src="https://www.domain.com/video.mp4" width="740" height="350" controls="controls" loop="loop"></video>
```
