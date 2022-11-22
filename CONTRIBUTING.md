# Second Life contribution guide

Thank you for your interest in contributing to Second Life!

## New contributor guide

To get an overview of the project, review our [Open Source Portal][portal] and
the viewer's GitHub repository. Here are some resources to help you get started
with open source contributions:

- [Finding ways to contribute to open source on GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github)
- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)
- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)

## Getting started

If you have a new feature request or technical bug report to file, you should
search for existing tickets on [Second Life's Jira][jira] and create a new
one if you can't find an existing one covering the same topic.

### Solve an issue

Search through our [existing issues](issues) to find one that interests you. You
can narrow down the search by entering keywords and filtering by labels. As a
general rule we don't assign public issues to anyone. If you can find an issue
to work on, you are welcome to open a PR with a fix.

#### Make changes to code 

1. [Install git](https://github.com/git-guides/install-git).

2. Fork the repository.
- Using GitHub Desktop:
  - [Getting started with GitHub Desktop](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/getting-started-with-github-desktop) will guide you through setting up Desktop.
  - Once Desktop is set up, you can use it to [fork the repo](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/cloning-and-forking-repositories-from-github-desktop)!

- Using the command line:
  - [Fork the repo](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo#fork-an-example-repository) so that you can make your changes without affecting the original project until you're ready to merge them.

3. If working with the viewer, follow our [build instructions](https://wiki.secondlife.com/wiki/Get_source_and_compile)

4. Create a working branch and start with your changes!

### Commit your update

Commit the changes once you are happy with them.

### Pull Request

When you're finished with the changes, create a pull request, also known as a PR.
- Fill the "Ready for review" template so that we can review your PR. This template helps reviewers understand your changes as well as the purpose of your pull request. 
- Don't forget to [link PR to issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue) if you are solving one.
- Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/allowing-changes-to-a-pull-request-branch-created-from-a-fork) so the branch can be updated for a merge.
Once you submit your PR, a viewer team member will review your proposal. We may ask questions or request additional information.
- We may ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request) or pull request comments. You can apply suggested changes directly through the UI. You can make any other changes in your fork, then commit them to your branch.
- As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
- If you run into any merge issues, checkout this [git tutorial](https://github.com/skills/resolve-merge-conflicts) to help you resolve merge conflicts and other issues.

### Your PR is merged!

Congratulations :tada::tada: The Second Life team thanks you :sparkles:. 

## Attribution

This guide is based on GitHub Docs' CC-BY licensed [instructions](https://github.com/github/docs/blob/main/CONTRIBUTING.md).

[portal]: https://wiki.secondlife.com/wiki/Open_Source_Portal
[jira]: https://jira.secondlife.com/
[jira-info]: https://wiki.secondlife.com/wiki/Bug_Tracker
[issues]: https://jira.secondlife.com/projects/BUG/issues