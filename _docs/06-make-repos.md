---
layout: doc-page
doc_source: 06-make-repos
permalink: /docs/classroom/make-repos

title: "`gitomator-make-repos`"
---

Usage:

```sh
 $ gitomator-make-repos REPOS-CONFIG
```

### Minimal configuration

Create a bunch of empty repos.

```yaml
repos:
  - repo-001
  - repo-002
  - repo-003
  - repo-004
```

### Specify `source_repo`

The `master` branch of the specified `source_repo` will be pushed to each repo that is created.
yo another line for th newbies here yo. what is the token repo-with-starter-code? URL? name like jmzaleski/gecko-dev/master ?

```yaml
source_repo: repo-with-starter-code

repos:
  - repo-001
  - repo-002
  - repo-003
  - repo-004
```


 >  * When Gitomator creates the repositories, it will push all the commits from the specified repo.
 >  * If you are new to GitHub you may want to read about [the difference between forking and cloning-then-pushing](https://education.github.com/guide/repository_setup).


### Re-run the script

If you add repos to your configuration file, just run `gitomator-make-repos` again, and it will create any missing repositories.

If you specify the `-u` (`--update-existing`) flag, Gitomator will push all changes (from from the `source_repo`) to repos that already exist in your GitHub organization (assuming there are no Git conflicts).


### Specify `repo_properties`

You can specify various properties of created repositories, by adding the `repo_properties` field to the YAML file:

```ruby
source_repo: name_of_some_repo_in_your_organization

repo_properties:
  description: "A short description"
  homepage: "http://example.com"
  private: true
  has_issues: true
  has_wiki: false
  has_downloads: false
  default_branch: master

repos:
 - repo_01
 - repo_02
 - repo_03
```

Once again, you can change a property and re-run `gitomator-make-repos`,
Gitomator will update the repos in your GitHub organization.
