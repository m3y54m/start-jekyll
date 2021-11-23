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

## Jekyll Plugins

### Jalali date

https://github.com/mehdisadeghi/jekyll-jalali

### KaTeX

There is no need to install [`jekyll-katex`](https://github.com/linjer/jekyll-katex) plugin. Just add the following lines to `_includes/head.html` according to the [KaTeX documentation](https://github.com/KaTeX/KaTeX#getting-started).

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.15.1/dist/katex.min.css" integrity="sha384-R4558gYOUz8mP9YWpZJjofhk+zx0AS11p36HnD2ZKj/6JR5z27gSSULCNHIRReVs" crossorigin="anonymous">
<!-- The loading of KaTeX is deferred to speed up page rendering -->
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.15.1/dist/katex.min.js" integrity="sha384-z1fJDqw8ZApjGO3/unPWUPsIymfsJmyrDVWC8Tv/a1HeOtGmkwNd/7xUS0Xcnvsx" crossorigin="anonymous"></script>
<!-- To automatically render math in text elements, include the auto-render extension: -->
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.15.1/dist/contrib/auto-render.min.js" integrity="sha384-+XBljXPPiv+OzfbB3cVmLHf4hdUFHlWNZN5spNQ7rmHTXpd7WvJum6fIACpNNfIR" crossorigin="anonymous"
    onload="renderMathInElement(document.body);"></script>
```

## Modify the Theme

https://github.com/jekyll/minima

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


