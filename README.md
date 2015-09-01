---
title: README
layout: page
permalink: /about/
---

This is my attempt to bring together [Jekyll](http:/jekyllrb.com) and [Foundation](http://foundation.zurb.com) in harmony.  This perhaps may be a bit of overkill, but I wanted to use all the tools that were most "natural" for everything:

* I want my gems in [Bundles](http://bundler.io/), not installed globally.  Yes, even Jekyll.

* Foundation wants to be installed via [bower](http://bower.io/).  Sure I could just import the files manually, but that's why we have computers.

* I don't want to have to copy/minify/whatever my assets by hand, so let's add a dash of [Jekyll Assets](http://jekyll-assets.github.io/jekyll-assets/).  Mostly this was to tie together bower's directories and the standard directories as simply as I could.

* Minimalist: While Foundation does have everything and the [kitchen sink](http:/foundation.zurb.com/docs/components/kitchen_sink.html), I'd rather just pull in what I need.  So this project tends to pull individual portions of Foundation and trust to assets to minify them later.

Prerequisites
-------------

* [Ruby](http://www.ruby-lang.org)
* [node.js](http://nodejs.org)

Quickstart
----------

```sh
gem install bundler
bundle install
cd vendor
npm install
node_modules/.bin/bower install
cd ..
bundle exec jekyll build
```

After that, you can build your site to your liking.  The theme here is a minimal translation of the base Jekyll theme to use Foundation.
