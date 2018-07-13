# laurengulland.github.io
Personal Website

## Set Up Instructions for Jasper + Jekyll
Pulling from information [here](https://github.com/jekyller/jasper2#deployment).

**Installations:**
```bash
$ npm install
$ sudo apt install jekyll
$ sudo apt install ruby-bundler
$ bundle install
```

At this point, I got a fatal error that it couldn't install `ffi` (version 1.9.25),
so I found [this](https://github.com/jasmine/jasmine/issues/755) that helped (instructions copied here for clarity):

```bash
$ sudo apt-get install gcc ruby ruby-dev libxml2 libxml2-dev  libxslt1-dev
$ sudo gem install ffi -v '1.9.25'
$ bundle install
```

**The command that actually runs the site locally:**
```bash
$ bundle exec jekyll serve
```
