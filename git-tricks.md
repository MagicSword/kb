# Git tricks

https://github.com/git-tips/tips

Count the commits for the branch you are on
<br>
`git rev-list --count <branch-name>|HEAD`

List authors, commit count and email 
<br>
`git shortlog --email --summary --numbered` 

Merge commits from origin/master into local master while being (possibly) in another branch
<br>
`git fetch origin master:master` 

Remove branches that have already been merged with master
<br>
`git branch --merged master | grep -v '^\*' | xargs -n 1 git branch -d`
