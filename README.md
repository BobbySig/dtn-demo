# DTN Presentation Creator

This document is to collect everything we have pertaining to making a web-based
presentation creation platform for DTN (and other places) in one place.

## Demo Presentation

A demo of a synchronized Reveal.js presentation and a launcher can be found in
the `gh-pages` branch. It isn't much, but it works.

## Things We Know

### Things We Cannot Do In a Normal Web Page

* Move windows arbitrarily around the screen
* Make another window go into fullscreen mode

### Things We Can Do, But Only In a Chrome App

* Arbitrarily spawn windows anywhere on the screen
* Fullscreen other windows

## Possible Tech Stack

* Reveal.js - Javascript presentation library.
* Ruby on Rails - Web application framework.

## UI Designs

We never got very far, but a few UI sketches were made early on the last time we
tried. You can find them in `./media/sketches/`.

## Synchronizing Reveal.js Presentations

See [Reveal.js Multiplexing](https://github.com/hakimel/reveal.js/#multiplexing)
for detailed instructions, and refer to the demo presentation for some other
configuration details. Eventually we'll need our own socket server for this,
but it really is just a standard socket server so you don't need to deal with
Node unless you want to.
