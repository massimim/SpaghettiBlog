---
layout: post
title: Jekyll Local Server
subtitle: how to install, update, run
tags: [Jekyll, blog]
comments: false
---

How to install jekyll: 

```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
gem install jekyll bundler
```

To configure the blog, run the following from the blog root diretory:

```bash
bundle install # only once
bundle update jekyll # only when some configurations are changed 
bundle exec jekyll serve # to run the server locally
```
