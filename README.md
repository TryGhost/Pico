# Pico

A minimal, functional theme for running a paid-membership publication on [Ghost](https://ghost.org) - originally created by [@pjrvs](https://github.com/pjrvs) and [@jackellis](https://github.com/jackellis), acquired and stewarded by [@tryghost](https://github.com/tryghost) in 2020. Now available for free, for everyone!

![pico](https://user-images.githubusercontent.com/120485/70646878-67b93400-1c7a-11ea-9722-64bb7ecf2d22.png)

&nbsp;


# Instructions

1. [Download this theme](https://github.com/TryGhost/Pico/archive/master.zip)
2. Log into Ghost, and go to the `Design` settings area to upload the zip file
3. Unzip the theme archive on your computer and locate the file called `routes.yaml`
4. Inside Ghost admin, go to the `Labs` settings area and scroll down until you see the `Custom Routes` section
5. Upload the `routes.yaml` from this theme

That's it! You now have a Ghost publication which supports free and paid memberships. If you need help, check out the <a href="https://ghost.org/docs/members/">Ghost members documentation</a> or chat with other Ghost users on <a href="https://forum.ghost.org">Ghost forum</a>.

&nbsp;

# Development

Styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
$ yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
yarn zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.
- Variables - Simple pure CSS variables
- [Color Function](https://github.com/postcss/postcss-color-function)


# Copyright & License

Copyright (c) 2013-2020 Ghost Foundation - Released under the [MIT license](LICENSE).
