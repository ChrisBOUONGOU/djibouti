# FDF redesign — Symfony 8 / Twig

This branch contains a Symfony-oriented implementation of the FDF homepage concept.

## Files added

- `src/Controller/HomeController.php`: Symfony 8 attribute route for `/`.
- `templates/base.html.twig`: shared HTML layout and AssetMapper entry point.
- `templates/home/index.html.twig`: homepage sections, navigation, news cards, teams, competitions and contact footer.
- `assets/app.js`: mobile navigation and CSS import.
- `assets/styles/app.css`: responsive visual system.

## Requirements

These files are intended to be copied into a Symfony 8 application that has Twig, Symfony AssetMapper and ImportMap configured (the usual Symfony webapp setup). This repository branch does not itself contain a full Symfony project scaffold or `composer.json`.

If the target application does not have AssetMapper/ImportMap installed, install/configure the project's chosen frontend asset pipeline and adapt the `importmap('app')` call in `base.html.twig`.

## Local setup

From the root of your existing Symfony 8 project:

1. Copy the files into the matching paths.
2. Ensure Twig and AssetMapper/ImportMap are installed and configured.
3. Start the Symfony local server with `symfony server:start` or your usual local setup.
4. Open the root URL.

## Before production

- Replace the text crest with the official FDF logo and use authorized photos.
- Replace example editorial cards with real, verified articles from the federation.
- Connect news, teams and competitions to entities/repositories or a CMS.
- Verify all official links and contact information.
- Add tests, accessibility checks, metadata/social previews and image optimization.

This is an unofficial design proposal, not an official FDF publication. Remote images are temporary Unsplash placeholders.
