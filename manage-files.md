

### Removing a file added in the most recent unpushed commit
If the file was added with your most recent commit, and you have not pushed to GitHub, you can delete the file and amend the commit:


* Change the current working directory to your local repository.

To remove the file, enter `git rm --cached`:
```
$ git rm --cached giant_file
# Stage our giant file for removal, but leave it on disk
```

* Commit this change using --amend -CHEAD:

```
$ git commit --amend -CHEAD
# Amend the previous commit with your change
# Simply making a new commit won't work, as you need
# to remove the file from the unpushed history as well
```

* Push your commits to GitHub:
```
$ git push
# Push our rewritten, smaller commit
```

#### More Resources
[Removing sensitive data from a repository](https://help.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository)
[Removing files from a repository's history](https://help.github.com/en/github/managing-large-files/removing-files-from-a-repositorys-history)
