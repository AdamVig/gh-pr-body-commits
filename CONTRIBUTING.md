# Contributing

After cloning the repository, run:
```shell
gh extension remove gh-pr-body-commits
gh extension install .
```

From now on, `gh watch` will run the code in your local clone of the repository.

To revert back to the published version, run:
```shell
gh extension remove gh-pr-body-commits
gh extension install AdamVig/gh-pr-body-commits
```
