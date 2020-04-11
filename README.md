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

Does this mean you can only merge this branch once? If so, than I have to make date specific branches every time I start learning...
