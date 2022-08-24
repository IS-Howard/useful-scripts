# Example of create bash script
https://www.freecodecamp.org/news/shell-scripting-crash-course-how-to-write-bash-scripts-in-linux/

* find bash path
```Shell
which bash
```
ex : usr/bin/bash

* creat file
```Shell
touch 1.sh
vim 1.sh
```

edit 1.sh

* example shell for 1.sh
```Shell
#! usr/bin/bash
echo "Hello World"
```

* exacute
```Shell
//provide rights to user(u), execute(x)
chmod u+x hello_world.sh
bash hello_world.sh or ./hello_world.sh
```
