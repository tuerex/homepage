homepage [![Build Status](https://travis-ci.org/pep-dortmund/homepage.svg?branch=master)](https://travis-ci.org/pep-dortmund/homepage)
=====================

Repository of the PeP al. homepage (<https://pep-dortmund.org>).

## Contributing

See [Contributing](CONTRIBUTING.md) for detailled explanation how to
- write new posts
- add static pages
- edit the navigation
- minified markdown intro
- other crazy things


## Local Testing

It is advisable, that you test the website locally if you make any changes or review Pull Requests

### Install the required software

#### Ubuntu

```
$ sudo apt install ruby-dev nodejs-legacy libxml2-dev libxslt-dev
$ sudo gem install bundler
```

#### ArchLinux

```
$ sudo pacman -S ruby nodejs libxml2 libxslt
$ sudo gem install bundler
```

#### macOS
```
$ brew install ruby node
$ gem install bundler
```

### Testing
Go to the base directory of this repository.

First install all required gems
```
$ bundle install --path vendor/bundle
```

In order to test the site at this point, simply run

```bash
$ bundle exec jekyll serve
```
The website is then served at [localhost:4000](http://localhost:4000).
Changes to the inputfiles are recognised and the website is build again,
press f5 in the browser to update.

Some updates, like changing images might require to delete the cache (ctrl + r in chrome).
