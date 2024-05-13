# ONYX

An SSG for ONYX Events

# Quick Start

1. Download the Repo
2. Make changes
3. Run `build`
4. Rename and zip the `dist` folder

---

# Notes

-   The Deploy builds a site for preview with Github pages. **The Github Pages url is not meant for distribution.**
-   This repo uses `bun` as a package manager, but this can easily be swapped out for `npm`. Simply delete the `bun-lock` file and run `npm i` before continuing.

## Astro Config & Env Variables

-   The [Astro Config File](https://docs.astro.build/en/reference/configuration-reference/#buildassets) is set for [deployment to Github Pages](https://docs.astro.build/en/guides/deploy/github/) and is overridden with CLI arguments

### v1 and the Two Build Scripts:

In v1, there are 2 build scripts: `build` and `build-elite`. Because the client asked for two pages (with slight variations between the two), each build script is prefixed with an environment variable: `IS_ELITE`, which is used as a simple boolean value.

In v1, this environment toggles a few options:

-   The page `title` is set to "Onyx (Elite) Gift Event"
-   The main logo swaps svgs, to render "Onyx (Elite) Gift Event"
-   The `Details` section has a word about what type of gift event it is: "Onyx (Elite) Gift Event"

Each build script also updates Astro's `base` config to either be `/uploads/onyx-gift-event` or `/uploads/onyx-elite-gift-event`. This is a part of the [Astro CLI](https://docs.astro.build/en/reference/cli-reference/#--base-pathname).

---

# Changelog

## v1.1.0 (ONYX Gift Event &mdash; Grant)

-   Basically the same as v1, but for Grant. Different URLs, event times and images.

## v1.0.0 (ONYX Gift Event)
