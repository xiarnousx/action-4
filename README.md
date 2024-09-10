# Trigger Events Used

## `push` Event Activity Types & Filters

- Some events have activity types e.g pull_request has opened, closed, edited...
- Some events have filtes e.g push events filter based on target branch
- It is always good idea to look over the documentations provided by github

Activity Type Example:

```yaml
on:
  pull_request:
    types:
      - opened
      - edited
  workflow_dispatch:
```
