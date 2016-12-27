---
layout: doc-page
doc_source: 07-make-teams
permalink: /docs/classroom/teams

title: "`gitomator-make-teams`"
---

Usage:

```sh
 $ gitomator-make-teams TEAMS-CONFIG
```

### Minimal configuration

Specify teams (by name) and their members (e.g. GitHub usernames).

```yaml
Students:
  - Alice
  - Bob
  - Charlie
  - Dave

Teaching-Assistants:
  - Zoe
  - Ron
```

When you run `gitomator-make-teams`, Gitomator will:
 * Create all missing teams (in your GitHub organization)
 * Add all missing team memberships

 > Users who are not yet members of your GitHub organization, will automatically
   get an email invite to join.



### Specify Role

By default, team members have the `member` role, but you can specify a different
role. For example:

```yaml
Team1:
  - Alice
  - Bob
  - {Zoe: maintainer}

Team2:
  - Charlie
  - Dave
  - {Ron: maintainer}
```
