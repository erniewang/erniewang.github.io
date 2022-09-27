# how to set up github-page as homepage

On Ubuntu:

    sudo apt install build-essential ruby-dev
    sudo gem install jekyll bundler

From empty repo:

    git checkout --orphan gh-pages  # create new branch
    jekyll new --skip-bundle .   # init jekyll
    vi Gemfile  # comment out jekyll, uncomment github-pages
    bundle add webrick
    bundle install

Use a different theme:

    vi _config.yml  # default is minima, we use cayman
    rm -fr _posts/  
    mv index.markdown index.md
    vi index.md

test locally:

    bundle exec jekyll serve

Open browser window of `127.0.0.1:4000` to see result.

Add, commit, push.
