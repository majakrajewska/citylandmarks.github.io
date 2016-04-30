## aframe-href-component

A Hyper Link component for [A-Frame](https://aframe.io). Help you deal with web links like on the normal web.

Add `href="www.sample.com"` attribute to any a-frame tag, turn the object as a normal web link. [demo](https://gasolin.github.io/aframe-href-component/basic/link.html)

### Anchor support (experimental)

Besides the normal hyper link. you can add in-page anchor like `href="#id"` to any a-frame tag. When user click on the object, `a-camera` will move its position to the object with the specified id. [demo](https://gasolin.github.io/aframe-href-component/basic/anchor.html)

### Usage

#### Browser Installation

Install and use by directly including the [browser files](dist):

Add `href` attribute in target tag (In example is `a-box`).

```html
<head>
  <title>My A-Frame Scene</title>
  <script src="https://aframe.io/releases/0.2.0/aframe.min.js"></script>
  <script src="https://rawgit.com/gasolin/aframe-href-component/master/dist/aframe-href-component.min.js"></script>
</head>

<body>
  <a-scene>
    <a-entity position="0 1.8 4">
      <a-camera>
        <a-cursor color="#4CC3D9"></a-cursor>
      <a-camera>
    </a-entity>

    <a-box id="orange-cube" position="0 3.5 -2" rotation="30 30 0"
      width="2" depth="2" height="2" color="#F16745"
      href="https://github.com/gasolin/aframe-href-component"></a-box>
  </a-scene>
</body>
```

[demo](https://gasolin.github.io/aframe-href-component/basic/index.html)

#### NPM Installation

Install via NPM:

```bash
npm install aframe-href-component
```

Then register and use.

```js
require('aframe');
require('aframe-href-component');
```
