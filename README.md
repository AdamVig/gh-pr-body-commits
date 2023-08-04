# gh-pr-body-commits

A GitHub (`gh`) CLI extension to add a commit log to a pull request's body.

- When no pull request is detected, the commit log will be printed to the console and can be piped to other commands.
- When an existing pull request is detected, the body will be updated with the latest commit log, using the base of the pull request if a base is not provided.
- Uses hidden markers in the pull request body to avoid overwriting any content other than the commit log.
- Uses the repository's default branch when a base branch is not provided.

## Installation

1. [Install the GitHub CLI](https://github.com/cli/cli#installation).

2. Install the extension.
   ```shell
   gh extension install AdamVig/gh-pr-body-commits
   ```

## Usage

```shell
# In a GitHub repository

# To create a new pull request
gh pr-body-commits | gh pr create --body-file='-'

# To update an existing pull request
gh pr-body-commits

```
