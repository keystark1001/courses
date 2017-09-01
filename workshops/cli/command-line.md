# Introduction to the Command Line Interface (CLI)

Requirements:

* MacOS / Linux users: Terminal
* Windows: PuTTY [[Download](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)]

## Navigating the file system

Learn your way around without feeling stuck. These commands help you change directories and view their content.

List files/folders in a directory:

    ls

List all files (even hidden) in a directory, with detailed info:

    ls -al

List all files sorted by most recent edits:

    ls -alt

Return the present working directory (where I am now):

    pwd

Change directories:

    cd <dir>

More versions of changing directories:

    cd ..
    cd ../../
    cd ../dir

Change to my home directory:

    cd ~

Change to the base directory:

    cd /

Switch back to the directory I was in before this one:

    cd -

Clear the screen. Get rid of the chaos!:

    clear


## Changing the file system

Create a file without any contents:

    touch myfile.txt

Show the contents of a file (concatenate):

    cat myfile.txt

Show only the first 20 lines or so of a file:

    head myfile.txt

Show only the last few lines of a file:

    tail myfile.txt

POSIX ownership bits:

    drwxr-xr-x   5 user  staff      170 Feb  3  2017 gocode
    drwxr-xr-x  12 user  staff      408 Jun  8 09:41 miniconda2
    drwxr-xr-x   5 user  staff      170 Jun  8 09:36 sandbox
    drwxr-xr-x   4 user  staff      136 Apr 28 09:40 scripts

Copy command:

    cp myfile.txt newfile.txt

Copy something in a folder to another folder:

    cp folder/item.txt folder2/

Copy everything in this directory to a folder:

    cp * folder/

Copy just .txt files into a folder:

    cp *.txt folder/

Move all .txt files into a folder:

    mv *.txt folder/

## Redirecting Input/Output

Echo command writes arguments to output (the screen):

    echo "I am learning the command line"

You can also echo statements into files:

    echo "Here is some content for my file" > fileA

Note the single > which overwrites all previous contents of that file.

To simply ADD more contents to an existing file, use >>

    echo "Here is even more content for my file" >> fileB

Similarly, you can cat out the contents of files into other files to overwrite them:

    cat myfile.txt > fileC

Or you can append a file to another file:

    cat myfile.txt >> fileD

## Configuring your environment

    $VARIABLES
    apt install xxxxx
    pip install xxxxx

## Understanding your environment

Processes running:

    htop

Current date-time:

    date

Uptime (how long in days/hours/minutes)

    uptime
