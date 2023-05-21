# gnu-linux guide

## Some types of bash

- bash shell
- z shell
- PoweShell
- C shell
- Bourne Shell 
- Fish Shell

## Basic Comands

```linux
ls
```
> to list content from a directory

```
ls -l
```
> to see more information about the files inside a directory

```
ls -lh
```
> to see more information about the files inside a directory in a more legit form

```
ls -la
```
> to see hidden information about the files inside a directory 

```
cd
```
> Change from directory

```
clear 
```
> To clear terminal info or use control + l

```
pwd  
```
> Print working directory

```
file
```
> Describe metadata from a file

```
tree  
```
> Describe in a tree form our relative path

```
touch 
```
> Create a file

```
mkdir 
```
> Create a directory

```
cp [original_file] [copy_file]
```
> Copy a file

```
mv [original_file] [copy_file]
```
> Move or rename a file

```
rm 
rm -r 
```
> Delete a file or a directory

```
rm -i 
```
> Delete a file but ask for a confirmation

## Exploring a file

```
head [file_name]
head [file_name] -n 15
tail [file_name]
tail [file_name] -n
less [file_name]
less [file_name]
```
> See the first lines of a text file

```
type
```
> See the type of a comand

```
alias [comand]
```
> Create a alias to run comands

```
help
whatis
```
> See more information about a comand

## Wildcards

```
ls *.txt
ls [info]*
```
> Filter by extension or name

```
ls [info]? 
ls [info]??
```
> Filter by characters number

```
ls [[:upper:]]*
ls -d [[:upper:]]*
ls -d [[:lower:]]*
``` 
> Filter by UpperCase or lowerCase

```
ls [abc]*
``` 
> Filter by Characters 


## Redirecting

```
stdin 1 ? stdout 1 : stderr 2
ls -lh /courses > courses.txt 
ls -lh /courses >> courses.txt 
ls -lh dsdfs 2> error.txt 
ls -lh addaa > output.txt 2>&1
```

## Pipe operator

```
echo "Hello world!"
```

> Generate a stdout text on terminal 

```
ls -lh | tail -n 10
ls -lh | tee output.txt | less
ls -lh | sort | tee output.txt | cat
```

## Operator control

```
ls; mkdir temporal; cal; ls;
```

> Syncronouse using ;

```
ls & date
```
> Asyncronus

```
cd jjj && touch test.txt
cd jjj || touch test.txt && echo "archivo creado"
```
> Asyncronus with conditional

## Permissions

```
[d]rwxr-xr-x
```
> File types
- -: Normal file
- d: Directory
- l: simbolic link
- b: block file

```
    Owner  Group  World
[d] [rwx]  [r-x]  [r-x]
     1 1 1 1 0 1 1 0 1
```
> Mode types
- r: Read
- w: Write
- x: Execute 

```
chmod 777
```
> Give permission to a file or directory 

```
whoami
```
> See current user

```
passwd
```
> Change pass from the current user

## Enviroment variables

```
printenv
```
> See current enviroment variables 

```
echo $PATH
```
>> This variable contains binary references to our programs

```
cd ~ | vi .bashrc
```
>> This file contains env variables configuration and alias configurations

```
PATH=$PATH:/path
```
>> This is how we can add a new path to the $PATH variable

## Simbolic Links

```
ln -s /path
```
> Direct access to a path

## Absolute paths operators

```
cd ~
cd /
```

## Relative paths operators

```
cd ..
cd ../..
```

## Notes

To open a directory or file with a GUI using WSL we can use ``wslview`` 

## Theory

> What is a comand?
- Is a executable program. 
- Is a shell utility. 
- Is a function. 
- Is a alias. 

