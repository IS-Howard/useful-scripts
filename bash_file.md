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

----
### File Rename Example
```SHell
#! /bin/bash

# target be like: (60)雲霄飛車殺人事件(1996年1月8日)
#IFS=$'\n' files=($(find . -type d -name '(*)*(*)'))
mapfile -t files < <(find . -type d -name '(*)*(*)')
for file in "${files[@]}"; do
  #file=${files[0]} 
  page=${file%)*(*)}
  page=${page##*(}
  name=${file%)*}
  name=${name##*(}
  nname="($page) $name"
  #echo $nname
  path=${file%/*}
  npath="$path/$nname"
  echo $file
  echo $npath
  mv "$file" "$npath"
done
```
