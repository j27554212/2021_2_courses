#
```
#!/bin/bash
cur_dir=`pwd`
echo $cur_dir

#!/bin/bash
myarr=(one two three four five)
echo ${myarr[1]} #prints two which is the second element

#!/bin/bash
echo "You are using $(basename $0)"
echo "Hello $*"
exit 0

#!/bin/bash
myarr=(one two three four five)
echo ${myarr[*]}

#!/bin/bash
myarr=(one two three four five)
unset myarr[1] #This will remove the second element
unset myarr    #This will remove all elements


#!/bin/bash
name="Mokhtar"
age=35
total=16.5
echo $name  #prints Mokhtar
echo $age   #prints 35
echo $total #prints 16.5


# The first script
#!/bin/bash
name="Mokhtar"
export name # The variable will be accessible to other processes
./06-script2.sh


# The script2.sh script
#!/bin/bash
echo $name
```

## ch6 loop
```
#!/bin/bash
for var in one "This is two" "Now three" "We'll check four"
do
echo "Value: $var"
done

#!/bin/bash
a=$(( 2 + 3 ))
echo $a


#!/bin/bash
for path in /home/likegeeks/*
do
if [ -d "$path" ]
then
echo "$path is a directory"
elif [ -f "$path" ]
then
echo "$path is a file"
fi
done

#!/bin/bash
for (( v=1; v <= 10; v++ ))
do
echo "value is $v"
done

#!/bin/bash
echo "You are using $(basename $0)"
for n in $*
do
    echo "Hello $n"
done
exit 0


#!/bin/bash
for (( v1 = 1; v1 <= 5; v1++ ))
do
echo "$v1"
done > file


#!/bin/bash
for (( v1 = 1; v1 <= 3; v1++ ))
do
echo "First loop $v1:"
for (( v2 = 1; v2 <= 3; v2++ ))
do
echo " Second loop: $v2"
done
done


#!/bin/bash
# Author: @theurbanpenguin
# Web: www.theurbapenguin.com
# Script to ping servers from file
# Last Edited: August 2015
if [ ! -f "$1" ] ; then
  echo "The input to $0 should be a filename"
  exit 1
fi
echo "The following servers are up on $(date +%x)" > server.out
while read server
do
  ping -c1 "$server" && echo "Server up: $server" >> server.out
done < $1
cat server.out


8.8.8.8
8.8.4.4
```

```

#!/bin/bash
file="file1.txt"
IFS=$'\n'   #Here we change the default IFS to be newline
for var in $(cat $file)
do
echo " $var"
done

```
```
#!/bin/bash
file="file1.txt"
for var in $(cat $file)
do
echo " $var"
done
```
### file1.txt
```
Hello, this is a test
This is the second line
And this is the last line
```
```

