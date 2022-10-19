# My Homepage

This `gh-pages` branch hosts the `erniewang.github.io`, which is an `A` record for my website: [erniewang.com](https://erniewang.com/).

## Local Mac Setup

Make sure correct Ruby version is installed:

    ruby -v

If it's < 3.1, follow the instructions in [here](https://jekyllrb.com/docs/installation/macos/).

Install Jekyll:

    gem install jekyll bundler

## Check out repo

    git clone git@github.com:erniewang/erniewang.github.io.git
    cd erniewang.github.io
    git checkout gh-pages
    bundle install

## serve locally

    bundle exec jekyll serve

Point the browser to 127.0.0.1:4000
