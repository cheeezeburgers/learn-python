# learn-python

This could come in handy: https://coolestguidesontheplanet.com/syncing-github-fork-via-command-line/

## Getting git fork up and running

Fork the Repo, then:

```bash
# get the working clone to local
git clone FORKED-REPO

# make a new branch
git branch NEW-BRANCH
git checkout NEW-BRANCH

# set upstream to new branch
git push --set-upstream origin NEW-BRANCH
git push -u origin NEW-BRANCH

# add upstream (for pull-requests I think) to original repo (we forked from)
git remote add upstream LINK-TO-ORIGINAL-REPO
```

## Push and Pull between branches and Repos

### Sync forked local and remote

Now you can - after `add` & `commit` locally - `push` normally to your forked repo.

Now forked local and forked remote are in sync.

### Sync with original repo

Then you can simply: `hub pull-request --browse -m "Title"` to create a pull request at the original repo.

You can only have one active pull request at a time so changes have to wait to accept or deny the active PR.

> You can check on existing pull requests with `hub pr show`. 

## Update the forked master from the original repo

So in the next you can switch back to `master` and ~~fetch~~ **pull** the new version of the original repo.

```bash
git pull upstream master
git push		# don't forget to push back to your repo
```

> You can work with a new brach for changes if you like but you can continue working with the old one, too – **as long you have the last pull request merged or denied!**
