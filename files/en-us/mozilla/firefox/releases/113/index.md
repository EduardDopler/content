---
title: Firefox 113 for developers
slug: Mozilla/Firefox/Releases/113
---

{{FirefoxSidebar}}

This article provides information about the changes in Firefox 113 that affect developers. Firefox 113 is the current [Beta version of Firefox](https://www.mozilla.org/en-US/firefox/channel/desktop/#beta) and ships on [May 09, 2023](https://wiki.mozilla.org/RapidRelease/Calendar#Future_branch_dates).

## Changes for web developers

### Developer Tools

### HTML

#### Removals

### CSS

- The [`color()`](/en-US/docs/Web/CSS/color_value/color), [`lab()`](/en-US/docs/Web/CSS/color_value/lab), [`lch()`](/en-US/docs/Web/CSS/color_value/lch), [`oklab()`](/en-US/docs/Web/CSS/color_value/oklab), [`oklch()`](/en-US/docs/Web/CSS/color_value/oklch), and [`color-mix()`](/en-US/docs/Web/CSS/color_value/color-mix) functional notations are now supported, along with the [`forced-color-adjust`](/en-US/docs/Web/CSS/forced-color-adjust) property.
  For more information on the functional notations, see the [CSS color value](/en-US/docs/Web/CSS/color_value) documentation.
  ([Firefox bug 1352753](https://bugzil.la/1352753), [Firefox bug 1813497](https://bugzil.la/1813497), [Firefox bug 1818819](https://bugzil.la/1818819), [Firefox bug 1824526](https://bugzil.la/1824526)).

#### Removals

### JavaScript

#### Removals

### SVG

#### Removals

### HTTP

#### Removals

### Security

#### Removals

### APIs

- [`CanvasRenderingContext2D.reset()`](/en-US/docs/Web/API/CanvasRenderingContext2D/reset) and [`OffscreenCanvasRenderingContext2D.reset()`](/en-US/docs/Web/API/OffscreenCanvasRenderingContext2D#canvasrenderingcontext2d.reset) are now supported, and can be used to return the associated rendering context to its default state.
  ([Firefox bug 1709347](https://bugzil.la/1709347)).
- The [Compression Streams API](/en-US/docs/Web/API/Compression_Streams_API) is now supported.
  The interfaces provided by this API are used to compress and decompress data using the `gzip` and `deflate` formats ([Firefox bug 1823619](https://bugzil.la/1823619)).
- [`Window.print()`](/en-US/docs/Web/API/Window/print) now opens a print dialog on Firefox for Android, allowing the current document to be printed ([Firefox bug 1809922](https://bugzil.la/1809922)).

#### DOM

#### Media, WebRTC, and Web Audio

- The [AV1 video codec](/en-US/docs/Web/Media/Formats/Video_codecs#av1) is now enabled on Android. Hardware accelerated decoding is used if supported by the device ([Firefox bug 1672276](https://bugzil.la/1672276)).

#### Removals

- The deprecated and non-standard `CanvasRenderingContext2D.mozTextStyle` attribute was permanently removed. This was previously hidden behind a preference. ([Firefox bug 1294362](https://bugzil.la/1294362)).

### WebAssembly

#### Removals

### WebDriver conformance (WebDriver BiDi, Marionette)

#### WebDriver BiDi

#### Marionette

## Changes for add-on developers

- When an extension registers multiple listeners for the same event, all the event listeners are called when the event page wakes up, instead of only the first one ([Firefox bug 1798655](https://bugzil.la/1798655)).
- Support is now provided for the {{WebExtAPIRef("declarativeNetRequest")}} API ([Firefox bug 1782685](https://bugzil.la/1782685)).
- The `gecko_android` subkey has been added to the [`browser_specific_settings`](/docs/Mozilla/Add-ons/WebExtensions/manifest.json/browser_specific_settings) key. This subkey enables an extension to specify the range of Firefox for Android versions it is compatible with ([Firefox bug 1824237](https://bugzil.la/1824237)).

### Removals

### Other

## Older versions

{{Firefox_for_developers(112)}}
