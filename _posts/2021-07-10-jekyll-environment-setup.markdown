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
  - `[cmd|cntr]+shift+P` -> Jekyll: Run
    - Your site should be presented [Your Site](http://localhost:4000)

#### Still working on it :-)
![](https://media.giphy.com/media/1oDwWUJWeDvyz12yWb/giphy.gif)

## Links

### Bundle CLI References

 - [Bundle install](https://bundler.io/man/bundle-install.1.html)