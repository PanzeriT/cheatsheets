---
title: "GitHub CLI"
date: 2023-05-25T07:14:05
author: Thomas Panzeri
---

## Basic Commands

{{< cheatitems >}}
gh auth login | logs you in to your GitHub account and stores your authentication credentials locally.
gh repo create | creates a new repository on GitHub and initializes it with a README file.
gh repo clone [repository] | clones a remote repository to your local machine.
gh issue create | creates a new issue on GitHub.
gh pr create | creates a new pull request on GitHub.
gh pr checkout [pull request] | checks out the specified pull request locally.
gh pr merge [pull request] | merges the specified pull request into the base branch.
gh pr list | lists all open pull requests for the current repository.
{{< /cheatitems >}}

## Branching

{{< cheatitems >}}
gh repo fork | forks the current repository on GitHub.
gh repo clone [repository] --fork | clones a forked repository to your local machine.
gh repo fork --clone | forks the current repository on GitHub and clones it to your local machine.
{{< /cheatitems >}}
gh repo view | displays information about the current repository.

## Collaborating

{{< cheatitems >}}
gh collaborator add [username] | adds the specified user as a collaborator on the current repository.
gh collaborator remove [username] | removes the specified user as a collaborator on the current repository.
gh issue assign [issue] [username] | assigns the specified issue to the specified user.
gh issue close [issue] | closes the specified issue on GitHub.
{{< /cheatitems >}}

## Workflows

{{< cheatitems >}}
gh workflow run [workflow] | runs the specified GitHub Actions workflow.
gh secret set [name] | sets a secret for use in GitHub Actions workflows.
gh secret list | lists all secrets for the current repository.
{{< /cheatitems >}}
