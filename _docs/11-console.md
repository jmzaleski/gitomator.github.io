---
layout: doc-page
doc_source: 11-console
permalink: /docs/console/

title: "`gitomator-console`"
---

change above jekkly?? magic so no "next" link appears 

Start an interactive Ruby shell, with pre-loaded convenience functions.

Usage:

```sh
 $ gitomator-console
```

The following functions are available at the global namespace:

### `search_repos(text)`

Search for repos whose name contains the given text (pass an empty string to list all repos).

### `delete_repo(repo_name)`


### `search_teams(text)`

Search for teams whose name contains the given `text` (pass an empty string to list all teams in your organization).

### `delete_team(team_name)`

### `list_team_members(team_name)`

### `gitomator_context`

In addition to pre-loaded convenience functions, the `gitomator_context` function will return the Gitomator context object.
This allows you to implement additional functionality using the underlying Gitomator library.

