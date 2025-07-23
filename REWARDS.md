**Welcome to Second Life's Reward Program!** We use the [Opire platform][opire] to offer monetary rewards (bounties) on certain GitHub issues. This document supplements our general [CONTRIBUTING][] guidelines and [Code of Conduct][conduct], explaining how to participate in reward issues (both feature requests and bug fixes) and what we expect from contributors.

## Scope of Rewards

Our bounties can apply to any type of issue. If an issue has an associated reward, it will typically be noted by the Opire bot (e.g. a comment indicating a reward) or the label `💎 reward`. Keep an eye out for these and feel free to tackle them if you’re interested and capable. All the usual contribution rules apply, with a few extra steps for claiming rewards (detailed below).

## How to Claim a Reward (Process)

1. **Find a Reward Issue:** Look for open issues with bounties (the Opire bot may comment with a reward amount). Choose an issue you want to work on and make sure no one else is already exclusively assigned (see Exclusive Windows below).
2. **Ask for Clarification if Needed:** If anything about the issue is unclear, please ask questions first by commenting on the issue. It’s better to clarify requirements up front than to do rework later. Maintainers are happy to provide guidance to ensure you’re on the right track.
3. **Announce Your Intent:** To avoid duplicate efforts, let others know you’re working on the issue. You can simply comment that you plan to work on it, or use the Opire command /try on the issue to signal that you intend to solve it. (If you’re not the first to try, Opire will list others who are also attempting the issue, so you can coordinate or be aware.) Announcing your intent is not required, but it’s strongly encouraged: it helps maintainers and other contributors know the issue is being actively worked on.
4. **Respect Exclusive Windows:** In some cases, a maintainer might grant a contributor an exclusive time window to work on a reward issue. This is to prevent multiple people doing redundant work. If we decide to do this, we will leave a comment on the issue explicitly stating who has exclusive rights and until what date/time. (There’s no special command or bot status for this: we’ll communicate it in the comments.) Please respect these exclusive blocks: if someone else has an active exclusive window on the issue, do not start work on it until that period expires or the maintainer opens it up again. Conversely, if you’ve been given an exclusive window but can’t continue, let us know so we can release the issue to others.
5. **Develop Your Solution:** Fork the repository and implement the needed changes to fix the bug or implement the feature. Follow our coding standards and make sure your solution addresses all acceptance criteria. This includes writing or updating tests and documentation if applicable. Aim to write clean, readable code that fits with the project’s style.
6. **Submit a Pull Request:** Once your changes are ready:
    1. **Title & Description:** Open a PR with a clear title and description of your changes. Reference the issue number (e.g., "Fixes #123") so it links to the reward issue.
    2. **Demo Video:** Include a short demo video in your PR description demonstrating your changes in action (for example, a quick screencast or animated GIF). This is required to claim the reward: it allows us to quickly verify the functionality you’ve added or fixed. A 30-60 second video showing the feature or bug fix is usually sufficient.
    3. **Claim the Reward:** In the PR description or as a comment on your PR, use the Opire command to claim the reward for the issue. For example, if the issue is #123, comment /claim #123. This will notify the reward creators (sponsors) that you believe the issue is resolved and are claiming the reward. (The Opire bot only recognizes this command when creating a PR or comment, not edits        , so make sure to do it in a new comment or in the initial PR message.)
7. **Follow Up:** After submitting, keep an eye on your PR for feedback or review comments. Be ready to make revisions if the maintainers request changes. Prompt responses and updates will help get your contribution merged faster, which is also in your interest for receiving the reward.

## Pull Request Quality Standards

Because reward issues come with monetary compensation, we have high standards for accepting these PRs. Low-effort or low-quality submissions will be declined. To ensure your pull request meets our expectations, please follow these guidelines (in addition to our normal [CONTRIBUTING][] rules):

