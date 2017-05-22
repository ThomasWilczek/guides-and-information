# How we use git
1. Fork the repository you want to work on.
2. Set up your remotes so that they look like this.  
````
$ git remote -v
origin  git@github.com:dreisen/guides-and-information.git (fetch)
origin  git@github.com:dreisen/guides-and-information.git (push)
upstream        git@github.com:Crankenhaus/guides-and-information.git (fetch)
upstream        git@github.com:Crankenhaus/guides-and-information.git (push)
````
3. Make sure you are on your local master branch and sync it with the `upstream`.  
````
git checkout master
git fetch upstream
git rebase upstream/master
````
4. Create a new branch to work on.  
`git checkout -b my_feature`
5. Commit changes on your feature_branch.
6. Rebase your changes ontop of the upstream.  
`git rebase upstream/master`
7. Push your commits to your fork (`origin`).  
`git push origin my_feature`
8. Open a pull request on the original repository (`upstream`).  
In the pull request, link your issue or describe your feature. Explain why you changed something.
9. If you need to make changes to your pull request, push these changes to your local branch `origin`.  Then they will be automatically added to the pull request.
10. If your pull request is closed (accepted or rejected), you can delete your local branch.

# Notes
* Please don't merge your own Pull Requests.
