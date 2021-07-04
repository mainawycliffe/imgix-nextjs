# Imgix NextJS Images Library

The official imgix library works well out of the box, but when using it SSR with NextJS, lazy loading isn't quite there. The problem images are first loaded and then removed from dom when using the recomended approach, as it relies with lazy sizes to switch from src to data-src for images. This library will attempt to do this but will use data-src and  data-src-set for images. This will allow lazy sizes to kick in and handle lazy loading. A default image can be set to have something like a low dpi initial image.

## Objective:

- [ ] Responsive Images 
  - Generates Responsive Images Using Src Set
  - Fine grain control on sizes being generated - prevents large sizes from being generated unnecessarily
  - Default Image - Possibly Support for Low DPI initial Image
- [ ] Lazy Loading Images
  - Using [Lazysizes](https://github.com/aFarkas/lazysizes) and/or [Native Browser Lazy Loading](https://caniuse.com/loading-lazy-attr)
