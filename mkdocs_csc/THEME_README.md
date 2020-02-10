## Theme

This is the documentation of the Material theme. Docs CSC uses a modified version of the Material mkdocs theme. Material theme enables efficient search engine visibility and a well scalable UI. https://squidfunk.github.io/mkdocs-material/

# Relevant directories and files

## mkdocs_csc/base.html

This is the base html file which gets populated by other html files from the partials-directory. If you need to do large scale structure modifications, this is where to start.

## mkdocs.yml

This file dictates the general settings of the site.

* __nav__ for the navigation panel structure
* __theme__ for the theme settings
* __extra_css__ for the css stylesheet we have implemented to the site
* __markdown_extensions__ for the installed extensions. These have to be also in the __requirements.txt__
* __google_analytics__ for the Google Analytics id which links the site to Google Analytics

## mkdocs_csc/assets/stylesheets directory

### extra.css

This is the main CSS file that overwrites CSS in the mkdocs-generated CSS files which represent the default theme. All changes to CSS should be added here or the __extra_mobile.css__ file. Consult #docs.csc.fi in Rocket chat before making changes

### extra_mobile.css

This file is activated when the screen size of the user gets small enough. It scales the content first a bit smaller and eventually (around tablet sizes) starts to change the structure as well. Consult #docs.csc.fi in Rocket chat before making changes

The other CSS files in the directory are generated by mkdocs at build and should not be changed.

## mkdocs_csc/partials directory

Partials directory includes all the html-files of different containers on the site (e.g header div, footer div, sidebar div). If you need to make structural changes inside these containers, this is where to start