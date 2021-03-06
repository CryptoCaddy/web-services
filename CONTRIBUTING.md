# Contributing to CryptoCaddy

Contributions to CryptoCaddy could come in different forms. Some contribute code
changes, some provide relevant tax and accounting information, while others contribute docs etc.

We welcome all contributions from folks who are willing to work in good faith
with the community. No contribution is too small and all contributions are
valued.

* [Discussions And General Help](#discussions-and-general-help)
* [Issues](#issues)
* [Pull Requests](#pull-requests)
  * [Step 1: Fork](#step-1-fork)
  * [Step 2: Branch](#step-2-branch)
  * [Step 3: Code](#step-3-code)
  * [Step 4: Commit](#step-4-commit)
  * [Step 5: Rebase](#step-5-rebase)
* [Code of Conduct](#code-of-conduct)




## Issues
Issues in `CryptoCaddy/web-app` are the primary means by which bug reports and
general discussions are made. 

## Discussions And General Help
Go to our [slack](https://cryptocaddy.slack.com/) for the most recent project information and for more in depth discussion or help.

## Pull Requests
Pull Requests are the way in which concrete changes are made to the code and
documentation.

### Step 1: Fork

Fork the project on [GitHub](https://github.com/cryptocaddy/web-app) and clone your
fork locally.

Once forked, follow these instructions to clone your forked branch.

```text
$ git clone git@github.com:username/web-app.git
$ cd web-app
$ git remote add upstream https://github.com/cryptocaddy/web-app.git
$ git fetch upstream
```

### Step 2: Branch

It's always better to create local branches to work on a specific issue. Makes
life easier for you if you are the kind who enjoys multiple things parallely.
These should also be created directly off of the `master` branch.

```text
$ git checkout -b my-branch -t upstream/development
```

### Step 3: Code

As of now, we don't have any sort of design style / lint to validate things.
So we ask you to ensure all these are met before you shoot out a PR.
- Avoid trailing whitespace & un-necessary white lines
- Indentation is as follows
  - 1 tab = 2 spaces for `.html` files
  - 1 tab = 4 spaces for everything else
  - __Linters will be added to make this easier.__

### Step 4: Commit

1. List all your changes as a list if needed else simply give a brief
  description on what the changes
2. All lines at 100 columns.
3. If your PR fixed an issue, Use the `Fixes:` prefix and the full issue URL.
  For other references use `Refs:`.

   _Examples:_
   - `Fixes: https://github.com/cryptocaddy/web-app/issues/1`
   - `Refs: https://github.com/cryptocaddy/web-app/issues/1`

4. _Sample commit A_
   ```txt
   if you can write down the changes explaining it in a paragraph which each
   line wrapped within 30 lines.

   Fixes: https://github.com/cryptocaddy/web-app/issues/1
   Refs: https://github.com/cryptocaddy/web-app/issues/1
   ```

   _Sample commit B_
   ```txt
   - list out your changes as points if there are many changes
   - all wrapped within 30 lines

   Fixes: https://github.com/cryptocaddy/web-app/issues/1
   Refs: https://github.com/cryptocaddy/web-app/issues/1
   ```
5. [Squashing](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History) and
   [Merging](https://git-scm.com/docs/git-merge) your commits to make our
   history neater is always welcomed.

### Step 5: Rebase

Ensure you neat description on what your PR is for, so that it's
easier for folks to understand the gist of it without before jumping to the
the code / doc.

As a best practice, once you have committed your changes, it is a good idea
to use `git rebase` (not `git merge`) to ensure your changes are placed at the
top. Plus merge conflicts can be resolved

```text
$ git fetch upstream
$ git rebase upstream/development
```


## Code of Conduct
CryptoCaddy [Code of Conduct](https://github.com/CryptoCaddy/web-app/blob/master/.github/CODE_OF_CONDUCT.md).

## Acknowledgement
The [Gitcoin contributing file](https://github.com/gitcoinco/web/blob/master/docs/CONTRIBUTING.md) was used as a template for this file.
