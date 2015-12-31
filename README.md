# noscroll

The scroll event handler is often used to implement custom smooth<sup>[sic]</sup> scrolling behaviour on web pages. This ends up being super janky nearly every time though and makes reading these web pages quite annoying. Unfortunately, we can't just write off these misbehaving websites entirely since sometimes they have useful content on them.

This Chrome extension blocks web pages from attaching to certain scroll-related events, meaning that you never again have to be annoyed by a web page's broken custom scrolling.

It works by hijacking the `EventTarget.prototype.addEventListener` function and preventing any event listeners from being attached to the following event types:

* `scroll`
* `scrollstop`
* `mousewheel`
* `wheel`

It also blocks these events through the old-style `onevent` interface on `window` and `document`.

## Installing

* Clone this repo

* Go to chrome://extensions/

* Click **Load unpacked extension**

* Navigate to wherever you cloned this repo on disk

## License

[MIT](LICENSE)
