# Trigger Events Used

## `push` Event Activity Types & Filters

- Some events have activity types e.g pull_request has opened, closed, edited...
- Some events have filtes e.g push events filter based on target branch
- It is always good idea to look over the documentations provided by github

Activity Types Example:

```yaml
on:
  pull_request:
    types:
      - opened
      - edited
  workflow_dispatch:
```

Event Filters Example:

```yaml
on:
  push:
    branches:
      - main
      - dev-* # wildcart match example
      - feature/** # nested wildcard match
```

Filer on file paths

```yaml
on:
  paths:
```

# Cheat Sheet

- [Cheat Sheet](https://docs.github.com/en/actions/writing-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet)
