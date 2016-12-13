# <more-animations>

<p align="center">
  <img alt="more-animations" src="MoreAnimations400.png" width="300">
</p>

<p align="center">
More animations to use with <a target="_blank" href="https://github.com/PolymerElements/neon-animation#a-basic-animatable-element">Neon Animations Runner</a>.
</p>

<p align="center">
  <a href="https://beta.webcomponents.org/element/convoo/more-animations"><img src="https://img.shields.io/badge/webcomponents.org-published-blue.svg"></a>
  <a href="https://gitter.im/convoo/general"><img src="https://img.shields.io/badge/gitter-join%20chat-brightgreen.svg"></a>
</p>

---

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="../paper-button/paper-button.html">
    <link rel="import" href="../paper-dropdown-menu/paper-dropdown-menu.html">
    <link rel="import" href="../paper-item/paper-item.html">
    <link rel="import" href="../paper-listbox/paper-listbox.html">
    <link rel="import" href="../paper-slider/paper-slider.html">
    <link rel="import" href="animation-demo.html">
    <style>
        paper-slider {
            --paper-slider-knob-color: #ca3b50;
            --paper-slider-active-color: #e5435a;å
        }
        .demo {
            min-height: 500px;
        }
    </style>
    <div>
        <template is="dom-bind">
            <next-code-block></next-code-block>
        </template>
    </div>
  </template>
</custom-element-demo>
```
-->
```html
<div class="demo">
    <animation-demo play="[[selected]]" duration="{{duration}}" delay="{{delay}}">
    </animation-demo>
    <div>
        Duration: [[duration]]
    </div>
    <paper-slider min="100" max="1000" immediate-value="{{duration}}" value="500" snaps step="50"></paper-slider>
    <div>
        Delay: [[delay]]
    </div>
    <paper-slider min="0" max="500" immediate-value="{{delay}}" value="0" snaps step="50"></paper-slider>

    <paper-dropdown-menu label="Show me...">
        <paper-listbox class="dropdown-content" selected="{{selected}}" attr-for-selected="value">
            <paper-item value="bounce-animation">Bounce</paper-item>
            <paper-item value="blink-animation">Blink</paper-item>
            <paper-item value="bulge-animation">Bulge</paper-item>
            <paper-item value="stretch-animation">Stretch</paper-item>
            <paper-item value="shake-animation">Shake</paper-item>
            <paper-item value="swing-animation">Swing</paper-item>
            <paper-item value="tadaa-animation">Tadaa</paper-item>
            <paper-item value="flip-in-side-animation">Flip In Side</paper-item>
            <paper-item value="flip-in-top-animation">Flip In Top</paper-item>
        </paper-listbox>
    </paper-dropdown-menu>
</div>
```


## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
