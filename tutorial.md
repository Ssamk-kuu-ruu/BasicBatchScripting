# Basics of Batch Scripting

### What do we need?
- **Visual Studio Code** or **Notepad**
- **Command Prompt**
- **File Format (.bat)**

#

### Basic Command Execution
- Echo
- Variables
- Comment
- ENV Variables
- String Concatenation
- Maths
- Input
- Command Argument
- Functions
- Local Scope
- Conditionals
- FOR Loop
- ERROR LEVEL
- Log files

#
if you want to display something on the console:

```bat
echo Hello World!
echo 519
```
    Hello World!
    519

#
if you just want to display an output on cmd:

```bat
@echo off
```
#

### The @ symbol...

```bat
@echo This is a sentence.

@vol 

@ver
```
    This is a sentence.

    Volume in drive C is Windows.
    Volume serial number is -----.

    Microsoft Windows [Version 10.0.----]

vol = volume  
ver = version  
***"@ symbol is preventing that particular prompt so it is not displaying batchscript in cmd everytime before executing the output."***
#

### The Variables (cmd version)

```cmd
set var = Kkuru

echo %var%
```
    Kkuru

#

```cmd
set myCommand = dir

echo %myCommand%
```
    Directory of ------

#

### The Variables (batch version)

if you want to call the variable and you want to display the data thatw as just store, use the % sign at the variable name.

```bat
@echo off

set filename = test.txt

echo The file name is %filename%
```
    The file name is test.txt

#

### Comments

There are two ways to perform or use comment in batchscripting:

```bat
rem This is a comment.
:: This is also a comment.
```

#

### ENV Variables

in order to display the environment variable, use "set".

```bat
@echo off

rem to see the whole env variable
set

rem if you want to switch back, remember to use set first to check the whole env variable
cd %SystemRoot%
dir
```
    Directory of C:\Windows
    ----------

#

### String Concatenation

Just adding two strings.

```bat
@echo off

set statement = My name is

set statement2 = Kkuru

set complete = %statement% %statement2%

echo %result%
```
    My name is Kkuru