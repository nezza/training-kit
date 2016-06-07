# GitHub Training Kit

This is the official courseware for the [GitHub Training Team](http://training.github.com). This repository provides open source materials and slides for teaching GitHub Classes under the [_CC BY 4.0_ license](http://creativecommons.org/licenses/by/4.0/).

We know that part of effectively sharing GitHub and Git with the world goes beyond our team's course offerings. We are pleased to provide you with this training kit that you can use to teach these same concepts at your company, for a user group, or at a conference.

## Download

We know that many of the users of this repository are just focused on getting the materials and teaching from them.  We've made that easy.

1. You can view and teach from the kit, hosted on GitHub, at https://services.github.com/kit/
2. You can download an offline copy of the kit via the green button at https://github.com/github/training-kit/releases


## Contribute

We’re eager to have your help in improving this kit. If you have an idea for a change, start by opening a new [Issue](https://github.com/github/training-kit/issues) so we can discuss and help guide your contribution to the right location. If you have corrections or kit contributions, we'd be glad to receive them via a [Pull Request](https://help.github.com/articles/using-pull-requests). For kit contributions, we ask you to share in our mindset of minimalism.

### Class Material

[GitHub for Developers](https://services.github.com/kit/courses/github-for-developers.html) and [GitHub for Everyone](https://services.github.com/kit/courses/github-for-everyone.html) are the two class types taught by the GitHub Training team. Their content is composed of several modules listed in the `[_modules/](https://github.com/github/training-kit/tree/master/_modules/)` subdirectory.

### Cheat Sheets

The Git and GitHub Cheat Sheets are located within the `[downloads/](https://github.com/github/training-kit/tree/master/downloads/)` directory. There are some translations available and we're always looking for more. If you are looking to get a `.pdf` generated for the html version of a cheatsheet, please start an issue and @mention [@brntbeer](https://github.com/brntbeer) or [@crichid](https://github.com/crichid) and they will see to the request.

### Legacy Class Material

There are old slides that slides align with the [Foundations](https://github.com/github/training-kit/tree/master/foundations/index.md), [Intermediate](https://github.com/github/training-kit/blob/master/intermediate/index.md), and [Advanced](https://github.com/github/training-kit/tree/master/advanced/index.md) classes previously delivered by the GitHub Training team.

These three legacy class' slides reside at top-level directories:
- [`foundations/`](https://github.com/github/training-kit/tree/master/foundations)
- [`intermediate/`](https://github.com/github/training-kit/tree/master/intermediate)
- [`advanced/`](https://github.com/github/training-kit/tree/master/advanced)


## File Format

The class materials are written in [Markdown](http://whatismarkdown.com), a [lightweight markup language](http://en.wikipedia.org/wiki/Lightweight_markup_language) supported in the GitHub web application user interface. There is a syntax guide to the original [Markdown format](http://daringfireball.net/projects/markdown/syntax) and also [GitHub Flavored Markdown](http://github.github.com/github-flavored-markdown/).

The class material content possess two specialized uses of Markdown for slide-like rendering and formatting:

- Full-screen slides are preceded with a `---` and followed by `---`
- Step-by-step *lab* sections are wrapped with `{% capture lab %}` and `{% endcapture %}{% include lab %}`

 This repository is based on [Hydeslides](https://github.com/jordanmccullough/HydeSlides). That project offers additional information on the file and directory structure.

## Build

The build of this repository is fully automated through several shell scripts. To perform a build of the materials identical to that of our continuous integration server, from the top directory of this project, run `script/cibuild` and then inspect the output in the `_site` directory.

The `script/makerelease` script produces a zip bundle for offline use of these materials. Pre-built releases are available at https://github.com/github/training-kit/releases
