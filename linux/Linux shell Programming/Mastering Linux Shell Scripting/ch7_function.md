# clean.sh
```bash
#!/bin/bash
# Script will prompt for filename
# then remove commented and blank lines

function is_file {
    if [ ! -f "$1" ] ; then
        echo "$1 does not seem to be a file"
        exit 2
    fi
}

function clean_file {
    is_file "$1"
    BEFORE=$(wc -l "$1")
    echo "The file $1 starts with $BEFORE"
    sed -i.bak '/^\s*#/d;/^$/d' "$1"
    AFTER=$(wc -l "$1")
    echo "The file $1 is now $AFTER"
}

read -p "Enter a file to clean: "
clean_file "$REPLY"
exit 1
```


## menu2
```bash
#!/bin/bash
# Author: @theurbanpenguin
# Web: www.theurbapenguin.com
# Sample menu with functions
# Last Edited: Sept 2015
function to_lower {
    input="$1"
    output=$(tr [A-Z] [a-z] <<< "$input")
    echo $output
}

function do_backup {
    tar -czvf $HOME/backup.tgz ${HOME}/bin
}

function show_cal {
    if [ -x /usr/bin/ncal ] ; then
      command="/usr/bin/ncal -w"
    else
      command="/usr/bin/cal"
    fi
    $command
}
while true
do
  clear
  echo "Choose an item: a,b or c"
  echo "a: Backup"
  echo "b: Display Calendar"
  echo "c: Exit"
  read -sn1
  REPLY=$(to_lower "$REPLY")
  case "$REPLY" in
    a) do_backup;;
    b) show_cal;;
    c) exit 0;;
  esac
  read -n1 -p "Press any key to continue"
done


```


## pass_array
```bash
#!/bin/bash
myfunc() {
arr=$@
echo "The array from inside the function: ${arr[*]}"
}

test_arr=(1 2 3)
echo "The origianl array is: ${test_arr[*]}"
myfunc ${test_arr[*]}

```


## recursive_function
```bash
#!/bin/bash
calc_factorial() {
if [ $1 -eq 1 ]
then
echo 1
else
local var=$(( $1 - 1 ))
local res=$(calc_factorial $var)
echo $(( $res * $1 ))
fi
}
 
read -p "Enter a number: " val
factorial=$(calc_factorial $val)
echo "The factorial of $val is: $factorial"

```


## variable_scope
```bash
#!/bin/bash
myvar=10
myfunc() {
myvar=50
}
myfunc
echo $myvar

```


## variable_scope2
```bash
#!/bin/bash
myvar=30
myfunc() {
local myvar=10
}
myfunc
echo $myvar

```


##
```bash


```


##
```bash


```


##
```bash


```
