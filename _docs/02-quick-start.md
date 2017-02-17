---
layout: doc-page
doc_source: 02-quick-start
permalink: /docs/quick-start/

title: "Quick-Start"
excerpt: "Getting started with Gitomator"
---

## Dependencies

Make sure the dependencies are installed.

 * [Ruby](https://www.ruby-lang.org/en/downloads/) (Gitomator is developed and tested on version 2.2)
 * [Ruby Gems](https://rubygems.org/pages/download)
 * [Bundler](http://bundler.io/)

## Installation

```sh
gem install gitomator
```


## Configure Credentials

Create a [YAML](https://en.wikipedia.org/wiki/YAML) configuration file called `.gitomator` *in your home directory*.

```ruby
hosting:
  provider: github
  access_token: YOUR-GITHUB-ACCESS-TOKEN
  organization: YOUR-GITHUB-ORGANIZATION

ci:
  provider: travis_pro
  access_token: YOUR-TRAVIS-CI-ACCESS-TOKEN
  github_organization: YOUR-GITHUB-ORGANIZATION
```

 >  * You can read more about how to [create an access token on GitHub](https://github.com/blog/1509-personal-api-tokens).
 >  * If you don't use Travis CI, feel free to omit the `ci` configuration
 >  * You can specify a different path (other than `~/.gitomator`) for your configuration file, by setting the `GITOMATOR_CONTEXT` environment variable.
 >  * **Important:** Keep your credentials safe!      
      The `.gitomator` file is local to your machine, and should *not* be committed to version control.
