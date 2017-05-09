# pyastro17-my-first-PR
Repo for demonstrating how to make a pull request.

To make a pull request (PR):
- Fork a repo
- Clone your fork of the repo
- Create a new branch in your local repo
- Make some changes to your local branch
- Push the changes to your fork
- Create PR

## Fork a repo
Find and click the 'Fork' button in the top-right of a GitHub repo that belongs to someone else - e.g.: SolarDrew/pyastro-my-first-PR.
This will make a copy of that repo, and that copy belongs to you.

## Clone your fork of the repo
On your fork of the repo (<_your-username_>/pyastro17-my-first-PR), use the 'Clone or Download' button to download the repo.
This is the same as you've done before with any of your other repos.

### Remotes
If you run `git remote -v` in your newly-cloned repo, you should see that you have one remote called 'origin'.
Again, this is the same as when you've pushed and pulled a repo to and from your GitHub account before.
When your repo is a fork of someone else's, it's often useful to deal with that version as well as your own, in which case you may need to add it as another remote.
By convention, that remote is called 'upstream'.

## Create a new branch in your local repo
[and then a miracle occurs...]

## Make some changes to your local branch
Make some changes to some document on your local branch of the repo.
For this example, add your name and GitHub username to the contributors list in this README.md.
Commit your changes with `git add` and `git commit`.

## Push the changes to your fork
This is very similar to pushing you've done before, but now you need to take branches into account.

### `git push` syntax
Up until now we have been doing `git push origin master`.
What this actually does is tell git to push your current branch of the local repo (which has been master until this example) to the 'master' branch of the 'origin' remote.
In this case we've been working in a different branch, 'new_contributor', so we don't want to push to the master branch.
Instead we should push to the new_contributor branch on origin, if it exists.
If not, we should push to it anyway and git will create it for us, so the command is the same either way:
`git push origin new_contributor`

## Create PR
On the GitHub page for your fork of the repo, you should see drop-down menu that says 'Branch: master' and a button next to it saying 'New pull request'.
On the drop-down menu, select the new_contributor branch and then click the button.

## Contributors

- Drew Leonard (SolarDrew)
