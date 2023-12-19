# Technical Report Template

## Installation

1. Install [`latex-styles`](https://github.com/dpo/latex-styles) and set up environment variables.
2. Fork this repository to your GitHub account. 
3. Clone your fork with `git clone https://github.com/<your-github-id>/report.git`.
4. Add the original repository as a remote so you can pull updates in the future with `git remote add upstream https://github.com/dpo/report.git`.
5. Install the git hooks with `cp .config/hooks/* .git/hooks/ && chmod +x .git/hooks/*`.

## GitHub Actions

In order for GitHub Actions to work properly, set the following permissions in your fork's settings, under Actions > General:

* Check *Action permissions > Allow all actions and reusable workflows*.
* Check *Workflow permissions > Read and write permissions*.
* Check *Allow GitHub Actions to create and approve pull requests*.

## Updating Workflows

If you can think of useful improvements to the GitHub Actions workflows, please open a pull request against https://github.com/dpo/report.git.

When updates are available at https://github.com/dpo/report.git, incorporate them into your fork as follows:

```shell
> git fetch upstream
> git checkout main
> git rebase upstream
```

