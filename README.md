# [![newspaper](./assets/logo.png)](https://vllur.github.io/newspaper/)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
[![Build Status](https://travis-ci.org/vllur/newspaper.svg?branch=master)](https://travis-ci.org/vllur/newspaper)

Light box Jekyll theme.

### Main features:
- full Github Pages compatibility
- tags
- custom baseurl support
- Google Analytics support
- complex Travis CI testing with [htmlproofer](https://github.com/gjtorikian/html-proofer) (thanks to [jekyll-test](https://github.com/Floppy/jekyll-test) gem)
- 2 side menus
- customizable layout (boxes, colors)
- post pinning, with automatic de-pinning after certain number of new pinned post (default: 2)

### Dependencies:
- jekyll plugins
  - see [Gemfile](./Gemfile) for full list
- external libraries
  - [normalize.css](https://github.com/necolas/normalize.css) (8.0) ([local](./css/normalize.css))
- Google Fonts
  - [Open Sans](https://fonts.google.com/specimen/Open+Sans) font

### Usage:
To start using it, fork this repo and rename it to: 
- ```your-repository-name``` and in settings publish it from master branch
  - will be accessible at ```username.github.io/your-repository-name```
- or ```username.github.io```
  - will be accessible at ```username.github.io```

Then you need to properly change ```_config.yml```:
```yml
url: "https://username.github.io"
baseurl: /
```
If your repository is the root of your Github Pages site, or
```yml
url: "https://username.github.io"
baseurl: /your-repository-name
```
else.

Now you can custumize it (css parts are in ```_sass``` directory), clear the _posts directory and start placing your own posts in there. Few sample post are available for reference.

You can specify your post's tags in post's yaml front matter separated by space, like this:
```yml
---
tags: funny cats
---
```
Then run [this python script](https://github.com/qian256/qian256.github.io/blob/master/tag_generator.py) to generate unique site for each tag.

If you want to pin a post, set its ```pinned``` variable to true:
```yml
---
pinned: true
---
```
or to false otherwise.

### Notes
- linking to internal files by relative url (example in post by ```[article](/article)``` will cause tests to fail. If you encounter this, use absolute url.
