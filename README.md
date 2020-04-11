# learn-python

This could come in handy: https://coolestguidesontheplanet.com/syncing-github-fork-via-command-line/

## Getting git fork up and running

Fork the Repo, then:

```bash
git clone FORKED-REPO

git branch NEW-BRANCH
git checkout NEW-BRANCH

git push --set-upstream origin NEW-BRANCH
git push -u origin NEW-BRANCH

git remote add upstream LINK-TO-ORIGINAL-REPO
```

Then you can simply: `hub pull-request`

This means you can only merge this branch once. So, that means I have to make date specific branches every time I start learning...

So in the next you can switch back to `master` and fetch the new version of the original repo.

Work with a new branch for changes.
