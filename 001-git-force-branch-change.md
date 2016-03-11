# Git: Force Branch Change without Checkout

`git reset --hard` is a common action to force a branch to a different commit. But it only works if you've checked out the branch you're changing. If you want to change the branch without checking it out first, try:

`git branch -f branch_to_change new_ref_to_point_to`

Hat Tip: http://stackoverflow.com/a/1591255
