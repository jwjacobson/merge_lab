# Merge Lab
## Understanding merge commits, squash merging, and rebasing

While working through Adam Johnson's excellent [Boost your Git DX](https://adamchainz.gumroad.com/l/bygdx), I decided to make a repo to help solidify how the different merging strategies work. I created and modified some trivial files through three different PRs, merging each using one of the strategies.

Here is a summary of my findings:

### Merge commit
Commits from the feature branch appear sequentially in the main branch's commit history, plus an extra Merge commit that shows all the changes together.

### Squash merge
Only the squash merge commit appears in the main branch's commit history (no individual commits from the feature branch); however, by default, it will include each individual commit message in the details when you click on it.

### Rebase
Only the individual commits from the feature branch appear in the main branch's commit history (no merge commit); the original commit time is also lost, as each commit is dated to the time of rebase.

You can check the [commit history](https://github.com/jwjacobson/merge_lab/commits/main/) to see how these work in detail, but it will probably be more tangible for you if you create your own repo and try this out yourself.