- **Complete Solution:** The PR should fully resolve the issue and add value: it needs to be a complete piece of work, not a half-done fix or a workaround. Make sure you’ve addressed the root problem and met the requirements outlined in the issue.
- **Clear Title and Description:** Write a descriptive PR title and include a summary in the description that provides context. Reviewers should understand what your change is and why it’s needed by reading your PR description. If the issue is complex, explain your approach or solution briefly in the PR body.
- **Well-Structured Commits:** Craft your commits carefully. Each commit should have a meaningful message explaining the change. We prefer a tidy commit history that "tells the story" of the development. Use multiple commits if it makes sense to logically separate changes, or squash into one commit if it’s a small change: but avoid messy commit history (e.g. fix-up commits for typos or merge noise). A reviewer (or future maintainer) should be able to read your commits and understand the progression of the fix.
- **Focused and Manageable:** Keep the PR focused on the single issue or feature at hand. Avoid introducing unrelated changes. Ideally, a reward PR should be relatively small and easy to review. Large PRs can be overwhelming and may take longer to review (or even be rejected for being too broad). If you find the fix requires an enormous change, consider discussing with maintainers first or breaking it into smaller parts.
- **Code Quality and Best Practices:** Ensure your code meets our project’s coding standards and best practice. This includes proper formatting, following naming conventions, adding or updating unit tests if the project requires it, and not introducing new bugs or security issues. We hold reward contributions to the same quality bar as any other code in the project.
- **No Low-Quality Submissions:** Do not submit throwaway or spammy PRs just to claim a reward. If a PR is clearly low-effort, doesn’t follow these guidelines, or doesn’t actually solve the issue, we will decline it. Repeated low-quality contributions may get you disqualified from future bounties. It’s not first-come-first-served: it’s first high-quality solution wins.

*(For a deeper understanding of what we consider a "good PR," you can refer to Mike Pea’s ["Pull Request Etiquette" guide][pr-etiquette], which inspired many of the points above.)*

## Using Opire (Rewards Platform)

All our bounties are managed through the Opire platform and its GitHub bot integration. You do not need to leave GitHub or have a separate account just to start working on a reward: commenting with commands like /try or /claim will interface with Opire automatically. However, to receive payments, you’ll eventually need to log in to Opire and set up a payout method:

- **Account Setup:** If you haven’t used Opire before, the first time you interact (e.g. use `/try` or `/claim`), an Opire account is created for you behind the scenes (linked to your GitHub). We recommend you log in to Opire at some point to configure your settings. In particular, set up your Stripe account for payouts. This is required to receive your reward: if your payment info isn’t configured, the reward sponsors won’t be able to pay you. You can find this in your Opire dashboard under settings.
- **Commands Recap:** The key commands are:
  - `/reward [amount]`: (Used by maintainers or any user to put up a bounty on an issue. You don’t need this as a reward hunter, but you might see it in issue comments.)
  - `/try`: Use this in an issue comment to say "I’m going to try solving this." This lets the bot (and everyone watching) know you’re on it.
  - `/claim #[issue]`: Use this in a pull request comment or description to claim the reward for that issue once your PR is ready. For example, `/claim #123` in your PR will signal that you believe issue #123 is fixed by your PR and will trigger the review/payment workflow.
  - `/tip [amount] @user`: (Optional) If you want to thank another user, you or others can tip via this command. This isn’t directly part of the reward process, but a nice gesture if someone helped you.
- **Opire Dashboard:** You can also use Opire’s web dashboard to track rewards. If for some reason the bot isn’t responding, you can claim or manage rewards through the website as a fallback. But in most cases, interacting via GitHub comments is sufficient and easier.

## Communication Channels

We encourage open collaboration and are happy to support contributors through a variety of channels. Whether you have a question, need feedback, or want to engage with other developers, here’s where to reach us:

- **Official Discord:** Join the [Second Life Official Discord][discord] and visit the **#open-source-general** channel to chat with other contributors and maintainers in real time.
- **GitHub Issues and Pull Requests:** Comment directly on issues or pull requests to ask for clarification, provide updates, or coordinate with others. We monitor these actively.
- **GitHub Discussions:** Use our [GitHub Discussions][discuss] board to propose ideas, get help, or talk through technical challenges with the community.
- **Mailing List:** For more traditional communication, we also maintain the [OpenSource-Dev mailing list][mail]. This is a good option for longer-form technical discussions or announcements.

## Final Notes

By participating in our reward program, you agree to abide by all the rules laid out here, as well as our general [contribution][contributing] guidelines and [Code of Conduct][conduct]. We want this to be a positive experience for everyone: our goal is to get quality contributions to the project and reward developers for their valuable work.

If you have any questions about the process or a specific reward, please don’t hesitate to ask a maintainer or comment on the issue. We’re here to help. Thank you for contributing to Second Life, and good luck: we look forward to reviewing your pull requests!

[opire]: https://opire.dev
[contributing]: https://github.com/secondlife/.github/blob/main/CONTRIBUTING.md
[conduct]: https://github.com/secondlife/.github/blob/main/CODE_OF_CONDUCT.md
[pr-etiquette]: https://gist.github.com/mikepea/863f63d6e37281e329f8
[discord]: https://discord.gg/secondlifeofficial
[discuss]: https://github.com/secondlife/viewer/discussions
[mail]: https://wiki.secondlife.com/wiki/OpenSource-Dev
