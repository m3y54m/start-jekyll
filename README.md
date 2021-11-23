# Getting Started with Jekyll

In this repository I will be sharing my journey of learning [Jekyll](https://jekyllrb.com) that I will be using to build my personal blog.

## Installation

I will follow the [Jekyll Installation Guide](https://jekyllrb.com/docs/installation/) to install Jekyll.

Version of prerequisites on my system are as follows:

- ubuntu 20.04.2 
- ruby 2.7.0p0 
- gem 3.1.2
- gcc 9.3.0
- make 4.2.1


```console
sudo apt-get install ruby-full build-essential zlib1g-dev
gem install jekyll bundler
```

## Creating a new Jekyll blog

Create a new Jekyll site at `./myblog`.

```console
jekyll new myblog
```

## Building the blog

Build the site and make it available on a local server.

```console
cd myblog
bundle exec jekyll serve
```

**Note:** Pass the `--livereload` option to `serve` to automatically refresh the page with each change you make to the source files:

```console
bundle exec jekyll serve --livereload
```

Browse to `http://localhost:4000` to see the blog.


