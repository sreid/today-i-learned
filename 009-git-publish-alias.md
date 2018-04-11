A small git alias that's a big timesaver, just add the following to your `.gitconfig` file

```
[alias]
        branch-name = "!git rev-parse --abbrev-ref HEAD"
        publish = "!git push -u origin $(git branch-name)"
```

Then pushing the current branch to origin is just a `git publish` away.

hat tip: https://gist.github.com/robmiller/6018582
