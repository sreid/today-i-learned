# JQ: Command Line JSON Manipulation

Frequently, you'll end up with JSON in a file, and either need to take a quick look at some portion of it, or feed parts of it into another command. The `jq` command line tool to the rescue! `jq` offers a simple syntax for parsing out a portion or even transforming one JSON doc into another.

Example: Print just the name of all your Lambda functions on AWS

```
aws lambda list-functions | jq -r '.["Functions"][] | .FunctionName'
```

Useful options:
```
-r : raw output mode, drops extra quotes for easier piping 
```

Installable via `brew install jq` or find out more here: https://stedolan.github.io/jq/ and also a online playground tool for easy testing: https://jqplay.org/
