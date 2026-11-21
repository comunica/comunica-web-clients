# Comunica Web Clients

[Comunica web clients](https://github.com/comunica/jQuery-Widget.js), built from [comunica/comunica](https://github.com/comunica/comunica)
on every commit to its `master` and `next/*` branches, and for every release.

**Browse them at https://comunica.github.io/comunica-web-clients/**

The web client of the latest release is also available at https://query.comunica.dev/.

## How this works

The CI of [comunica/comunica](https://github.com/comunica/comunica) builds these web clients,
and deploys them to the `gh-pages` branch of this repository, from which they are served with GitHub Pages.
Each branch or release has its own directory, such as `master/` or `v5.4.1/`, and each config in it has its own subdirectory, such as `master/default/`.

Every deploy replaces the `gh-pages` branch with a single commit, so its history is not kept.
Changes to the branch are kept by later deploys, which is how old releases can be removed if the site grows too large.

The configs that are built, and the build itself, are defined in the
[`web-clients` directory](https://github.com/comunica/comunica/tree/master/web-clients) of comunica/comunica.

## License

This code is copyrighted by the [Comunica Association](https://comunica.dev/association/) and [Ghent University – imec](http://idlab.ugent.be/)
and released under the [MIT license](http://opensource.org/licenses/MIT).
