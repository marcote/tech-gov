# Contribution and Pull Requests Etiquette

Pull Requests (PR) are the fundamental unit of how we progress change and the vehicle to deliver value and new features to our users.
A good Pull Request should match a task from the backlog, and it should take 2 or 3 days of effort to complete it. 
If your PR takes more time, it means your taks could be decomposed into smaller tasks. The smaller the tasks, the smaller the PR, hence easier to review the code. Not to mention it will be easier to revert if something goes wrong. It's not easy at the beginning, but the reviewers (remember, you're one of them!) will thank you.

Design discussions should be taken outside the scope of the PR. While yes, in the Open Source world, the PR is the place to have design and code style discussions, we work at same team and for the same company. If we're having too many design discussions in a PR, this means we haven't designed our feature correctly and haven't asked for feedback from more experienced team members in advanced. If this happens, please talk with your team members. Not only its a great way to understand the existing codebase, good communication is essential for a healthy and productive team.

## Pull Requests Traits

| Trait                          | Value             |
| ------------------------------ | ----------------- |
| Creation/work time             | 2 - 3 days aprox. |
| Time to review a PR            | 1 day             |
| # of approvals needed to merge | 2                 |
| Suggested # of files per PR    | < 10              |

## What constitutes a good PR?

A good quality PR will have the following characteristics:

  - It will be a complete piece of work that adds value in some way. 
  - It will have a title that reflects the work within, and a summary that helps to understand the context of the change.
  - There will be well written commit messages, with well crafted commits that tell the story of the development of this work.
  - Ideally it will be small and easy to understand. Single commit PRs are usually easy to submit, review, and merge.
  - The code contained within will meet the best practices set by the team wherever possible.

A PR does not end at submission though. A code change is not made until it is merged and used in production.
A good PR should be able to flow through a peer review system easily and quickly.

### Discussions

- Discussions **must be kept polite** and every remark should be well received. No exceptions.
- No linting discussions, unless stricly necessary. Make sure to format your code before submitting any file
- Remarks on good code and practices are encouraged
  - Must be resolved by the PR owner. If the error persists it should be remarked in a new review
  - Be a good team player and show valid arguments 
  
### Further Considerations

- Drafts can also be reviewed, though it is not enforced and the rules above do not apply
- Only the Owner is responsible to merge the PR
- Remote branches must be deleted upon merge
- No orphan PRs, always assign yourself when creating a PR
- Every request for review should be fulfilled
- Merged branches must be deleted. No orphan or stale branches should be allowed.
- Assign 2+ reviewers to every PR

## Guidelines 

### Everyone

* Accept that many programming decisions are opinions. Discuss tradeoffs, which
  you prefer, and reach a resolution quickly.
* Remember that you are here to provide feedback, not to be a gatekeeper.
* Ask good questions; don't make demands. ("What do you think about naming this
  `:user_id`?")
* Good questions avoid judgment and avoid assumptions about the author's
  perspective.
* Ask for clarification. ("I didn't understand. Can you clarify?")
* Avoid selective ownership of code. ("mine", "not mine", "yours")
* Avoid using terms that could be seen as referring to personal traits. ("dumb",
  "stupid"). Assume everyone is intelligent and well-meaning.
* Be explicit. Remember people don't always understand your intentions online.
* Be humble. ("I'm not sure - let's look it up.")
* Don't use hyperbole. ("always", "never", "endlessly", "nothing")
* Don't use sarcasm.
* Keep it real. If emoji, animated gifs, or humor aren't you, don't force them.
  If they are, use them with aplomb.
* Talk synchronously (e.g. chat, screensharing, in person) if there are too many
  "I didn't understand" or "Alternative solution:" comments. Post a follow-up
  comment summarizing the discussion.

### Having Your Code Reviewed

* Be grateful for the reviewer's suggestions. ("Good call. I'll make that
  change.")
* A common axiom is "Don't take it personally. The review is of the code, not you." We used to include this, but now prefer to say what we mean: Be aware of [how hard it is to convey emotion online] and how easy it is to misinterpret feedback. If a review seems aggressive or angry or otherwise personal, consider if it is intended to be read that way and ask the person for clarification of intent, in person if possible.
* Keeping the previous point in mind: assume the best intention from the reviewer's comments.
* Explain why the code exists. ("It's like that because of these reasons. Would
  it be more clear if I rename this class/file/method/variable?")
* Extract some changes and refactorings into future tickets/stories.
* Link to the code review from the ticket/story. ("Ready for review:
  https://github.com/organization/project/pull/1")
* Push commits based on earlier rounds of feedback as isolated commits to the
  branch. Do not squash until the branch is ready to merge. Reviewers should be
  able to read individual updates based on their earlier feedback.
* Seek to understand the reviewer's perspective.
* Try to respond to every comment.
* Wait to merge the branch until continuous integration (Jenkins, Travis CI,
  CircleCI, etc.) tells you the test suite is green in the branch.
* Merge once you feel confident in the code and its impact on the project.

[how hard it is to convey emotion online]: https://www.fastcodesign.com/3036748/why-its-so-hard-to-detect-emotion-in-emails-and-texts

### Reviewing Code

Understand why the change is necessary (fixes a bug, add value to the users, refactors the existing code). Then:

* Communicate which ideas you feel strongly about and those you don't.
* Identify ways to simplify the code while still solving the problem.
* If discussions turn too philosophical or academic, move the discussion offline
  to a regular Friday afternoon technique discussion. In the meantime, let the
  author make the final decision on alternative implementations.
* Offer alternative implementations, but assume the author already considered
  them. ("What do you think about using a custom validator here?")
* Seek to understand the author's perspective.
* Sign off on the pull request with a :thumbsup:, "LGTM" (looks good to me) or "Ready to merge" comment.
* Remember that you are here to provide feedback, not to be a gatekeeper.

## Keep the flow going

If PRs are getting clogged up in the system, either unreviewed or unmanaged, they are preventing a piece of work from being completed.

As PRs clog up in the system, merges become more difficult, as other features and fixes are applied to the same codebase. This in turn slows them down further, and often completely blocks progress on a given codebase.

There is a balance between flow and ensuring the quality of our PRs. As a reviewer you should make a call as to whether a code quality issue is sufficient enough to block the PR whilst the code is improved. Possibly it is more prudent to simply flag that the code needs rework, and raise an issue.

Any quality issue that will obviously result in a bug should be fixed.

If you disagree with a guideline, open an issue on the guides repo rather than
debating it within the code review. In the meantime, apply the guideline.


### Referencias
https://gist.github.com/mikepea/863f63d6e37281e329f8

https://github.com/thoughtbot/guides/tree/master/code-review 
