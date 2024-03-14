![screenshot](screenshot.png)

[Live version](https://joeriexelmans.github.io/freehand/sketching.html)

Prototype of a web-/SVG-based sketching app. Wanted to find out if it is possible to support:
  * pressure sensitivity
  * multi-touch (multiple people drawing simultaneously on a large touchscreen)

Pressure sensitivity is working. Tested with Huion Q11V2 tablet.

Multi-touch is currently not working. Have yet to figure out the right APIs, and whether it **is** actually possible to implement in a browser.

Could serve as a basis for research:
  * compressing freehand drawing data (by removing data points that don't matter, or approximating curvy lines with splines)
  * collaborative (a)synchronous sketching