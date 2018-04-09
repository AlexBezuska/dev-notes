# Bash

### Create a symlink

```
ln -s /any/file/on/the/disk linked-file
```


### Making a script file executable

- First line of file should be `#!/bin/sh` 

- Permissions shoudl be set to 755 `sudo chmod 755 myscript.sh`
  - This allows the file to be executable by bash: `./myscript.sh` or `./myscript` instead of `sh myscript.sh`
