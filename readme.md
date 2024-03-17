![screenshot](screenshot.png)

[Live version](https://joeriexelmans.github.io/freehand/sketching.html)

Prototype of a web-/SVG-based sketching app. Supports:
  * pressure sensitivity
  * multi-touch (multiple people drawing simultaneously on a single touchscreen)

Could serve as a basis for research:
  * building a multi-touch interface for large (multi-user) touchscreens
  * shape recognition
  * collaborative (a)synchronous sketching
  * compressing freehand drawing data (by removing data points that don't matter, or approximating curvy lines with splines), like this paper: https://www.researchgate.net/publication/220998377_Sketch_Parameterization_Using_Curve_Approximation


TODOs (if we ever want to actually use this):
  * Text mode
  * Image (PNG, SVG, JPEG, ...) import
  * Rotating, resizing selection
  * Xournal++ import/export
  * SVG export (easy)
  * Editor state + history (de-)serialization
  * Improving sketch quality:
      * Pointer events in Firefox and Chrome currently have integer coordinates, even when zoomed in! As a result, diagonal lines drawn slowly look like staircases. Xournal++ has access to float coordinates, which looks better. https://github.com/w3c/pointerevents/issues/107
      * Line thickness should respond smoothly to pointer pressure, instead of in 10% increments.