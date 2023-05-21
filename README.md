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

## Exploring  a file

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
