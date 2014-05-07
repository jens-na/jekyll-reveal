Overview
========
**jekyll-reveal** is a template for the site generator Jekyll to create presentations
with the framework revleal.js in a very easy way. You can even specify options
in the YAML front matter of Jekyll.

Currently the submodule of reveal.js points to the [2.6.1](https://github.com/hakimel/reveal.js/releases/tag/2.6.1) release.

Installation
============

```
  $ gem install jekyll  
  $ git clone --recursive https://github.com/jens-na/jekyll-reveal.git
  $ cd jekyll-reveal
  $ jekyll serve --watch
```

Aferwards you can point your favorite browser to http://localhost:4000/

Create a new slide
==================
New slides are created in the directory `_slides`. The index page updates
automatically. Take a look at the [example slide](https://github.com/jens-na/jekyll-reveal/blob/master/_slides/test-reveal-slides.html).

YAML front matter
=================
jekyll-reveal extends the YAML front matter of Jekyll. You can specify
different options there.

```yml
---
layout: slide
title: "Test slides with reveal.js"
reveal:
  theme: default
  controls: true
  progress: false
  history: false
  transition: default
---
```

- `theme` - Any theme in the directory /reveal.js/css/theme/
- `controls` - enables the controls in your presentation
- `progress` - enables the progress bar at the bottom of your page
- `history` - enables the history of the presentation
- `transition` - the transition, which may be default, cube, page, concave, zoom, linear, fade, none

License
=======
Licensend under the MIT License

(C) Jens Nazarenus, 2014
