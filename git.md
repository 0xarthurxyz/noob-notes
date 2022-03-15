---
title: "🤷‍♂️ Git"
date: 2022-02-12T12:00:00+01:00
draft: true
showtoc: false
tags: ["git", "noob notes"]
---

### Reset remote (origin) to a specific commit

Basically:

- go onto main branch
- reset that branch to a commit locally
- force push that commit to remote (origin)

```bash
git checkout master
git reset --hard e3f1e37
git push --force origin master
```

_Source: [Stack Overflow](https://stackoverflow.com/a/17667057)_

## Submodules 

### Add submodule to repo

```bash
git submodule add <URL>
```

### Remove submodule from repo

- this command removes the reference to the submodule in .gitmodules.
- you might need to remove it from .git/config (if it still shows up)

```bash
git rm <path_to_module>
```

_Source: [Stack Overflow](https://stackoverflow.com/a/1260982)_ (linked from [Atlassian](https://www.atlassian.com/git/articles/core-concept-workflows-and-tips))
