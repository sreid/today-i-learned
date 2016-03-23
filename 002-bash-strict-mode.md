Save yourself a lot of hassle when writing shell scripts by adding the following to the top of the file:

```
#!/bin/bash
set -euo pipefail
IFS=$'\n\t'
```

```
-e: stop if a command fails
-u: error on undefined variable
-o pipefail: show errors that occur when piping one command to another
```

Hat tip and more details: http://redsymbol.net/articles/unofficial-bash-strict-mode/
