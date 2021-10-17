---
layout: post
title:  "Jekyll Blogging Using Minimal Setup"
date:   2021-07-11
categories: jekyll setup development environment
tag: ide
---

## TLDR;

- [Development in Containers](https://code.visualstudio.com/docs/remote/containers) 
  - [Quick Start](https://code.visualstudio.com/docs/remote/containers#_quick-start-open-an-existing-folder-in-a-container)
    - `NOTE:` Select Show All then select Ruby
    - `.devcontainer/devcontainer.json`
    ```json
        ...
        "extensions": [
          "rebornix.Ruby",
          "ginfuru.vscode-jekyll-snippets",
          "dedsec727.jekyll-run",
        ],
        "postCreateCommand": "gem install jekyll bundler && bundler install",
    ```
  - Start Remote Container
    - Steps here
  - Create new blog
    - `jekyll new .`
  - Update `Gemfile`
  ```ruby
    ...
    gem "webrick", "~> 1.7"
  ```
  - `[cmd|ctr]+shift+P` -> Jekyll: Run
    - Your site should be presented [Your Site](http://localhost:4000)
  - Update `_config.yml` with information
  - Create new post
    - > `touch _posts/Year-Month-Day-title.md` \
      > [Layout](https://jekyllrb.com/docs/posts/) 
  - Create github account 
  - Log in and create repository
  - Clone repository
  - Copy project into repository
  - Commit and push
  - Go to repository settings -> Pages 
    - source -> Branch master -> / (root)
    - if you don't have a custom domain use the username.github.io
  - Select Enforce HTTPS
  - New browser and navigate to username.github.io

#### Still working on it :-)
![](https://media.giphy.com/media/1oDwWUJWeDvyz12yWb/giphy.gif)

## Links

### Bundle CLI References

 - [Bundle install](https://bundler.io/man/bundle-install.1.html)