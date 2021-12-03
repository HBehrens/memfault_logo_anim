[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/HBehrens/memfault_logo_anim)

# Animated Memfault Logo

Project for Memfault Awesome Day (MAD) project by [@HBehrens](https://twitter.com/hbehrens).
Renders the [Memfault](https://memfault.com) logo and provides some animations and interactions.

![Animated Memfault Logo](https://raw.githubusercontent.com/HBehrens/readme_assets/main/memfault_logo_anim/memfault_logo_anim.gif)

[Try it out now!](https://hbehrens.github.io/memfault_logo_anim/) This project was heavily inspired by Gitpod's former loading screen ❤️

# How does it work

The logo is technically a 2D SVG with several nested groups each with individually configured CSS transforms.
Careful placement of SVG clipping paths that are transformed in sync creates the desired effect.

JavaScript performs logic and drives changes values for various CSS variables using [GreenSock](https://greensock.com/gsap/).
Various `calc()` expressions in the CSS will apply these variables leading to the visual effects without making any changes to SVG itself.

![Fake perspective triggered by mouse movement](https://raw.githubusercontent.com/HBehrens/readme_assets/main/memfault_logo_anim/memfault_logo_anim_mouse.gif)

The example further responds to mouse movement to give the illusion of a truly three-dimensional object.

# Next Steps

* [x] Publish to [Github Pages](https://hbehrens.github.io/memfault_logo_anim/)
* [ ] Clean up [horrible source code](https://github.com/HBehrens/memfault_logo_anim/blob/main/index.html)
* [ ] Re-package as React component to be used in [Memfault's UI](https://docs.memfault.com/docs/platform/charts)
* [ ] Hire awesome talent for [open positions in Berlin/EU](https://mflt.io/careers)
