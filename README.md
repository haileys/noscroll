# noscroll

Web developers can not be trusted with the scroll event. This extension blocks them from using it.

It blocks the following events:

* `scroll`
* `scrollstop`
* `mousewheel`
* `wheel`

It blocks these events by overriding the `EventTarget.prototype.addEventListener` function and preventing any event listeners from being attached to these event types.

It also blocks these events through the old-style `onevent` interface on `window` and `document`.

## Installing

* Clone this repo

* Go to chrome://extensions/

* Click **Load unpacked extension**

* Navigate to wherever you cloned this repo on disk

## License

[MIT](LICENSE)
