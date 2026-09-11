# go-fileshare.github.io

The landing page for [go-fileshare](https://github.com/go-fileshare), built
with Hugo and deployed by GitHub Actions.

⚠ Pages must be set to **build from the workflow**, not from a branch:

```sh
gh api -X PUT repos/go-fileshare/go-fileshare.github.io/pages -f build_type=workflow
```

A repository left on the default (legacy Jekyll) builder publishes this
README **over** the Hugo output while the deploy workflow reports success —
which is precisely what happened to a sibling org for a week, and is checked
here by looking at the live page's `generator` meta rather than at the
workflow's green tick.
